<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=00Jane&&theme=tokyonight" alt="Jane" /></p>
<style>
 body{
    width: 100%;
    height: 100%;
    background: #0d0d2d;
    }
  .container {
            width: 400px;
            height: 400px;
            margin: 0 auto;
            perspective: 180px;
        }
    .window {
        position: absolute;
        top: 0;
        left: 0;
        width: 400px;
        height: 200px;
        transform: translate3d(250px, 110px, -190px) rotateY(110deg);
    }
    .window::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: #999;
            z-index: 1;
        }
    .window::after {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background:
                linear-gradient(0deg, transparent 12px,  #0d0d2d 12px,  #0d0d2d 15px),
                linear-gradient(90deg,  #0d0d2d 20px, transparent),
                linear-gradient(90deg,  #0d0d2d 20px, transparent),
                linear-gradient(90deg,  #0d0d2d 5px, transparent),
                linear-gradient(90deg,  #0d0d2d 5px, transparent);
        background-size: 100% 15px, 20px 100%, 20px 100%, 5px 100%, 5px 100%;
        background-repeat: repeat, no-repeat, no-repeat, no-repeat, no-repeat;
        background-position: 0 10px, 100px 0, 280px 0, 50px 0, 200px 0;
        z-index: 3;
    }
    .window .moon {
        position: absolute;
        width: 60px;
        height: 100px;
        top: 13px;
        left: 3px;
        background: #e6e6e6;
        z-index: 2;
        border-radius: 50%;
        box-shadow: inset 16px 5px 8px #e6e6e6;
        -webkit-transform: scale(0.6);
        transform: scale(0.3);
      }
    .floor {
        position: absolute;
        top: 0;
        left: 0;
        width: 400px;
        height: 200px;
        transform: translate3d(7px, 270px, -115px) rotateZ(-90deg) rotateY(100deg);
    }
    .floor::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: #999;
        z-index: 1;
    }
    .floor::after {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background:
        linear-gradient(0deg, transparent 12px,  #0d0d2d 12px,  #0d0d2d 15px),
        linear-gradient(90deg,  #0d0d2d 20px, transparent),
        linear-gradient(90deg,  #0d0d2d 20px, transparent),
        linear-gradient(90deg,  #0d0d2d 5px, transparent),
        linear-gradient(90deg, #0d0d2d 5px, transparent);
        background-size: 100% 15px, 20px 100%, 20px 100%, 5px 100%, 5px 100%;
        background-repeat: repeat, no-repeat, no-repeat, no-repeat, no-repeat;
        background-position: 0 10px, 100px 0, 280px 0, 50px 0, 200px 0;
        z-index: 2;
    }
    .door {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate3d(-50%, -50%, -290px);
        width: 50px;
        height: 100px;
        border-radius: 100px 100px 0 0 ;
        background: linear-gradient(45deg, transparent 65%, #999);
        box-shadow: inset -5px 5px 4px #999;
    }
</style>
<body>
<div class="container">
    <div class="window">
        <div class="moon"></div>
    </div>
    <div class="floor"></div>
    <div class="door"></div>
</div>
</body>


