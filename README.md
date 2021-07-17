<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Landing page UI design with HTML & CSS</title>
    <link href="pizza.html" rel="stylesheet" type="text/css">
    <style>
        *{
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        img{
            max-width: 100%;
        }
        body{
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            overflow-x: hidden;
            overflow-y: scroll;

        }
        header{
            padding: 15px 70px;
            display: inline-block;
            width: 100%;
        }
        .logo{
            float:left;
        }
        .menu{
            float: right;
            margin: 15px;
        }
        ul li{
            list-style: lower-greek;
            display: inline-block;
            margin: 0 25px;
        }
        ul li a{
            font-size: 16px;
            text-decoration:none;
            color: #000;
            font-weight: 700;
            
        }
        .left{
            width: 50%;
            float: left;
            text-align: right;
            padding: 0 0 0 80px;
        }
        .right{
            width: 50%;
            float: right;
            padding:100px 50px;

        }
        .right h1{
            font-size: 72px;
            font-weight: 500;
        }
        .right p{
            padding: 15px 0;
            font-size: 16px;
        }
        .right a{
            display: inline-block;
            padding: 15px 40px;
            background-color: #fff;
            text-decoration: none;
            color: rgb(248, 110, 31);
            font-weight: 700;
            font-size: 18px;
            margin-top: 50px;
            box-shadow: 0 0 24px rgba(0,0,0,0.16);
        }
        .square{
            position: absolute;
            top: 0;
            left: 0;
            width: 500px;
            height: 500px;
            background-color: #ffb300;
            z-index: -1;
        }
        .grid{
            position: absolute;
            bottom: 70px;
            left: -70px;
        }
        .scrolldown{
            position: absolute;
            bottom: 100px;
            right: 30px;
            font-weight: 500;
            transform: rotate(90deg);

        }
    </style>
</head>
<body>
    <div class="wrapper">
        <header>
            <div class="logo">
                <img src="" alt="">
            </div>
            <div class="menu">
                <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Menu</a></li>
                <li><a href="#">Offer</a></li>
                <li><a href="#">Contacts</a></li>
                </ul>
            </div>
        </header>
        <div classs="content">
            <div class="left">
                <img class="js-tilt" src="580b57fcd9996e24bc43c1e0.png"alt="">
            </div>
            <div class="right">
                <h1>Cheesy & Spicy Pizza only</h1>
                <p>Treat yourself with the delicious and cheesy bite of pizza making your time a memorable one!
                    WHAT ARE YOU WAITING FOR?
                </p>
                <a class="js-tilt" href="#">ORDER NOW</a>
            </div>
        </div>
        <div class="grid"><img src="" alt""></div>
        <div class="square"></div>
        <div class="scroll">SCROLL DOWN</div>
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/tilt.js/1.2.1/tilt.jquery.min.js"></script>
    <script type="text/javascript">
    $('.js-tilt').tilt({
    glare: true,
    maxGlare: .5,
    scale: 1.1
})
    </script>
</body>
</html>
