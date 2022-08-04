<! --- Full Credits Goes To NotReallyShikhar & TeamYukki --->
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="shortcut icon" href="favicon.png" type="image/x-icon">
    <title>Heroku Deployer</title>
</head>
<meta http-equiv="X-UA-Compatible" content="ie=edge">
<style>
    @import url(https://fonts.googleapis.com/css?family=Oswald|Roboto);

    @-webkit-keyframes btn {

        0%,
        100% {
            -moz-transform: scale(1);
            -ms-transform: scale(1);
            -webkit-transform: scale(1);
            transform: scale(1);
        }

        70% {
            -moz-transform: scale(1);
            -ms-transform: scale(1);
            -webkit-transform: scale(1);
            transform: scale(1);
        }

        80% {
            -moz-transform: scale(1.04);
            -ms-transform: scale(1.04);
            -webkit-transform: scale(1.04);
            transform: scale(1.04);
        }

        90% {
            -moz-transform: scale(0.96);
            -ms-transform: scale(0.96);
            -webkit-transform: scale(0.96);
            transform: scale(0.96);
        }
    }

    @-moz-keyframes btn {

        0%,
        100% {
            -moz-transform: scale(1);
            -ms-transform: scale(1);
            -webkit-transform: scale(1);
            transform: scale(1);
        }

        70% {
            -moz-transform: scale(1);
            -ms-transform: scale(1);
            -webkit-transform: scale(1);
            transform: scale(1);
        }

        80% {
            -moz-transform: scale(1.04);
            -ms-transform: scale(1.04);
            -webkit-transform: scale(1.04);
            transform: scale(1.04);
        }

        90% {
            -moz-transform: scale(0.96);
            -ms-transform: scale(0.96);
            -webkit-transform: scale(0.96);
            transform: scale(0.96);
        }
    }

    @keyframes;

    @-webkit-keyframes fish {

        0%,
        70% {
            opacity: 0;
        }

        100% {
            opacity: 1;
        }
    }

    @-moz-keyframes fish {

        0%,
        70% {
            opacity: 0;
        }

        100% {
            opacity: 1;
        }
    }

    @keyframes;

    html {
        height: 100%;
    }

    body {
        font-family: Roboto, sans-serif;
        color: #515a6e;
        background-color: #d5eafc;
        height: 100%;
        margin: 0;
        overflow: hidden;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-align: center;
        -ms-flex-align: center;
        align-items: center;
        -webkit-box-pack: center;
        -ms-flex-pack: center;
        justify-content: center;
    }

    a {
        cursor: pointer;
        color: #000;
        text-decoration: none;
        -moz-transition: all 0.3s;
        -o-transition: all 0.3s;
        -webkit-transition: all 0.3s;
        transition: all 0.3s;
    }

    a:hover {
        color: #ff5050;
    }

    .fish,
    .fish-shadow {
        width: 640px;
        height: auto;
        position: absolute;
        top: -145px;
        left: -177px;
        -moz-animation: fish 3s forwards ease-in-out;
        -webkit-animation: fish 3s forwards ease-in-out;
        animation: fish 3s forwards ease-in-out;
    }

    .fish path,
    .fish-shadow path {
        fill: #fff;
    }

    .fish path:hover,
    .fish-shadow path:hover {
        fill: #ff6100;
    }

    .fish .line,
    .fish-shadow .line {
        fill: none;
    }

    .fish-shadow-con {
        opacity: 0.2;
        filter: blur(10px);
        position: absolute;
        top: 0;
        left: 0;
    }

    .fish-shadow {
        top: -125px;
        left: -157px;
    }

    .fish-shadow path {
        fill: #211922;
    }

    .fish-shadow path:hover {
        fill: #211922;
    }

    .fish-shadow {
        -webkit-filter: url("#goo");
        filter: url(#goo);
        top: -125px;
        left: -157px;
        opacity: 0.4;
    }

    .container {
        position: relative;
        background-color: #fafafe;
        border-radius: 10px;
        margin: 40px;
        padding: 25px 20px 10px;
        box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        width: 320px;
        box-sizing: border-box;
    }

    .container:before {
        content: "";
        position: absolute;
        left: 0;
        bottom: 0;
        right: 0;
        height: 60%;
        background-color: #fafafe;
        border-radius: 10px;
        z-index: 2;
    }

    .card {
        position: relative;
        z-index: 2;
    }

    .card_title {
        font-size: 24px;
        margin: 0;
    }

    .card_title-info {
        font-size: 14px;
        margin: 7px 0 10px;
    }

    .card_button {
        border-radius: 4px;
        border: none;
        outline: none;
        width: 100%;
        padding: 0 15px;
        font-size: 18px;
        line-height: 36px;
        font-weight: 500;
        margin: 25px 0 10px;
        color: #fff;
        background: linear-gradient(#ff6100, #ff5050);
        box-shadow: 0 2px 12px -3px #ff5050;
        -moz-animation: btn 6s 3s infinite ease-in-out;
        -webkit-animation: btn 6s 3s infinite ease-in-out;
        animation: btn 6s 3s infinite ease-in-out;
        opacity: 0.9;
        -moz-transition: all 0.3s;
        -o-transition: all 0.3s;
        -webkit-transition: all 0.3s;
        transition: all 0.3s;
    }

    .card_button:hover {
        opacity: 1;
        box-shadow: 0 2px 2px -3px #ff5050;
    }

    .card_info {
        font-size: 14px;
    }

    .input {
        display: flex;
        flex-direction: column-reverse;
        position: relative;
        padding-top: 10px;
    }

    .input+.input {
        margin-top: 10px;
    }

    .input_label {
        color: #8597a3;
        position: absolute;
        top: 20px;
        -moz-transition: all 0.3s;
        -o-transition: all 0.3s;
        -webkit-transition: all 0.3s;
        transition: all 0.3s;
    }

    .input_field {
        border: 0;
        padding: 0;
        z-index: 1;
        background-color: transparent;
        border-bottom: 2px solid #eee;
        font: inherit;
        font-size: 14px;
        line-height: 30px;
    }

    .input_field:focus,
    .input_field:valid {
        outline: 0;
        border-bottom-color: #665856;
    }

    .input_field:focus+.input_label,
    .input_field:valid+.input_label {
        color: #665856;
        -moz-transform: translateY(-25px);
        -ms-transform: translateY(-25px);
        -webkit-transform: translateY(-25px);
        transform: translateY(-25px);
    }

    .input_eye {
        position: absolute;
        bottom: 0;
        right: 0;
        width: 36px;
        height: 30px;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-align: center;
        -ms-flex-align: center;
        align-items: center;
        -webkit-box-pack: center;
        -ms-flex-pack: center;
        justify-content: center;
    }

    .input_eye svg {
        width: 24px;
        height: auto;
        stroke: #8597a3;
    }

    .link {
        position: absolute;
        bottom: 20px;
        right: 20px;
        z-index: 3;
    }

    .rabbit {
        width: 50px;
        height: 50px;
        fill: #fff;
    }
</style>
</head>

<body>
    <!-- partial:index.partial.html -->
    <script async defer src="https://buttons.github.io/buttons.js"></script>
    <div class="container">
        <div class="card">
            <h1 align="center" class="card_title"><b>Heroku Deployer</b></h1>
            <p align="center"><a class="github-button" href="https://github.com/MerissaRobot"
                    data-color-scheme="no-preference: dark; light: dark; dark: dark;" data-size="large"
                    data-show-count="true" aria-label="Follow @NotReallyShikhar On Github">MerissaRobot</a></p>
            <p align="center">
                <a href="https://github.com/MerissaRobot/MerissaRobot"> Source |</a>
                <a href="https://t.me/MerissaRobot"> Telegram |</a>
                <a href="https://t.me/MerissaxSupport"> Channel </a>
            </p>
            <p align="center" class="card_title-info">Deploy Now!</p>
            <form class="card_form">
                <div class="input">
                    <input type="text" class="input_field" required id="myInput"/>
                    <label class="input_label">Input Your Forked Repo Link</label>
                </div>
                <button class="card_button" onclick="getInputValue();">Deploy Now </button>
            </form>
        </div>
        <script>
            function getInputValue(){
            var inputVal = document.getElementById("myInput").value;
            if (inputVal == "") {
                return alert("Provide Your Github Repo Link!");
            }
            if (inputVal.includes("TeamYukki")) {
                return alert("You Can't Deploy Official Repo As It Has Been Blacklisted By Heroku. Simply Fork The Repo & Then Input Your Forked Repo Link Here!");
            } else {
                if (inputVal.includes("https://github.com/")) {
                    her = "https://dashboard.heroku.com/new?template=";
                    herokulink = her.concat(inputVal);
                    window.open(herokulink,"blank");
                } else {
                    return alert("Input Github Link Starting With https:// Only!");
                }
            }
        }
        </script>
    </div>
</body>

</html>
