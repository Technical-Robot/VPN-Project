<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VPN Toggle Button</title>
    <style>
        html {
            font-size: 62.5%;
        }

        .bigbox {
            height: 90vh;
            width: 100%;
            display: grid;
            background-color: rgb(251, 215, 187);
            /* align-items: center; */
            justify-content: center;
            align-content: center;
        }
        .vpnlogo {
            display: inline-block;
            width: 220px;
            height: 200px;
            padding: 15px 0px;
            background-position: center;
            background-repeat: no-repeat;
            background-image: url(vpn-old-pic.png);
            /* background-color: #fff; */
        }

        .big-cleint {
            height: 10vh;
            width: 212px;
            display: inline-block;
            padding: 4px;
            text-align: center;
            align-items: center;
            justify-content: center;
            /* background-color: #fff; */
        }

        .down-cleint {
            background-color: #000a00;
            height: 145px;
            width: 210px;
            margin: 10px 0px;
            padding: 0px;
            display: inline-block;
            align-items: center;
            /* margin-bottom: 50px; */
        }

        .down-cleint-pera {
            height: 100%;
            font-size: 14px;
            margin: -2px 0px;
            display: inline-block;
            overflow-y: scroll;
            border: 2px solid black;
            /* background-color: red; */
        }

        .list-box {
            height: 20px;
            width: 195px;
            display: inline-block;
            padding: 3px 0px;
            margin: 3px 2px;
            border-left: 1px solid rgb(255, 200, 0);
            border-right: 1px solid rgb(255, 200, 0);
            border-top: 1px solid rgb(255, 200, 0);
            border-bottom: 1px solid rgb(255, 200, 0);
            background-color: rgb(89, 18, 18);
            text-align: center;
        }
.flags-pic{
    text-align: center;
    width: 30px;
    float:left;
    list-style: none;
    margin: 1px 3px;
    display: inline-block;
    display: flex;
    background-color: #fff;
}
.Server-Name{
    color: rgb(12, 20, 241);
    font-size: 14px;
    font-weight: bold;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    width: 88px;
    margin: 1px 2px;
    display: inline-block;
    background-color: rgb(222, 243, 237);
}
.on-off{
    display: inline-block;
    width: 40px;
    background-color:rgb(30, 221, 19);
    font-family:system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    float: right;
    font-weight: bold;
    margin: 0px 4px;
    text-align: center;
}
        .box1 {
            width: 70px;
            margin: auto;
            margin-top: 4px;
            border-radius: 3rem;
            display: flex;
            background-color: #fff;
            align-items: center;
            justify-content: center;
        }

        .control-me {
            font-size: 14px;
            width: 212px;
            margin-top: 7px;
            font-weight: bold;
            position: relative;
            text-align: center;
            /* background-color: rgb(4, 255, 0); */
            font-family:Verdana, Geneva, Tahoma, sans-serif;
            color: black;
            padding: 3px 0px;
        }

        .switch {
            position: relative;
            display: inline-block;
            width: 7rem;
            height: 3rem;
            background-color: rgba(201, 24, 24, 0.837);
            border-radius: 2rem;
        }

        .switch::after {
            content: "";
            position: absolute;
            top: .1rem;
            left: .1rem;
            width: 2.8rem;
            height: 2.8rem;
            border-radius: 50%;
            background-color: #fff;
            transition: all 0.3s linear;
        }

        input[type="checkbox"]:checked+.switch::after {
            transform: translateX(4rem);
            /* Corrected typo in the property name */
        }

        input[type="checkbox"]:checked+.switch {
            background-color: #00ec00;
        }

        input[type="checkbox"] {
            display: none;
            background-color: red;
        }
    </style>
</head>

<body>
    <div class="box">
        <p></p>
    </div>

    <div class="bigbox">
        <div class="vpnlogo"></div>
        <div class="big-cleint">
            <div class="box1">
                <input type="checkbox" name="checkbox" id="toggle">
                <label for="toggle" class="switch"></label>
            </div>

            <div>
                <p class="control-me" style="text-align: center;">Not Connected</p>
            </div>
        </div>
        <div class="down-cleint">
            <div class="down-cleint-pera">
                <li class="list-box"><img src="flags/india.jpeg" class="flags-pic"><div class="Server-Name">India</div><div class="on-off">Off</div></li>

                <li class="list-box"><img src="flags/china.jpeg" class="flags-pic"><div class="Server-Name">China</div><div class="on-off">Off</div></li>

                <li class="list-box"><img src="flags/canada.png"  class="flags-pic"><div class="Server-Name">Canada</div><div class="on-off">Off</div>
                </li>

                <li class="list-box"><img src="flags/south-korea.png" class="flags-pic"><div class="Server-Name">South Korea</div><div class="on-off">Off</div></li>

                <li class="list-box"><img src="flags/pakistan-flag.png" class="flags-pic"><div class="Server-Name">Pakisthan</div><div class="on-off">Off</div>
                </li>

                <li class="list-box"><img src="flags/Nepal-flags.png" class="flags-pic"><div class="Server-Name">Nepal</div><div class="on-off">Off</div></li>

                <li class="list-box"><img src="flags/germany-flag.png" class="flags-pic"><div class="Server-Name">Germany</div><div class="on-off">Off</div></li>

                <li class="list-box"><img src="flags/United Kingdom-flag.png" class="flags-pic"><div class="Server-Name">U. Kingdom</div><div class="on-off">Off</div></li>

                <li class="list-box"><img src="flags/Malaysia -flag.png" class="flags-pic"><div class="Server-Name">Malaysia</div><div class="on-off">Off</div></li>

                <li class="list-box"><img src="flags/Switzerland-flag.png" class="flags-pic"><div class="Server-Name">Switzerland</div><div class="on-off">Off</div></li>

                <li class="list-box"><img src="flags/United State-flag.png" class="flags-pic"><div class="Server-Name">United State</div><div class="on-off">Off</div></li>
            </div>
        </div>
    </div>

    <script>
        const toggle = document.getElementById("toggle");
        const controlMe = document.querySelector(".control-me");
        const vpnlogo = document.querySelector(".vpnlogo");

        toggle.addEventListener("change", function () {
            if (toggle.checked) {
                controlMe.textContent = "Connected";
                vpnlogo.style.backgroundImage = "url('vpn-new-pic.png')"

            } else {
                controlMe.textContent = "Not Connected";
                vpnlogo.style.backgroundImage = "url('vpn-old-pic.png')"
            }
        });
    </script>
</body>

</html>