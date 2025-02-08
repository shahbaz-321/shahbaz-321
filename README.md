- 👋 Hi, I’m @shahbaz-321
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
shahbaz-321/shahbaz-321 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Valentine's Decision!</title>
<style>
body {
background-color: #ff69b4;
font-family: Arial, sans-serif;
text-align: center;
}

.container {
width: 80%;
margin: 40px auto;
background-color: #fff;
padding: 20px;
border-radius: 10px;
box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

button {
background-color: #ff69b4;
color: #fff;
border: none;
padding: 10px 20px;
font-size: 18px;
cursor: pointer;
}

button:hover {
background-color: #ff99cc;
}

.no-button {
position: absolute;
}

.yes-button {
transition: all 0.5s ease-in-out;
transform: scale(1);
}
</style>
</head>
<body>
<div class="container">
<h1>Will you be my Valentine, Shahbaz Jii? 🐱❤️</h1>
<button class="yes-button" onclick="yesClicked()">Yes! I love you, Shahbaz Jii! 😻</button>
<button class="no-button" onclick="noClicked()">No! 😊</button>
<p id="cat-text">You have 5 chances to say yes to Shahbaz Jii! 🐈</p>
</div>
<script>
let scale = 1;
let chances = 5;

function noClicked() {
document.querySelector('.no-button').innerHTML = 'No! 😠';
document.querySelector('.no-button').style.top = Math.random() * window.innerHeight + 'px';
document.querySelector('.no-button').style.left = Math.random() * window.innerWidth + 'px';
scale += 0.1;
document.querySelector('.yes-button').style.transform = 'scale(' + scale + ')';
chances--;
document.getElementById('cat-text').innerText = 'You have ' + chances + ' chances left to say yes to Shahbaz Jii! 🐈';
if (chances === 0) {
document.querySelector('.yes-button').style.transform = 'scale(10)';
document.querySelector('.yes-button').style.position = 'absolute';
document.querySelector('.yes-button').style.top = '0px';
document.querySelector('.yes-button').style.left = '0px';
document.querySelector('.yes-button').style.width = '100%';
document.querySelector('.yes-button').style.height = '100%';
}
}

function yesClicked() {
alert('Yay! You said yes to Shahbaz Jii! 😻');
document.querySelector('.no-button').innerHTML = 'No! 😊';
}
</script>
</body>
</html>
```
