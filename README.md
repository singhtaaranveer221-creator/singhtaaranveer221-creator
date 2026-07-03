<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Taranveer Singh | Developer</title>

    <link rel="stylesheet" href="style.css">

    <link rel="preconnect" href="https://fonts.googleapis.com">

    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap"
        rel="stylesheet">

</head>

<body>

    <!-- Background -->

    <div class="background"></div>

    <!-- Navbar -->

    <nav>

        <h2 class="logo">TS.</h2>

        <ul>

            <li><a href="#home">Home</a></li>

            <li><a href="#about">About</a></li>

            <li><a href="#skills">Skills</a></li>

            <li><a href="#projects">Projects</a></li>

            <li><a href="#contact">Contact</a></li>

        </ul>

    </nav>

    <!-- Hero -->

    <section id="home" class="hero">

        <div class="hero-left">

            <h1>Hi, I'm <span>Taranveer Singh</span></h1>

            <h2 id="typing"></h2>

            <p>

                Passionate Computer Science student who enjoys building websites,

                solving problems and learning modern technologies.

            </p>

            <div class="buttons">

                <a href="#projects" class="btn">Projects</a>

                <a href="#contact" class="btn-outline">Contact</a>

            </div>

        </div>

        <div class="hero-right">

            <div class="profile-card">

                <img src="https://avatars.githubusercontent.com/u/9919?s=200&v=4">

            </div>

        </div>

    </section>

    <!-- About -->

    <section id="about">

        <h2 class="section-title">About Me</h2>

        <div class="glass">

            <p>

                I'm Taranveer Singh, a Computer Science student from GGDSD College.

                I enjoy programming in C, C++, JavaScript and creating responsive

                websites. My goal is to become a Full Stack Developer and contribute

                to exciting projects.

            </p>

        </div>

    </section>

    <!-- Skills -->

    <section id="skills">

        <h2 class="section-title">Skills</h2>

        <div class="skills-grid">

            <div class="skill">
                <h3>C++</h3>
                <div class="bar"><span style="width:90%"></span></div>
            </div>

            <div class="skill">
                <h3>C</h3>
                <div class="bar"><span style="width:85%"></span></div>
            </div>

            <div class="skill">
                <h3>HTML</h3>
                <div class="bar"><span style="width:95%"></span></div>
            </div>

            <div class="skill">
                <h3>CSS</h3>
                <div class="bar"><span style="width:90%"></span></div>
            </div>

            <div class="skill">
                <h3>JavaScript</h3>
                <div class="bar"><span style="width:80%"></span></div>
            </div>

        </div>

    </section>

    <!-- Projects -->

    <section id="projects">

        <h2 class="section-title">Projects</h2>

        <div class="project-grid">

            <div class="card">

                <h3>Portfolio Website</h3>

                <p>Modern responsive portfolio built using HTML, CSS and JS.</p>

            </div>

            <div class="card">

                <h3>Linux Practice</h3>

                <p>Collection of Linux commands and shell scripting exercises.</p>

            </div>

            <div class="card">

                <h3>Upcoming Projects</h3>

                <p>More exciting repositories coming soon...</p>

            </div>

        </div>

    </section>

    <!-- Contact -->

    <section id="contact">

        <h2 class="section-title">Contact</h2>

        <div class="glass">

            <p>Email : your@email.com</p>

            <p>GitHub : github.com/yourusername</p>

            <p>Location : Pehowa, Haryana</p>

        </div>

    </section>

    <footer>

        © 2026 Taranveer Singh

    </footer>

    <script src="script.js"></script>

</body>

</html>
/* ===========================
   GOOGLE FONT
=========================== */
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
    font-family:'Poppins',sans-serif;
}

body{
    background:#0f172a;
    color:#fff;
    overflow-x:hidden;
}

/* ===========================
   ANIMATED BACKGROUND
=========================== */

.background{
    position:fixed;
    width:100%;
    height:100%;
    z-index:-1;
    background:
        radial-gradient(circle at top left,#6d28d9,transparent 30%),
        radial-gradient(circle at bottom right,#06b6d4,transparent 30%),
        #0f172a;
}

.background::after{
    content:"";
    position:absolute;
    width:100%;
    height:100%;
    background:linear-gradient(
        45deg,
        transparent,
        rgba(255,255,255,.03),
        transparent
    );
    animation:bgMove 8s linear infinite;
}

@keyframes bgMove{
    from{
        transform:translateX(-100%);
    }
    to{
        transform:translateX(100%);
    }
}

/* ===========================
   NAVBAR
=========================== */

nav{

    width:100%;
    padding:22px 9%;

    display:flex;
    justify-content:space-between;
    align-items:center;

    position:fixed;

    backdrop-filter:blur(15px);
    background:rgba(255,255,255,.05);

    z-index:1000;
}

.logo{

    font-size:32px;
    font-weight:700;
    color:#38bdf8;
}

nav ul{

    display:flex;
    gap:40px;
    list-style:none;
}

nav a{

    color:white;
    text-decoration:none;
    transition:.3s;
}

nav a:hover{

    color:#38bdf8;
}

/* ===========================
   HERO
=========================== */

.hero{

    min-height:100vh;

    display:flex;

    align-items:center;

    justify-content:space-between;

    padding:120px 10%;
}

.hero-left{

    width:55%;
}

.hero-left h1{

    font-size:58px;

    line-height:1.2;
}

.hero-left span{

    color:#38bdf8;
}

.hero-left h2{

    margin:20px 0;

    color:#c084fc;

    height:40px;
}

.hero-left p{

    color:#cbd5e1;

    line-height:1.8;

    margin-bottom:35px;
}

.buttons{

    display:flex;

    gap:20px;
}

.btn{

    padding:14px 34px;

    background:#38bdf8;

    color:white;

    text-decoration:none;

    border-radius:50px;

    transition:.3s;
}

.btn:hover{

    transform:translateY(-5px);

    box-shadow:0 10px 30px rgba(56,189,248,.5);
}

.btn-outline{

    padding:14px 34px;

    border:2px solid #38bdf8;

    color:white;

    border-radius:50px;

    text-decoration:none;

    transition:.3s;
}

.btn-outline:hover{

    background:#38bdf8;
}

/* ===========================
   PROFILE CARD
=========================== */

.hero-right{

    width:40%;

    display:flex;

    justify-content:center;
}

.profile-card{

    width:340px;

    height:340px;

    border-radius:30px;

    overflow:hidden;

    background:rgba(255,255,255,.05);

    backdrop-filter:blur(25px);

    box-shadow:0 0 40px rgba(0,0,0,.4);

    animation:float 5s ease-in-out infinite;
}

.profile-card img{

    width:100%;

    height:100%;

    object-fit:cover;
}

@keyframes float{

    0%{
        transform:translateY(0px);
    }

    50%{
        transform:translateY(-20px);
    }

    100%{
        transform:translateY(0px);
    }
}

/* ===========================
   SECTION
=========================== */

section{

    padding:100px 10%;
}

.section-title{

    text-align:center;

    font-size:40px;

    margin-bottom:50px;

    color:#38bdf8;
}

/* ===========================
   GLASS CARD
=========================== */

.glass{

    background:rgba(255,255,255,.05);

    backdrop-filter:blur(15px);

    border-radius:20px;

    padding:40px;

    color:#dbeafe;

    box-shadow:0 10px 30px rgba(0,0,0,.3);
}

/* ===========================
   SKILLS
=========================== */

.skills-grid{

    display:grid;

    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));

    gap:30px;
}

.skill h3{

    margin-bottom:10px;
}

.bar{

    width:100%;

    height:10px;

    background:#1e293b;

    border-radius:30px;

    overflow:hidden;
}

.bar span{

    display:block;

    height:100%;

    border-radius:30px;

    background:linear-gradient(to right,#38bdf8,#8b5cf6);

    animation:grow 2s ease;
}

@keyframes grow{

    from{
        width:0;
    }
}

/* ===========================
   PROJECTS
=========================== */

.project-grid{

    display:grid;

    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));

    gap:30px;
}

.card{

    background:rgba(255,255,255,.05);

    border-radius:20px;

    padding:30px;

    transition:.4s;

    backdrop-filter:blur(12px);

    cursor:pointer;
}

.card:hover{

    transform:translateY(-10px);

    box-shadow:0 20px 40px rgba(56,189,248,.25);
}

.card h3{

    color:#38bdf8;

    margin-bottom:15px;
}

.card p{

    color:#d1d5db;

    line-height:1.7;
}

/* ===========================
   CONTACT
=========================== */

#contact p{

    margin:15px 0;
}

/* ===========================
   FOOTER
=========================== */

footer{

    text-align:center;

    padding:30px;

    color:#94a3b8;

    border-top:1px solid rgba(255,255,255,.1);
}

/* ===========================
   SCROLLBAR
=========================== */

::-webkit-scrollbar{

    width:8px;
}

::-webkit-scrollbar-track{

    background:#0f172a;
}

::-webkit-scrollbar-thumb{

    background:#38bdf8;

    border-radius:10px;
}

/* ===========================
   RESPONSIVE
=========================== */

@media(max-width:900px){

    nav{

        flex-direction:column;

        gap:20px;
    }

    nav ul{

        gap:20px;

        flex-wrap:wrap;

        justify-content:center;
    }

    .hero{

        flex-direction:column-reverse;

        text-align:center;

        gap:60px;
    }

    .hero-left{

        width:100%;
    }

    .hero-right{

        width:100%;
    }

    .hero-left h1{

        font-size:42px;
    }

    .profile-card{

        width:260px;

        height:260px;
    }

}
// ================================
// Typing Animation
// ================================

const typingElement = document.getElementById("typing");

const words = [
    "Frontend Developer",
    "C++ Programmer",
    "JavaScript Enthusiast",
    "Linux Learner",
    "Future Full Stack Developer"
];

let wordIndex = 0;
let charIndex = 0;
let deleting = false;

function typeEffect() {

    const currentWord = words[wordIndex];

    if (!deleting) {

        typingElement.textContent = currentWord.substring(0, charIndex + 1);
        charIndex++;

        if (charIndex === currentWord.length) {
            deleting = true;
            setTimeout(typeEffect, 1800);
            return;
        }

    } else {

        typingElement.textContent = currentWord.substring(0, charIndex - 1);
        charIndex--;

        if (charIndex === 0) {
            deleting = false;
            wordIndex = (wordIndex + 1) % words.length;
        }
    }

    setTimeout(typeEffect, deleting ? 50 : 100);
}

typeEffect();


// ================================
// Navbar Background on Scroll
// ================================

const navbar = document.querySelector("nav");

window.addEventListener("scroll", () => {

    if (window.scrollY > 50) {

        navbar.style.background = "rgba(15,23,42,0.90)";
        navbar.style.boxShadow = "0 8px 30px rgba(0,0,0,.35)";

    } else {

        navbar.style.background = "rgba(255,255,255,.05)";
        navbar.style.boxShadow = "none";
    }

});


// ================================
// Fade In Sections
// ================================

const sections = document.querySelectorAll("section");

const observer = new IntersectionObserver((entries) => {

    entries.forEach(entry => {

        if (entry.isIntersecting) {

            entry.target.classList.add("show");

        }

    });

}, {
    threshold: 0.15
});

sections.forEach(section => {
    observer.observe(section);
});


// ================================
// Smooth Button Click Animation
// ================================

const buttons = document.querySelectorAll(".btn, .btn-outline");

buttons.forEach(button => {

    button.addEventListener("click", function () {

        this.style.transform = "scale(.95)";

        setTimeout(() => {

            this.style.transform = "";

        }, 150);

    });

});


// ================================
// Active Navigation Link
// ================================

const navLinks = document.querySelectorAll("nav ul li a");

window.addEventListener("scroll", () => {

    let current = "";

    sections.forEach(section => {

        const sectionTop = section.offsetTop - 120;

        if (pageYOffset >= sectionTop) {
            current = section.getAttribute("id");
        }

    });

    navLinks.forEach(link => {

        link.classList.remove("active");

        if (link.getAttribute("href") === "#" + current) {
            link.classList.add("active");
        }

    });

});


// ================================
// Project Card Hover Effect
// ================================

const cards = document.querySelectorAll(".card");

cards.forEach(card => {

    card.addEventListener("mousemove", (e) => {

        const rect = card.getBoundingClientRect();

        const x = e.clientX - rect.left;
        const y = e.clientY - rect.top;

        card.style.background =
            `radial-gradient(circle at ${x}px ${y}px,
            rgba(56,189,248,.25),
            rgba(255,255,255,.05) 60%)`;

    });

    card.addEventListener("mouseleave", () => {

        card.style.background = "rgba(255,255,255,.05)";

    });

});


// ================================
// Welcome Message
// ================================

window.addEventListener("load", () => {

    console.log("Welcome to Taranveer Singh's Portfolio 🚀");

});
