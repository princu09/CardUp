## CardUp CSS Layout Free Source Code By NorthFox Developers

##### 📫 Connect with me here:<br />
 <br />
 <p>
  <a href="https://www.instagram.com/princu.09">
    <img src="https://img.shields.io/badge/princu.09-386938188?style=flat&logo=instagram&color=black">
  </a> &nbsp; 
  <a href="https://twitter.com/princu09">
    <img src="https://img.shields.io/badge/@princu09-30302f?style=flat&logo=twitter&color=black">
  </a>&nbsp; 
  <a href="https://github.com/princu09">
    <img src="https://img.shields.io/badge/@princu09-30302f?style=flat&logo=github&color=black">
  </a>&nbsp;
    <a href="https://www.t.me/proghub09">
    <img src="https://img.shields.io/badge/ProgHub09-386938188?style=flat&logo=telegram&color=black">
  </a>
</p>

![Video Here](https://github.com/princu09/CardUp/blob/master/CardUp.gif?raw=true)

HTML File :

```
<!-- Owner: NorthFox Developers
Developer: Prince Patel
Oraganization: NorthFox Group
Code: Totally Free For Developing -->

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CardUp</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" integrity="sha384-wvfXpqpZZVQGK6TAh5PVlGOfQNHSoD2xbE+QkPxCAFlNEevoEH3Sl0sibVcOQVnN" crossorigin="anonymous">
    <link rel="stylesheet" href="style.css">
    <link rel="icon" href="https://princu09.github.io/nfwebbuilder/img/logo.png" type="image/png" sizes="16x16">
</head>

<body>
    <div class="header">
        <h1>About Us</h1>
        <h3>NorthFox Developers</h3>
    </div>
    <div class="container">
        <div class="card">
            <div class="imgBx">
                <img src="https://princu09.github.io/nfwebbuilder/img/gaurav.jpg" alt="Image Here">
            </div>
            <div class="content">
                <h2>Gaurav Barot</h2>
                <p>Web Developer</p>
                <br>
                <p>10+ Projects Complated in 2 Year. More than 6 Months Experience.
                </p>
            </div>
        </div>
        <div class="card">
            <div class="imgBx">
                <img src="https://princu09.github.io/nfwebbuilder/img/owner2.jpg" alt="Image Here">
            </div>
            <div class="content">
                <h2>Prince Patel</h2>
                <p>Owner Of NorthFox Group</p>
                <br>
                <p>Web, Python, Flutter & PHP Developer</p>
                <br>
                <p>100+ Projects Complated in 1 Year. More than 2 Years Experience.
                </p>
            </div>
        </div>
        <div class="card">
            <div class="imgBx">
                <img src="https://princu09.github.io/nfwebbuilder/img/harshm.jpg" alt="Image Here">
            </div>
            <div class="content">
                <h2>Harsh Malhotra</h2>
                <p>Web Developer</p>
                <br>
                <p>15+ Projects Complated in 1.5 Year. More than 1 Year Experience.
                </p>
            </div>
        </div>
    </div>
</body>

</html>
```

CSS File :

```
html {
    scroll-behavior: smooth;
}

@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;1,100;1,200;1,300;1,400;1,500;1,600;1,700&display=swap');

/* Created By NorthFox Group */

* {
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
}

body {
    justify-content: center;
    align-items: center;
    background: url(BG.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

.header h1 {
    color: #fff;
    position: absolute;
    top: 20%;
    left: 50%;
    font-size: 50px;
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
}

.header h3 {
    font-weight: 600;
    letter-spacing: 5px;
    color: #fff;
    font-size: 15px;
    position: absolute;
    top: 24%;
    left: 50%;
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
}

.container {
    position: relative;
    max-width: 100%;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
}

.container .card {
    max-width: 300px;
    min-width: 300px;
    position: relative;
    height: 215px;
    border-radius: 5px;
    background: #fff;
    margin: 30px 10px;
    padding: 20px 15px;
    display: flex;
    flex-direction: column;
    box-shadow: 0 5px 202px rgba(0, 0, 0, 0.5);
    transition: 0.3s ease-in-out;
}

.container .card:hover {
    height: 400px;
}

.container .card:hover:nth-child(1) {
    height: 370px;
}

.container .card:hover:nth-child(3) {
    height: 370px;
}

.container .card .imgBx {
    position: relative;
    width: 260px;
    height: 260px;
    top: -60px;
    left: 20px;
    z-index: 1;
    box-shadow: 0 5px 20px rgba(0, 0, 0, 0.2);
}

.container .card .imgBx img {
    width: 100%;
    height: 100%;
    max-width: 100%;
    border-radius: 4px;
}

.container .card .content {
    position: relative;
    margin-top: -140px;
    padding: 10px 15px;
    text-align: center;
    color: #111;
    font-weight: 600;
    visibility: hidden;
    opacity: 0;
    transition: 0.3s ease-in-out;
}

.container .card:hover .content {
    visibility: visible;
    opacity: 1;
    margin-top: -40px;
    transition-delay: 0.3s;
}

@media screen and (min-width: 480px) {
    .container .card .imgBx {
        left: 20px;
    }
}

@media(max-width:1110px) {
    body {
        background: url(BG.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
    }
    .header {
        margin-bottom: 120px;
    }
    .header h1 {
        color: #fff;
        position: absolute;
        top: 5%;
        left: 50%;
        font-size: 40px;
        -ms-transform: translate(-50%, -50%);
        transform: translate(-50%, -50%);
    }
    .header h3 {
        font-weight: 600;
        letter-spacing: 5px;
        color: #fff;
        font-size: 12px;
        position: absolute;
        top: 9%;
        left: 50%;
        -ms-transform: translate(-50%, -50%);
        transform: translate(-50%, -50%);
    }
    .container .card {
        min-width: 300px;
        min-height: 250px;
    }
    .container .card:hover {
        height: 450px;
    }
    .container .card .imgBx {
        position: relative;
        width: 300px;
        height: 300px;
        top: -60px;
        left: 0px;
        z-index: 1;
        box-shadow: 0 5px 20px rgba(0, 0, 0, 0.2);
    }
    .container .card .imgBx img {
        width: 100%;
        height: 100%;
        max-width: 100%;
        border-radius: 4px;
    }
}

@media(min-width:400px) {
    .header h1 {
        color: #fff;
        position: absolute;
        top: 5%;
        left: 50%;
        font-size: 35px;
        -ms-transform: translate(-50%, -50%);
        transform: translate(-50%, -50%);
    }
    .header h3 {
        font-weight: 600;
        letter-spacing: 5px;
        color: #fff;
        font-size: 9px;
        position: absolute;
        top: 8%;
        left: 50%;
        -ms-transform: translate(-50%, -50%);
        transform: translate(-50%, -50%);
    }
}
```
