# socialicons1
Social Icons hover Effect using only Html &amp; css
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css"
        integrity="sha512-SzlrxWUlpfuzQ+pcUCosxcglQRNAq/DZjVsC0lE40xsADsfeQoEypE+enwcOiGjk/bSuGGKHEyjSoQ1zVisanQ=="
        crossorigin="anonymous" referrerpolicy="no-referrer" />
    <!-- <link rel="stylesheet" href="icon.css"> -->
    <style>
        *{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: sans-serif;
}
.hero{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    min-height: 100vh;
    width: 100%;
    background: linear-gradient(45deg,silver ,gold);
}
.hero h1{
    font-size: 50px;
    font-weight: 700;
    margin-bottom: 100px;
    margin-top: -100px;
    text-shadow: 0 10px 20px rgba(0,0,0,0.5);
}
.hero .icons{
    display: flex;
}
.hero .icons a{
    width: 80px;
    height: 80px;
    text-align: center;
    text-decoration: none;
    color: #000;
    box-shadow: 0 0 20px 10px rgba(0,0,0,0.08);
    margin: 0 30px;
    border-radius: 50%;
    position: relative;
    overflow: hidden;
   
}
.hero .icons a .fa-brands{
    font-size: 45px;
    line-height: 80px;
    position: absolute;
    top: 0;
    left: 20px;
    z-index: 1;
    transition: 0.7s;
}
.hero .icons a::after{
    position: absolute;
    top: -80px;
    left: 0;
    content: '';
    width: 100%;
    height: 100%;
    background: linear-gradient(45deg, red, blue);
    transition: 0.7s;
}
.hero .icons a:hover::after{
    position: absolute;
    top: 0;
}
.hero .icons a:hover .fa-brands{
    color: #fff;
}
    </style>
</head>

<body>
    <div class="hero">
        <h1>Socail Icons Hover Effect</h1>
        <div class="icons">
            <a href=""><i class="fa-brands fa-facebook"></i></a>
            <a href=""><i class="fa-brands fa-whatsapp"></i></a>
            <a href=""><i class="fa-brands fa-twitter"></i></a>
            <a href=""><i class="fa-brands fa-instagram"></i></a>
            <a href=""><i class="fa-brands fa-linkedin"></i></a>
        </div>
    </div>
</body>

</html>
