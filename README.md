<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cricket Live</title>

<style>
body{font-family:Arial;background:#f2f2f2;margin:0}
header{background:#009270;color:white;padding:10px;text-align:center}
.card{background:white;margin:10px;padding:10px;border-radius:5px}
button{padding:6px 10px;background:#009270;color:white;border:none}
</style>
</head>

<body>

<header>🏏 Cricket Live</header>

<div class="card">
  <b>Bangladesh vs India</b>
  <p>Bangladesh 145/4 (18.2)</p>
</div>

<button onclick="alert('Login clicked')">Login</button>

<script>
/* 🔴 JavaScript অবশ্যই script tag এর ভিতরে থাকবে */
const API_KEY = "PASTE_REAL_KEY_HERE";

/* এখন শুধু console এ দেখাবে */
fetch("https://api.cricapi.com/v1/currentMatches?apikey=" + API_KEY)
  .then(r => r.json())
  .then(d => console.log(d))
  .catch(e => console.log("API error", e));
</script>

</body>
</html>
