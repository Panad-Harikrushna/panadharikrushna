<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Panad Harikrushna | Data Analyst</title>

    <style>
	* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    background: #02050b;
    color: white;
    font-family: Arial, Helvetica, sans-serif;
    overflow-x: hidden;
}

#particles {
    position: fixed;
    inset: 0;
    z-index: -1;
}

.banner {
    width: 100%;
    min-height: 100vh;
    padding: 25px 40px;

    background:
        radial-gradient(
            circle at 70% 50%,
            rgba(0, 140, 255, 0.12),
            transparent 40%
        ),
        radial-gradient(
            circle at 90% 80%,
            rgba(100, 0, 255, 0.12),
            transparent 35%
        );

    position: relative;
}


/* =========================
   TOP
========================= */

.top-line {
    display: flex;
    align-items: center;
    justify-content: space-between;

    border-bottom: 1px solid rgba(0, 190, 255, 0.2);

    padding-bottom: 18px;
}

.hello {
    color: #1ea7ff;
    font-size: 18px;
    font-weight: bold;
}

.top-skills {
    display: flex;
    gap: 30px;

    color: #d7e9ff;
    font-size: 15px;
}

.top-skills span {
    transition: 0.3s;
}

.top-skills span:hover {
    color: #00d9ff;
    transform: translateY(-3px);
}

.insight {
    border: 1px solid #00eaff;
    border-radius: 8px;

    padding: 8px 18px;

    color: #00f2ff;

    box-shadow:
        0 0 15px rgba(0, 220, 255, 0.3);
}


/* =========================
   HERO
========================= */

.hero {
    display: grid;

    grid-template-columns:
        1fr
        1.2fr
        1fr;

    gap: 40px;

    margin-top: 40px;
}


/* =========================
   LEFT
========================= */

.name h1 {
    font-size: clamp(55px, 6vw, 100px);

    letter-spacing: 8px;

    line-height: 0.9;

    color: white;
}

.name h2 {
    font-size: clamp(45px, 5vw, 80px);

    letter-spacing: 3px;

    color: #168fff;

    text-shadow:
        0 0 15px rgba(0, 150, 255, 0.5);
}

.role {
    margin-top: 18px;

    font-size: 14px;

    color: #d8e8f8;

    letter-spacing: 1px;
}

.role span {
    color: #008cff;

    margin: 0 8px;
}


/* FEATURES */

.features {
    margin-top: 35px;

    display: flex;
    flex-direction: column;

    gap: 15px;
}

.feature {
    display: flex;
    align-items: center;

    gap: 15px;

    color: #dce9f5;

    font-size: 16px;
}

.feature-icon {
    width: 35px;
    height: 35px;

    display: grid;
    place-items: center;

    border: 1px solid #009dff;

    color: #00bfff;

    border-radius: 8px;

    box-shadow:
        0 0 10px rgba(0, 170, 255, 0.2);
}


/* QUOTE */

.quote {
    margin-top: 30px;

    padding: 15px 20px;

    border-left: 2px solid #00bfff;

    background:
        linear-gradient(
            90deg,
            rgba(0, 150, 255, 0.1),
            transparent
        );
}

.quote strong {
    font-size: 40px;

    color: #00aaff;
}

.quote p {
    display: inline-block;

    color: #e7f3ff;

    line-height: 1.5;
}

.quote span {
    color: #00bfff;
}


/* =========================
   CENTER
========================= */

.center-section {
    display: flex;

    flex-direction: column;

    align-items: center;
}


/* HEADLINE */

.headline-box {
    margin-top: 30px;

    padding: 25px;

    text-align: center;

    border-left: 2px solid #00d9ff;
    border-right: 2px solid #00d9ff;

    position: relative;
}

.headline-box::before,
.headline-box::after {
    content: "";

    position: absolute;

    width: 30px;
    height: 2px;

    background: #00d9ff;

    top: 0;
}

.headline-box::before {
    left: 0;
}

.headline-box::after {
    right: 0;
}

.headline-box h3 {
    font-size: clamp(22px, 2vw, 35px);

    line-height: 1.4;

    letter-spacing: 1px;
}

.headline-box span {
    color: #159cff;

    text-shadow:
        0 0 10px rgba(0, 150, 255, 0.5);
}


/* TECHNOLOGY */

.technology-box {
    display: flex;

    justify-content: center;

    gap: 20px;

    width: 100%;

    margin-top: 45px;

    padding: 18px;

    border: 1px solid rgba(0, 180, 255, 0.5);

    border-radius: 25px;

    background:
        rgba(0, 15, 30, 0.7);

    backdrop-filter: blur(10px);
}

.technology {
    display: flex;

    flex-direction: column;

    align-items: center;

    gap: 8px;

    min-width: 60px;

    transition: 0.3s;
}

.technology:hover {
    transform: translateY(-8px);

    color: #00cfff;
}

.technology b {
    font-size: 25px;
}

.technology small {
    font-size: 11px;

    color: #c4d8e8;
}


/* PRINCIPLES */

.principles {
    display: grid;

    grid-template-columns: repeat(4, 1fr);

    width: 100%;

    margin-top: 40px;

    gap: 15px;
}

.principles div {
    text-align: center;

    border-right: 1px solid rgba(255,255,255,0.15);
}

.principles div:last-child {
    border: none;
}

.principles strong {
    display: block;

    font-size: 25px;

    color: #00bfff;

    margin-bottom: 8px;
}

.principles span {
    font-size: 11px;

    color: #d7e5f2;

    line-height: 1.5;
}


/* =========================
   RIGHT
========================= */

.right-section {
    position: relative;

    min-height: 450px;
}

.world {
    position: absolute;

    right: 10px;
    top: -20px;

    font-size: 100px;

    opacity: 0.08;

    filter:
        drop-shadow(
            0 0 20px #008cff
        );
}


/* DASHBOARD */

.dashboard {
    position: absolute;

    top: 80px;
    right: 30px;

    width: 310px;
    height: 180px;

    padding: 20px;

    border: 1px solid rgba(0, 170, 255, 0.5);

    border-radius: 15px;

    background:
        linear-gradient(
            145deg,
            rgba(10, 30, 50, 0.95),
            rgba(0, 10, 20, 0.9)
        );

    box-shadow:
        0 0 30px rgba(0, 120, 255, 0.15);

    transform:
        perspective(600px)
        rotateY(-5deg);
}

.dashboard-title {
    font-size: 10px;

    color: #7dcfff;

    letter-spacing: 1px;
}


/* BAR CHART */

.bar-chart {
    position: absolute;

    bottom: 20px;
    left: 20px;

    height: 100px;

    display: flex;

    align-items: flex-end;

    gap: 8px;
}

.bar-chart span {
    width: 14px;

    background:
        linear-gradient(
            to top,
            #0077ff,
            #00d9ff
        );

    box-shadow:
        0 0 10px rgba(0, 170, 255, 0.4);

    animation:
        barAnimation 2s infinite alternate;
}

@keyframes barAnimation {

    from {
        transform: scaleY(0.8);
    }

    to {
        transform: scaleY(1.05);
    }

}


/* CIRCLE */

.chart-circle {
    position: absolute;

    right: 25px;
    bottom: 35px;

    width: 80px;
    height: 80px;

    border-radius: 50%;

    display: grid;
    place-items: center;

    background:
        conic-gradient(
            #00bfff 78%,
            #152535 78%
        );

    font-size: 14px;
}

.chart-circle::after {
    content: "";

    position: absolute;

    width: 60px;
    height: 60px;

    border-radius: 50%;

    background: #06111c;
}

.chart-circle span {
    position: relative;

    z-index: 2;

    color: white;
}


/* CODE WINDOW */

.code-window {
    position: absolute;

    top: 270px;
    right: 0;

    width: 330px;

    background: #06111b;

    border: 1px solid rgba(0, 180, 255, 0.4);

    border-radius: 12px;

    box-shadow:
        0 15px 40px rgba(0,0,0,0.5);

    transform:
        rotate(-4deg);
}

.window-header {
    display: flex;

    gap: 6px;

    padding: 10px;

    border-bottom:
        1px solid rgba(255,255,255,0.1);
}

.window-header span {
    width: 9px;
    height: 9px;

    border-radius: 50%;

    background: #555;
}

.code-window pre {
    padding: 15px;

    overflow: hidden;

    font-size: 11px;

    color: #63d9ff;

    line-height: 1.6;
}


/* FLOATING LABELS */

.floating-label {
    position: absolute;

    padding: 6px 14px;

    border: 1px solid #00bfff;

    border-radius: 7px;

    font-size: 10px;

    color: #00d9ff;

    background:
        rgba(0, 20, 35, 0.8);

    box-shadow:
        0 0 15px rgba(0,180,255,0.2);
}

.analyze {
    top: 250px;
    left: 10px;
}

.visualize {
    top: 140px;
    right: -10px;
}

.build {
    bottom: 20px;
    left: 70px;

    border-color: #a855f7;

    color: #c084fc;
}


/* =========================
   FOOTER
========================= */

footer {
    margin-top: 45px;

    display: grid;

    grid-template-columns:
        repeat(5, 1fr);

    border-top: 1px solid rgba(0,180,255,0.5);

    border-bottom: 1px solid rgba(0,180,255,0.5);

    padding: 20px 10px;

    gap: 15px;
}

footer div {
    display: flex;

    align-items: center;

    gap: 12px;

    color: #00bfff;

    border-right:
        1px solid rgba(255,255,255,0.15);

    padding-right: 15px;
}

footer div:last-child {
    border: none;
}

footer span {
    color: #d9e8f5;

    font-size: 11px;

    line-height: 1.5;
}


/* =========================
   RESPONSIVE
========================= */

@media(max-width: 1100px) {

    .hero {
        grid-template-columns: 1fr;
    }

    .right-section {
        min-height: 500px;
    }

    .top-skills {
        display: none;
    }

    footer {
        grid-template-columns: repeat(2, 1fr);
    }

}


@media(max-width: 600px) {

    .banner {
        padding: 20px;
    }

    .name h1 {
        font-size: 55px;
    }

    .name h2 {
        font-size: 42px;
    }

    .technology-box {
        flex-wrap: wrap;
    }

    .principles {
        grid-template-columns: repeat(2, 1fr);
    }

    footer {
        grid-template-columns: 1fr;
    }

    footer div {
        border-right: none;
    }

    .dashboard {
        right: 0;
    }

    .code-window {
        right: 0;
        width: 280px;
    }
}
	</style>
</head>

<body>

    <!-- Animated Background -->
    <canvas id="particles"></canvas>

    <main class="banner">

        <!-- Top Navigation -->
        <div class="top-line">
            <span class="hello">// Hello World! 👋</span>

            <div class="top-skills">
                <span>🐍 Python</span>
                <span>🗄️ SQL</span>
                <span>📊 Power BI</span>
                <span>🧠 AI / GenAI</span>
            </div>

            <span class="insight">INSIGHT</span>
        </div>


        <section class="hero">

            <!-- LEFT -->
            <div class="left-section">

                <div class="name">
                    <h1>PANAD</h1>
                    <h2>HARIKRUSHNA</h2>
                </div>

                <div class="role">
                    DATA ANALYST
                    <span>●</span>
                    PYTHON DEVELOPER
                    <span>●</span>
                    AI ENTHUSIAST
                </div>


                <div class="features">

                    <div class="feature">
                        <div class="feature-icon">🎯</div>
                        <span>Turning Data into Insights</span>
                    </div>

                    <div class="feature">
                        <div class="feature-icon">&lt;/&gt;</div>
                        <span>Building Solutions with Python</span>
                    </div>

                    <div class="feature">
                        <div class="feature-icon">🗄️</div>
                        <span>Query. Analyze. Visualize.</span>
                    </div>

                    <div class="feature">
                        <div class="feature-icon">🧠</div>
                        <span>Exploring AI & Building the Future</span>
                    </div>

                </div>


                <div class="quote">
                    <strong>“</strong>
                    <p>
                        Data is the new fuel,<br>
                        Insight is the new <span>power.</span>
                    </p>
                </div>

            </div>


            <!-- CENTER -->
            <div class="center-section">

                <div class="headline-box">

                    <h3>
                        I ANALYZE <span>DATA</span>,
                        <br>
                        BUILD <span>SOLUTIONS</span> &
                        <br>
                        CREATE <span>IMPACT</span>
                    </h3>

                </div>


                <div class="technology-box">

                    <div class="technology">
                        <b>🐼</b>
                        <small>Pandas</small>
                    </div>

                    <div class="technology">
                        <b>🔢</b>
                        <small>NumPy</small>
                    </div>

                    <div class="technology">
                        <b>📗</b>
                        <small>Excel</small>
                    </div>

                    <div class="technology">
                        <b>📈</b>
                        <small>Matplotlib</small>
                    </div>

                    <div class="technology">
                        <b>🔀</b>
                        <small>Git</small>
                    </div>

                    <div class="technology">
                        <b>🐙</b>
                        <small>GitHub</small>
                    </div>

                </div>


                <div class="principles">

                    <div>
                        <strong>&lt;/&gt;</strong>
                        <span>Clean Code<br>Best Practice</span>
                    </div>

                    <div>
                        <strong>📈</strong>
                        <span>Data Driven<br>Decision Making</span>
                    </div>

                    <div>
                        <strong>💡</strong>
                        <span>Problem Solver<br>Analytical Thinking</span>
                    </div>

                    <div>
                        <strong>🚀</strong>
                        <span>Always Learning<br>Always Growing</span>
                    </div>

                </div>

            </div>


            <!-- RIGHT -->
            <div class="right-section">

                <div class="world">
                    🌐
                </div>

                <div class="dashboard">

                    <div class="dashboard-title">
                        ANALYTICS DASHBOARD
                    </div>

                    <div class="bar-chart">

                        <span style="height:35%"></span>
                        <span style="height:55%"></span>
                        <span style="height:45%"></span>
                        <span style="height:75%"></span>
                        <span style="height:65%"></span>
                        <span style="height:90%"></span>
                        <span style="height:70%"></span>

                    </div>

                    <div class="chart-circle">
                        <span>78%</span>
                    </div>

                </div>


                <div class="code-window">

                    <div class="window-header">
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>

                    <pre><code id="code"></code></pre>

                </div>

                <div class="floating-label analyze">
                    ANALYZE
                </div>

                <div class="floating-label visualize">
                    VISUALIZE
                </div>

                <div class="floating-label build">
                    BUILD
                </div>

            </div>

        </section>


        <!-- Bottom Information -->
        <footer>

            <div>
                🎓
                <span>MCA Graduate</span>
            </div>

            <div>
                💼
                <span>Data Analyst &<br>Accounts Professional</span>
            </div>

            <div>
                🎯
                <span>Focused on Data, AI<br>& Automation</span>
            </div>

            <div>
                🏆
                <span>Building Practical Projects<br>that Solve Real Problems</span>
            </div>

            <div>
                ❤️
                <span>Passionate about<br>Learning & Growth</span>
            </div>

        </footer>

    </main>

    <script>
	/* =========================================
   PARTICLE BACKGROUND
========================================= */

const canvas = document.getElementById("particles");
const ctx = canvas.getContext("2d");

let particles = [];

function resizeCanvas() {

    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;

}

resizeCanvas();

window.addEventListener("resize", resizeCanvas);


class Particle {

    constructor() {

        this.x = Math.random() * canvas.width;
        this.y = Math.random() * canvas.height;

        this.size =
            Math.random() * 1.8 + 0.5;

        this.speedX =
            (Math.random() - 0.5) * 0.5;

        this.speedY =
            (Math.random() - 0.5) * 0.5;

        this.opacity =
            Math.random() * 0.6 + 0.2;
    }


    update() {

        this.x += this.speedX;
        this.y += this.speedY;

        if (this.x < 0)
            this.x = canvas.width;

        if (this.x > canvas.width)
            this.x = 0;

        if (this.y < 0)
            this.y = canvas.height;

        if (this.y > canvas.height)
            this.y = 0;

    }


    draw() {

        ctx.beginPath();

        ctx.arc(
            this.x,
            this.y,
            this.size,
            0,
            Math.PI * 2
        );

        ctx.fillStyle =
            `rgba(0,180,255,${this.opacity})`;

        ctx.fill();

    }

}


function createParticles() {

    particles = [];

    const count =
        Math.min(
            100,
            Math.floor(
                canvas.width / 15
            )
        );

    for (let i = 0; i < count; i++) {

        particles.push(
            new Particle()
        );

    }

}

createParticles();


function connectParticles() {

    for (let a = 0; a < particles.length; a++) {

        for (
            let b = a + 1;
            b < particles.length;
            b++
        ) {

            const dx =
                particles[a].x -
                particles[b].x;

            const dy =
                particles[a].y -
                particles[b].y;

            const distance =
                Math.sqrt(
                    dx * dx +
                    dy * dy
                );

            if (distance < 120) {

                const opacity =
                    1 -
                    distance / 120;

                ctx.strokeStyle =
                    `rgba(0,140,255,${opacity * 0.12})`;

                ctx.lineWidth = 1;

                ctx.beginPath();

                ctx.moveTo(
                    particles[a].x,
                    particles[a].y
                );

                ctx.lineTo(
                    particles[b].x,
                    particles[b].y
                );

                ctx.stroke();

            }

        }

    }

}


function animateParticles() {

    ctx.clearRect(
        0,
        0,
        canvas.width,
        canvas.height
    );

    particles.forEach(
        particle => {

            particle.update();
            particle.draw();

        }
    );

    connectParticles();

    requestAnimationFrame(
        animateParticles
    );

}

animateParticles();


/* =========================================
   CODE WINDOW TYPING EFFECT
========================================= */

const codeElement =
    document.getElementById("code");

const codeText = `import pandas as pd
import numpy as np

data = pd.read_csv("data.csv")

df = data.groupby(
    "category"
).agg({
    "sales": "sum"
})

df.plot(
    kind="bar"
)

print("Data analyzed successfully!")`;

let codeIndex = 0;


function typeCode() {

    if (codeIndex < codeText.length) {

        codeElement.textContent +=
            codeText.charAt(codeIndex);

        codeIndex++;

        setTimeout(
            typeCode,
            25
        );

    }

}

typeCode();


/* =========================================
   MOUSE PARALLAX EFFECT
========================================= */

const banner =
    document.querySelector(".banner");

document.addEventListener(
    "mousemove",
    (event) => {

        const x =
            (event.clientX /
                window.innerWidth -
                0.5);

        const y =
            (event.clientY /
                window.innerHeight -
                0.5);

        const dashboard =
            document.querySelector(
                ".dashboard"
            );

        const codeWindow =
            document.querySelector(
                ".code-window"
            );

        dashboard.style.transform =
            `perspective(600px)
             rotateY(${-5 + x * 5}deg)
             translate(${x * 5}px,
                       ${y * 5}px)`;

        codeWindow.style.transform =
            `rotate(-4deg)
             translate(${x * -8}px,
                       ${y * -8}px)`;

    }
);
	</script>

</body>
</html>
