<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Srihari | AI Developer</title>

<script src="https://cdn.tailwindcss.com"></script>

<style>
html{
scroll-behavior:smooth;
}

.hero{
background:linear-gradient(-45deg,#0f172a,#1e293b,#0ea5e9,#06b6d4);
background-size:400% 400%;
animation:gradient 10s ease infinite;
}

@keyframes gradient{
0%{background-position:0% 50%}
50%{background-position:100% 50%}
100%{background-position:0% 50%}
}

.profile{
animation:float 4s ease-in-out infinite;
}

@keyframes float{
0%{transform:translateY(0)}
50%{transform:translateY(-15px)}
100%{transform:translateY(0)}
}

.card{
transition:.3s;
}

.card:hover{
transform:translateY(-10px);
box-shadow:0 20px 40px rgba(0,0,0,.3);
}
</style>
</head>

<body class="bg-slate-950 text-white">

<nav class="fixed w-full bg-black/30 backdrop-blur-md z-50">
<div class="max-w-7xl mx-auto flex justify-between p-5">
<h1 class="font-bold text-xl">Mandapalli Srihari</h1>

<div class="space-x-6">
<a href="#about">About</a>
<a href="#skills">Skills</a>
<a href="#projects">Projects</a>
<a href="#contact">Contact</a>
</div>
</div>
</nav>

<section class="hero min-h-screen flex items-center justify-center text-center px-4">

<div>

<img
src="C:\1283\hari_image.jpeg"
class="profile w-52 h-52 rounded-full mx-auto border-4 border-cyan-400 object-cover">

<h1 class="text-6xl font-bold mt-8">
Mandapalli Srihari
</h1>

<h2 id="typing"
class="text-cyan-300 text-3xl mt-4 h-12">
</h2>

<p class="mt-5 text-xl text-slate-200">
Python • React • AI • SQL • Machine Learning • HTML&CSS
</p>

<div class="mt-8">

<a href="#projects"
class="bg-cyan-500 px-8 py-4 rounded-xl mr-4">
Projects
</a>

<a href="C:\Users\asrit\Downloads\srihari_resume_removed.pdf"
class="border border-white px-8 py-4 rounded-xl">
Resume
</a>

</div>

</div>

</section>

<section id="about" class="max-w-6xl mx-auto py-20 px-5">

<h2 class="text-4xl font-bold mb-6">
About Me
</h2>

<p class="text-slate-300 text-lg">
Aspiring Software Developer skilled in Python,
JavaScript, React.js, SQL, DSA, OOP, Agile Development,
Machine Learning, and Agentic AI.
Passionate about solving real-world problems through technology.
</p>

</section>

<section id="skills" class="max-w-6xl mx-auto py-20 px-5">

<h2 class="text-4xl font-bold mb-10">
Skills
</h2>

<div class="grid md:grid-cols-4 gap-4">

<div class="bg-slate-800 p-5 rounded-xl">Python</div>
<div class="bg-slate-800 p-5 rounded-xl">React.js</div>
<div class="bg-slate-800 p-5 rounded-xl">Node.js</div>
<div class="bg-slate-800 p-5 rounded-xl">SQL</div>
<div class="bg-slate-800 p-5 rounded-xl">Machine Learning</div>
<div class="bg-slate-800 p-5 rounded-xl">Agentic AI</div>
<div class="bg-slate-800 p-5 rounded-xl">GitHub</div>
<div class="bg-slate-800 p-5 rounded-xl">REST APIs</div>

</div>

</section>

<section id="projects" class="max-w-6xl mx-auto py-20 px-5">

<h2 class="text-4xl font-bold mb-10">
Projects
</h2>

<div class="grid md:grid-cols-3 gap-6">

<div class="card bg-slate-800 p-6 rounded-xl">
<h3 class="text-xl font-bold">
Deep Fake Audio Detection
</h3>
<p class="text-slate-400 mt-3">
Deep learning system to detect AI-generated audio.
</p>
</div>

<div class="card bg-slate-800 p-6 rounded-xl">
<h3 class="text-xl font-bold">
FutureCart
</h3>
<p class="text-slate-400 mt-3">
YouTube sentiment analysis using NLP.
</p>
</div>

<div class="card bg-slate-800 p-6 rounded-xl">
<h3 class="text-xl font-bold">
Pulse News
</h3>
<p class="text-slate-400 mt-3">
Real-time news aggregation platform.
</p>
</div>

</div>

</section>

<section id="contact" class="max-w-6xl mx-auto py-20 px-5">

<h2 class="text-4xl font-bold mb-10">
Contact
</h2>

<p>Email: mandapallisrihari9999@gmail.com</p>
<p>Phone: +91 8247685885</p>
<p>GitHub: github.com/mandapallisrihari9667</p>
<p>LinkedIn: linkedin.com/in/mandapalli-srihari</p>

</section>

<script>
const roles=[
"Software Developer",
"Python Developer",
"AI Enthusiast",
"Agentic AI Learner"
];

let roleIndex=0;
let charIndex=0;

function type(){
if(charIndex<roles[roleIndex].length){
document.getElementById("typing").innerHTML +=
roles[roleIndex].charAt(charIndex);
charIndex++;
setTimeout(type,100);
}else{
setTimeout(erase,1500);
}
}

function erase(){
if(charIndex>0){
document.getElementById("typing").innerHTML =
roles[roleIndex].substring(0,charIndex-1);
charIndex--;
setTimeout(erase,50);
}else{
roleIndex=(roleIndex+1)%roles.length;
setTimeout(type,300);
}
}

type();
</script>

</body>
</html>
