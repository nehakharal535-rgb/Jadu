# Jadu
<!DOCTYPE html>
<html>
<head>
<title>Magic Chirag Login</title>
<style>
body { background: radial-gradient(circle, #1a1a4e, #05051a); text-align: center; color: #ffd700; font-family: Arial; margin: 0; min-height: 100vh; }
h1 { margin-top: 30px; }
.lamp { font-size: 100px; cursor: pointer; margin-top: 30px; transition: transform 0.3s; }
.lamp:hover { transform: scale(1.1); }
.smoke { width: 20px; height: 20px; background: #aaa; border-radius: 50%; margin: 5px auto; opacity: 0; }
body[data-rubbed="true"] .smoke { animation: rise 3s infinite; }
@keyframes rise {
  0% { transform: translateY(0) scale(1); opacity: 0.7; }
  100% { transform: translateY(-150px) scale(3); opacity: 0; }
}
.login { background: #222; border: 2px solid #ffd700; padding: 20px; border-radius: 15px; width: 300px; margin: 30px auto; display: none; box-shadow: 0 0 30px #ffd700; }
body[data-rubbed="true"] .login { display: block; animation: fadein 1.5s; }
@keyframes fadein { from { opacity: 0; } to { opacity: 1; } }
input { display: block; width: 90%; padding: 10px; margin: 10px auto; border-radius: 5px; border: none; }
button { background: #ffd700; color: #111; font-weight: bold; padding: 10px 30px; border: none; border-radius: 5px; cursor: pointer; }
#msg { color: #7CFC00; font-weight: bold; }
</style>
</head>
<body data-rubbed="false">
<h1>🪔 Magic Chirag Login 🪔</h1>
<div class="lamp" onclick="rubLamp()">🪔</div>
<div class="smoke" style="animation-delay: 0s"></div>
<div class="smoke" style="animation-delay: 1s"></div>
<div class="smoke" style="animation-delay: 2s"></div>
<p>Chirag ko ragdo! (Rub the lamp!)</p>
<div class="login">
<h2>Genie Hazir Hai!</h2>
<input type="text" placeholder="Username">
<input type="password" placeholder="Password">
<button onclick="askGenie()">Genie se Poocho</button>
<p id="msg"></p>
</div>
<script>
function rubLamp() {
  document.body.setAttribute('data-rubbed', 'true');
}
function askGenie() {
  document.getElementById('msg').innerText = '✨ Khwahish poori! Signed In! ✨';
}
</script>
</body>
</html>
```
