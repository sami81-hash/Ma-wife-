<!DOCTYPE html>
<html>
<head>
    <title>5 Months With My Favorite Human ❤️</title>

    <style>
        body {
            margin:0;
            font-family: Comic Sans MS, cursive;
            background: linear-gradient(270deg,#ff9a9e,#fad0c4,#fbc2eb,#a6c1ee);
            background-size: 800% 800%;
            animation: bgMove 10s infinite alternate;
            text-align:center;
            color:white;
        }

        @keyframes bgMove {
            0%{background-position:0% 50%;}
            100%{background-position:100% 50%;}
        }

        h1{
            font-size:45px;
            margin-top:40px;
            text-shadow:2px 2px 10px black;
        }

        .box{
            background:rgba(0,0,0,0.3);
            padding:20px;
            margin:20px auto;
            width:80%;
            border-radius:30px;
        }

        button{
            padding:15px 25px;
            border:none;
            border-radius:25px;
            font-size:18px;
            background:white;
            color:#ff4b6e;
            cursor:pointer;
        }

        button:hover{
            background:#ff4b6e;
            color:white;
        }

        #funny{
            display:none;
            font-size:22px;
            margin-top:20px;
        }

        .count{
            font-size:30px;
            margin-top:15px;
        }
    </style>
</head>

<body>

<h1>Happy 5 Months My Love ❤️</h1>

<div class="box">
    <p>We survived 5 months of long distance 😎</p>
    <p>Only <b>4 months</b> until I hug you forever 😭❤️</p>
    <div class="count" id="countdown"></div>
</div>

<div class="box">
    <button onclick="funny()">Click if you are obsessed with me 😏</button>

    <div id="funny">
        😳 Oops… you clicked it…<br><br>

        That means you are now OFFICIALLY married to me 💍😂  
        No cancel button. No refund. Lifetime subscription only 😌❤️  
        <br><br>

        Signed with our fingerprints 🖤<br><br>

        <img src="https://upload.wikimedia.org/wikipedia/commons/2/27/Fingerprint_Whorl.jpg" width="80">
        <img src="https://upload.wikimedia.org/wikipedia/commons/8/8c/Fingerprint_Loop.jpg" width="80">
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/1b/Fingerprint_Arch.jpg" width="80">

        <br><br>
        See you in 4 months my wife 😭❤️
    </div>
</div>

<!-- Background Music -->
<audio autoplay loop>
  <source src="https://cdn.pixabay.com/audio/2022/03/15/audio_3e2b6b3c2e.mp3" type="audio/mpeg">
</audio>

<script>
function funny(){
    document.getElementById("funny").style.display="block";
}

let meetDate = new Date();
meetDate.setMonth(meetDate.getMonth() + 4);

let x = setInterval(function() {
  let now = new Date().getTime();
  let distance = meetDate - now;

  let days = Math.floor(distance / (1000 * 60 * 60 * 24));
  let hours = Math.floor((distance % (1000*60*60*24)) / (1000*60*60));
  let minutes = Math.floor((distance % (1000*60*60)) / (1000*60));

  document.getElementById("countdown").innerHTML =
  "⏳ " + days + " days " + hours + " hours " + minutes + " minutes";
}, 1000);
</script>

</body>
</html>
