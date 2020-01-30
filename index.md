<!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta charset="utf-8">
    <link rel="stylesheet" href="http://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.4.0/css/font-awesome.min.css">
    <style>
        body {
            margin: 0px 0px 0px 0px;
            border-bottom: 0px;
            padding-bottom: 0px;
            max-width: 400px;
            max-height: 800px;
            background-color: aliceblue;
            font-family: serif;
        }
        .header, .footer {
            background-color: #1874c4;
            color: white !important;
            width: 400px;
            height: 50px;
            position: relative;
            top: -21px;
        }
        h1 {
            text-align: left;
            position: relative;
            top: 6px;
        }
        h3 {
            color: #1874c4;
        }
        span {
            font-size: 30px!important;
        }
        .content {
            position: relative;
            left: 15px;
            top: -21px;
        }
        img {
            height: 50px;
            width: 90px;
            border-radius: 50%;
        }
        .image {
            width: 25%;
            display: block;
            float: left;
        }
        .comment{
            width 90%;
            display: block;
        }
        #footer {
            color: white;
            position: relative;
            top: 12px;
            left: 10px;
        }
        .nav {
            height: 350px;
            width: 100px;
            background-color:#1874c4;
            position: fixed!important;
            top: 51px;
            z-index: 1;
            overflow: auto;
            display: none;
        }
        .nav a {
            text-decoration: none;
            color: white;
            padding: 4px 2px 4px 16px;
            display: block;
        }
        .nav a:hover {
            background-color: #fff;
            color: black;
        }
    </style>
</head>
<body>
    <nav class="nav" style="width:30%">
        <div class="closebutton">
            <button onclick="closenav()" class="button">x</button>
            <br>
        </div>
        <br>
        <a href="#">Home</a>		
        <a href="#">Classes</a>		
        <a href="#">Races</a>		
    </nav>
    
    <div class="header">
        <h1>&nbsp;&nbsp;<span onclick="opennav()" class="fa fa-bars"></span>&nbsp; D&amp;D Classes</h1>
    </div>
    <div class="content">
        <div class="image">
            <img src="https://s-media-cache-ak0.pinimg.com/236x/cd/f0/45/cdf045926f3688f1d214c3194bcc7835.jpg">
        </div>
        <div class="comment">
            <h3>The Mage</h3>
            <p>The Mage wields powerful magic to destroy her foes or aid her allies. </p>
        </div>
    </div>
    <div class="content">
        <div class="image">
            <img src="http://cdn.playbuzz.com/cdn/d0ade8ae-ca29-4a3f-8561-c64741f21380/a0c590fe-ab13-4da0-84c4-0f634e0fa2d6.png">
        </div>
        <div class="comment">
            <h3>The Thief</h3>
            <p>The Thief is a master of stealth, silently striking from behind.</p>
        </div>
    </div>
    <div class="content">
        <div class="image">
            <img src="https://sjcmindsports.files.wordpress.com/2014/05/arcane-warrior-2.jpg">
        </div>
        <div class="comment">
            <h3>The Warrior</h3>
            <p>The Warrior is a stalwart fighter and protector. Proficient with all manner of weapons.</p>
        </div>
    </div>
    <div class="content">
        <div class="image">
            <img src="https://s-media-cache-ak0.pinimg.com/736x/54/68/1e/54681e33c36c764920be0ff585c04726.jpg">
        </div>
        <div class="comment">
            <h3>The Cleric</h3>
            <p>The Cleric is a warrior who wields divine magic to heal or to curse.</p>
        </div>
    </div>

    <div class="footer">
        <h3 id="footer">&copy; Wizards of the Coast</h3>
    </div>
    <script>
        function opennav() {
            var x = document.getElementsByClassName("nav")[0];
            x.style.display = "block";
        }
        function closenav() {
            var x = document.getElementsByClassName("nav")[0];
            x.style.display = "none";
        }
    </script>
</body>
</html>
