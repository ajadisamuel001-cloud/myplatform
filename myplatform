<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Ajadi Samuel | Portfolio</title>

    <style>
        :root {
            color-scheme: dark;
            --page: #07111f;
            --surface: #0c1a2c;
            --surface-raised: #10233a;
            --text: #f3f7fc;
            --muted: #a4b3c6;
            --accent: #52d6f5;
            --accent-soft: rgba(82, 214, 245, 0.1);
            --border: rgba(164, 179, 198, 0.14);
            --content-width: 1120px;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
            scroll-padding-top: 90px;
        }

        body {
            min-width: 320px;
            background:
                radial-gradient(ellipse at 75% 4%, rgba(19, 97, 137, 0.18), transparent 34rem),
                var(--page);
            color: var(--text);
            font-family: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
            line-height: 1.7;
        }

        header {
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 1px solid var(--border);
            background: rgba(7, 17, 31, 0.88);
            backdrop-filter: blur(16px);
        }

        .header-inner {
            width: min(100% - 48px, var(--content-width));
            min-height: 76px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 24px;
        }

        .logo {
            color: var(--text);
            font-size: 17px;
            font-weight: 750;
            letter-spacing: -0.03em;
            text-decoration: none;
            white-space: nowrap;
        }

        .logo span {
            color: var(--accent);
        }

        nav {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 8px 28px;
        }

        nav a {
            color: var(--muted);
            text-decoration: none;
            font-size: 14px;
            font-weight: 550;
            transition: color 0.2s ease;
        }

        nav a:hover,
        nav a:focus-visible {
            color: var(--accent);
        }

        a:focus-visible {
            outline: 2px solid var(--accent);
            outline-offset: 4px;
        }

        .skip-link {
            position: absolute;
            top: -100px;
            left: 24px;
            z-index: 101;
            padding: 10px 15px;
            border-radius: 8px;
            background: var(--text);
            color: var(--page);
        }

        .skip-link:focus {
            top: 10px;
        }

        .hero {
            width: min(100% - 48px, var(--content-width));
            min-height: min(720px, calc(100svh - 76px));
            margin: 0 auto;
            display: grid;
            grid-template-columns: minmax(0, 1.25fr) minmax(260px, 0.75fr);
            align-items: center;
            gap: clamp(40px, 8vw, 112px);
            padding: 88px 0;
        }

        .hero-text {
            max-width: 660px;
        }

        .hero-text .eyebrow {
            display: inline-flex;
            align-items: center;
            gap: 9px;
            margin-bottom: 22px;
            padding: 6px 12px;
            border: 1px solid rgba(82, 214, 245, 0.23);
            border-radius: 999px;
            background: var(--accent-soft);
            color: var(--accent);
            font-size: 13px;
            font-weight: 650;
            letter-spacing: 0.02em;
        }

        .hero-text .eyebrow::before {
            width: 7px;
            height: 7px;
            border-radius: 50%;
            background: var(--accent);
            content: "";
        }

        .hero-text h1 {
            max-width: 650px;
            font-size: clamp(46px, 7vw, 76px);
            line-height: 1.06;
            letter-spacing: -0.065em;
        }

        .hero-text h2 {
            margin-top: 16px;
            color: var(--accent);
            font-size: clamp(20px, 3vw, 27px);
            font-weight: 550;
            letter-spacing: -0.025em;
        }

        .hero-text p {
            max-width: 570px;
            margin: 22px 0 0;
            color: var(--muted);
            font-size: 17px;
        }

        .btn {
            display: inline-flex;
            min-height: 48px;
            align-items: center;
            justify-content: center;
            gap: 9px;
            margin-top: 28px;
            padding: 11px 20px;
            border: 1px solid transparent;
            border-radius: 10px;
            background: var(--accent);
            color: var(--page);
            text-decoration: none;
            font-size: 14px;
            font-weight: 750;
            transition: transform 0.2s ease, background 0.2s ease, border-color 0.2s ease;
        }

        .btn:hover {
            transform: translateY(-2px);
            background: #8ae8fb;
        }

        .profile {
            position: relative;
            width: min(100%, 340px);
            aspect-ratio: 1;
            justify-self: center;
            display: flex;
            justify-content: center;
            align-items: center;
            border: 1px solid rgba(82, 214, 245, 0.28);
            border-radius: 32px;
            background:
                radial-gradient(circle at 50% 35%, rgba(82, 214, 245, 0.2), transparent 56%),
                linear-gradient(145deg, #122b44, #0b1a2c 72%);
            color: var(--text);
            font-size: clamp(76px, 10vw, 112px);
            font-weight: 800;
            letter-spacing: -0.09em;
            box-shadow: 0 30px 90px rgba(0, 0, 0, 0.25), 0 0 70px rgba(20, 128, 164, 0.13);
        }

        .profile::after {
            position: absolute;
            right: -15px;
            bottom: 28px;
            width: 16px;
            height: 16px;
            border: 4px solid var(--page);
            border-radius: 50%;
            background: var(--accent);
            content: "";
        }

        section {
            padding: 104px max(24px, calc((100% - var(--content-width)) / 2));
        }

        .about,
        .contact {
            border-top: 1px solid var(--border);
            border-bottom: 1px solid var(--border);
            background: rgba(12, 26, 44, 0.72);
        }

        .section-title {
            margin-bottom: 14px;
            font-size: clamp(30px, 4vw, 42px);
            line-height: 1.2;
            letter-spacing: -0.045em;
        }

        .section-title span {
            color: var(--accent);
        }

        .section-intro {
            max-width: 620px;
            margin: 0 0 36px;
            color: var(--muted);
        }

        .about p {
            max-width: 760px;
            color: var(--muted);
            font-size: 17px;
        }

        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(min(100%, 230px), 1fr));
            gap: 18px;
        }

        .card {
            min-height: 170px;
            padding: 25px;
            border: 1px solid var(--border);
            border-radius: 14px;
            background: linear-gradient(150deg, rgba(16, 35, 58, 0.9), rgba(11, 26, 44, 0.9));
            transition: transform 0.2s ease, border-color 0.2s ease, background 0.2s ease;
        }

        .card:hover {
            transform: translateY(-4px);
            border-color: rgba(82, 214, 245, 0.42);
            background: linear-gradient(150deg, rgba(18, 45, 70, 0.96), rgba(11, 26, 44, 0.96));
        }

        .card h3 {
            margin-bottom: 9px;
            color: var(--text);
            font-size: 17px;
            letter-spacing: -0.02em;
        }

        .card p {
            color: var(--muted);
            font-size: 14px;
        }

        .contact {
            text-align: center;
        }

        .contact p {
            margin: 10px 0;
            color: var(--muted);
        }

        .contact a {
            color: var(--accent);
            text-decoration: none;
        }

        .contact a.btn {
            color: var(--page);
        }

        .contact a.btn:hover {
            color: var(--page);
        }

        footer {
            text-align: center;
            padding: 28px 24px;
            color: var(--muted);
            font-size: 13px;
        }

        @media (max-width: 700px) {
            .header-inner {
                width: min(100% - 32px, var(--content-width));
                min-height: 68px;
                flex-direction: column;
                gap: 10px;
                padding: 14px 0;
            }

            nav {
                gap: 5px 20px;
            }

            nav a {
                display: inline-flex;
                min-height: 40px;
                align-items: center;
                font-size: 13px;
            }

            .hero {
                width: min(100% - 40px, var(--content-width));
                min-height: auto;
                grid-template-columns: 1fr;
                gap: 42px;
                padding: 72px 0 84px;
            }

            .hero-text {
                text-align: center;
            }

            .hero-text p {
                margin-right: auto;
                margin-left: auto;
            }

            .profile {
                width: min(68vw, 260px);
                grid-row: 1;
                border-radius: 25px;
                font-size: 82px;
            }

            section {
                padding: 76px 20px;
            }
        }

        @media (max-width: 480px) {
            .hero {
                width: min(100% - 32px, var(--content-width));
                gap: 34px;
                padding: 56px 0 68px;
            }

            .hero-text h1 {
                font-size: clamp(38px, 10.5vw, 46px);
            }

            .hero-text h2 {
                font-size: 21px;
            }

            .hero-text p {
                font-size: 15px;
            }

            .profile {
                width: min(62vw, 220px);
                font-size: 70px;
            }

            section {
                padding: 64px 16px;
            }

            .card {
                min-height: auto;
                padding: 22px;
            }
        }

        @media (max-width: 380px) {
            nav {
                gap: 5px 13px;
            }
        }

        @media (prefers-reduced-motion: reduce) {
            html {
                scroll-behavior: auto;
            }

            *,
            *::before,
            *::after {
                transition-duration: 0.01ms !important;
                animation-duration: 0.01ms !important;
                animation-iteration-count: 1 !important;
            }
        }
    

        /* AJADISAMUEL SIGNATURE INTRO */
        .intro-screen {
            position: fixed;
            inset: 0;
            z-index: 9999;
            display: grid;
            place-items: center;
            overflow: hidden;
            background: #020409;
            opacity: 1;
            visibility: visible;
            transition: opacity .9s ease, visibility .9s ease;
        }
        .intro-screen.hide {
            opacity: 0;
            visibility: hidden;
            pointer-events: none;
        }
        .intro-glow {
            position: absolute;
            width: min(65vw, 440px);
            aspect-ratio: 1;
            border-radius: 50%;
            background: #006eff;
            filter: blur(130px);
            opacity: .25;
            animation: introGlow 3s ease-in-out infinite alternate;
        }
        .intro-content {
            position: relative;
            z-index: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            padding: 24px;
        }
        .intro-logo-wrap {
            width: clamp(170px, 28vw, 250px);
            aspect-ratio: 1;
            opacity: 0;
            transform: scale(.45) rotate(-12deg);
            animation: introLogoReveal 1.5s cubic-bezier(.2,.8,.2,1) .15s forwards;
        }
        .intro-logo {
            display: block;
            width: 100%;
            height: 100%;
            object-fit: contain;
            filter: drop-shadow(0 0 18px rgba(0,112,255,.55));
        }
        .intro-brand {
            margin-top: 14px;
            color: #f5f8ff;
            font-size: clamp(17px, 3vw, 25px);
            font-weight: 800;
            letter-spacing: .34em;
            padding-left: .34em;
            opacity: 0;
            transform: translateY(16px);
            animation: introTextReveal .8s ease 1.05s forwards;
        }
        .intro-caption {
            margin-top: 9px;
            color: #65aaff;
            font-size: 10px;
            letter-spacing: .42em;
            padding-left: .42em;
            opacity: 0;
            animation: introTextReveal .8s ease 1.35s forwards;
        }
        .intro-loading {
            width: 170px;
            height: 2px;
            margin-top: 30px;
            overflow: hidden;
            background: rgba(112,166,230,.2);
        }
        .intro-loading span {
            display: block;
            width: 0;
            height: 100%;
            background: #1685ff;
            box-shadow: 0 0 12px #1685ff;
            animation: introLoad 2.7s ease 0s forwards;
        }
        .skip-intro {
            position: absolute;
            right: 28px;
            bottom: 26px;
            z-index: 2;
            padding: 10px 15px;
            border: 1px solid rgba(101,170,255,.4);
            border-radius: 6px;
            background: transparent;
            color: #a8ceff;
            font: inherit;
            font-size: 11px;
            letter-spacing: .14em;
            cursor: pointer;
            transition: background .2s ease, color .2s ease;
        }
        .skip-intro:hover {
            background: #0875ed;
            color: white;
        }
        @keyframes introLogoReveal {
            0% { opacity: 0; transform: scale(.45) rotate(-12deg); filter: brightness(3) blur(12px); }
            65% { opacity: 1; filter: brightness(1.8) blur(0); }
            100% { opacity: 1; transform: scale(1) rotate(0); filter: brightness(1) blur(0); }
        }
        @keyframes introTextReveal {
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes introLoad { to { width: 100%; } }
        @keyframes introGlow {
            from { transform: scale(.8); opacity: .15; }
            to { transform: scale(1.25); opacity: .35; }
        }
        @media (max-width: 600px) {
            .skip-intro { right: 15px; bottom: 16px; }
        }
        @media (prefers-reduced-motion: reduce) {
            .intro-logo-wrap, .intro-brand, .intro-caption, .intro-loading span, .intro-glow {
                animation-duration: .01ms !important;
                animation-delay: 0ms !important;
            }
        }

    
/* CINEMATIC INTRO — independent overlay; portfolio content is unchanged */
#titanIntro {
  position: fixed; inset: 0; z-index: 99999; overflow: hidden;
  display: grid; place-items: center; isolation: isolate;
  background:
    radial-gradient(ellipse at 50% 44%, rgba(14,76,124,.32), transparent 34%),
    radial-gradient(ellipse at 50% 110%, rgba(0,190,255,.12), transparent 48%),
    #020711;
  color: #f4fbff;
  transition: opacity .85s ease, visibility .85s ease;
}
#titanIntro::before {
  content:""; position:absolute; inset:-30%;
  background: repeating-linear-gradient(115deg, transparent 0 80px, rgba(126,207,255,.025) 81px 82px);
  transform: rotate(-12deg); animation: introGridDrift 16s linear infinite;
}
#titanIntro::after {
  content:""; position:absolute; width:min(76vw,680px); aspect-ratio:1;
  border:1px solid rgba(92,190,255,.11); border-radius:50%;
  box-shadow:0 0 100px rgba(0,130,255,.08), inset 0 0 90px rgba(0,130,255,.05);
  animation: haloBreathe 4s ease-in-out infinite;
}
#titanIntro.is-done { opacity:0; visibility:hidden; pointer-events:none; }
.intro-content { position:relative; z-index:2; width:min(90vw,620px); display:flex; flex-direction:column; align-items:center; text-align:center; }
.intro-emblem { position:relative; width:clamp(190px,31vw,270px); aspect-ratio:1; display:grid; place-items:center; perspective:1000px; }
.intro-orbit { position:absolute; inset:-17px; border:1px solid rgba(92,196,255,.35); border-radius:50%; transform:rotateX(68deg) rotateZ(-18deg); box-shadow:0 0 24px rgba(0,160,255,.15); animation: orbitSpin 7s linear infinite; }
.intro-orbit::before,.intro-orbit::after { content:""; position:absolute; width:7px;height:7px;border-radius:50%; background:#9beaff; box-shadow:0 0 14px 4px #168bff; }
.intro-orbit::before { top:9%;left:19%; } .intro-orbit::after { right:11%;bottom:19%; }
.intro-orbit.two { inset:-31px; opacity:.42; transform:rotateX(72deg) rotateZ(52deg); animation:orbitSpinReverse 11s linear infinite; }
.intro-logo-wrap { width:100%; height:100%; display:grid; place-items:center; border-radius:50%; background:radial-gradient(circle,rgba(9,35,66,.8),rgba(2,9,20,.28) 68%,transparent 70%); filter:drop-shadow(0 0 22px rgba(0,153,255,.25)); opacity:0; transform:rotateY(76deg) scale(.62); animation: logoArrive 1.45s cubic-bezier(.16,.84,.24,1) .35s forwards; }
.intro-logo-wrap img { width:84%; height:84%; object-fit:contain; border-radius:50%; }
.intro-logo-wrap.logo-fallback { opacity:1; transform:none; }
.intro-logo-wrap.logo-fallback::before { content:"A"; display:grid; place-items:center; width:84%;height:84%; border:3px solid #79dfff;border-radius:50%;font-size:130px;font-weight:300;color:#d8f5ff; }
.intro-glint { position:absolute; z-index:3; top:8%; bottom:8%; left:-40%; width:34%; transform:skewX(-18deg); background:linear-gradient(90deg,transparent,rgba(255,255,255,.82),rgba(96,204,255,.45),transparent); filter:blur(5px); mix-blend-mode:screen; animation: glintPass 1.15s ease-in-out 1.8s forwards; }
.intro-name { margin-top:35px; font:700 clamp(20px,4vw,30px)/1.2 system-ui,sans-serif; letter-spacing:.27em; padding-left:.27em; opacity:0; transform:translateY(13px); animation: textArrive .8s ease 1.65s forwards; }
.intro-role { margin-top:11px; color:#8db6d2; font:500 10px/1.4 system-ui,sans-serif; letter-spacing:.42em; padding-left:.42em; opacity:0; animation: textArrive .8s ease 2s forwards; }
.intro-rule { width:0; height:1px; margin-top:25px; background:linear-gradient(90deg,transparent,#58caff,transparent); animation: ruleGrow .8s ease 2.25s forwards; }
.intro-loading { display:flex; align-items:center; gap:12px; width:min(230px,60vw); margin-top:20px; opacity:0; animation:textArrive .5s ease 2.3s forwards; }
.intro-loading-track { height:2px; flex:1; background:rgba(130,190,220,.18); overflow:hidden; }
.intro-loading-fill { width:0;height:100%; background:#69d9ff; box-shadow:0 0 10px #31aaff; animation:loadFill 2.6s ease 2.5s forwards; }
.intro-loading-label { color:#719bb9; font:9px system-ui,sans-serif; letter-spacing:.18em; }
.intro-corner { position:absolute; z-index:2; color:rgba(137,198,232,.42); font:9px system-ui,sans-serif; letter-spacing:.2em; }
.intro-corner.left { left:30px;bottom:27px; } .intro-corner.right { right:30px;bottom:27px; }
@keyframes logoArrive { 0%{opacity:0;transform:rotateY(76deg) rotateZ(-12deg) scale(.62);filter:brightness(2.2) drop-shadow(0 0 0 transparent)} 65%{opacity:1;transform:rotateY(-9deg) rotateZ(2deg) scale(1.04);filter:brightness(1.5) drop-shadow(0 0 38px rgba(0,153,255,.65))} 100%{opacity:1;transform:rotateY(0) rotateZ(0) scale(1);filter:brightness(1) drop-shadow(0 0 22px rgba(0,153,255,.3)} }
@keyframes glintPass { to { left:120%; } }
@keyframes textArrive { to { opacity:1;transform:translateY(0); } }
@keyframes ruleGrow { to { width:190px; } }
@keyframes loadFill { to { width:100%; } }
@keyframes orbitSpin { to { transform:rotateX(68deg) rotateZ(342deg); } }
@keyframes orbitSpinReverse { to { transform:rotateX(72deg) rotateZ(-308deg); } }
@keyframes haloBreathe { 50% { transform:scale(1.07); opacity:.55; } }
@keyframes introGridDrift { to { transform:translate3d(3%,2%,0) rotate(-12deg); } }
@media (prefers-reduced-motion:reduce) {
 #titanIntro *,#titanIntro::before,#titanIntro::after { animation-duration:.01ms!important; animation-delay:0ms!important; }
}

</style>
</head>

<body>

<div id="titanIntro" aria-label="Ajadisamuel introduction">
  <div class="intro-content">
    <div class="intro-emblem">
      <div class="intro-orbit"></div><div class="intro-orbit two"></div>
      <div class="intro-logo-wrap" id="introLogo">
        <img src="a_dark_minimal_high_contrast_graphic_logo_style.png" alt="Ajadisamuel logo" id="introLogoImage">
      </div>
      <div class="intro-glint"></div>
    </div>
    <div class="intro-name">AJADISAMUEL</div>
    <div class="intro-role">CREATIVE DEVELOPER</div>
    <div class="intro-rule"></div>
    <div class="intro-loading"><div class="intro-loading-track"><div class="intro-loading-fill"></div></div><span class="intro-loading-label">INITIALIZING</span></div>
  </div>
  <span class="intro-corner left">PORTFOLIO / 2026</span>
  <span class="intro-corner right">DESIGN • CODE • CREATE</span>
</div>
<script>
(() => {
  const intro = document.getElementById('titanIntro');
  const image = document.getElementById('introLogoImage');
  const logo = document.getElementById('introLogo');
  if (image) image.addEventListener('error', () => {
    image.remove();
    logo.classList.add('logo-fallback');
  }, { once:true });
  const finish = () => {
    intro.classList.add('is-done');
    setTimeout(() => intro.remove(), 900);
  };
  window.addEventListener('load', () => setTimeout(finish, 5600), { once:true });
  setTimeout(finish, 7200);
})();
</script>


    <!-- AJADISAMUEL SIGNATURE OPENING ANIMATION -->
    <div class="intro-screen" id="introScreen" aria-label="Ajadisamuel brand intro">
        <div class="intro-glow" aria-hidden="true"></div>
        <div class="intro-content">
            <div class="intro-logo-wrap">
                <img class="intro-logo" src="a_dark_minimal_high_contrast_graphic_logo_style.png" alt="Ajadisamuel A logo">
            </div>
            <div class="intro-brand">AJADISAMUEL</div>
            <div class="intro-caption">CREATIVE DEVELOPER</div>
            <div class="intro-loading" aria-hidden="true"><span></span></div>
        </div>
        <button class="skip-intro" type="button" id="skipIntro">SKIP INTRO →</button>
    </div>


    <a class="skip-link" href="#main-content">Skip to main content</a>

    <!-- NAVIGATION -->
    <header>
        <div class="header-inner">
            <a class="logo" href="#home" aria-label="Ajadi Samuel, home">Ajadi <span>Samuel</span></a>

            <nav aria-label="Main navigation">
                <a href="#home">Home</a>
                <a href="#about">About</a>
                <a href="#skills">Skills</a>
                <a href="#projects">Projects</a>
                <a href="#contact">Contact</a>
            </nav>
        </div>
    </header>

    <main id="main-content">
        <!-- HOME SECTION -->
        <section class="hero" id="home" aria-labelledby="home-title">

            <div class="hero-text">
                <p class="eyebrow">Student at SQI College of ICT</p>

                <h1 id="home-title">I'm Ajadi Samuel</h1>

                <h2>Aspiring Web Developer</h2>

                <p>
                    I'm learning web development and building my skills one project at a time.
                    I enjoy exploring new technologies and creating things that solve problems.
                </p>

                <a href="#projects" class="btn">Explore my projects <span aria-hidden="true">→</span></a>
            </div>

            <div class="profile" role="img" aria-label="Ajadi Samuel initials: AS">
                AS
            </div>

        </section>


        <!-- ABOUT SECTION -->
        <section class="about" id="about" aria-labelledby="about-title">

            <h2 class="section-title" id="about-title">A little <span>about me</span></h2>

            <p>
                I'm Ajadi Samuel, an aspiring programmer with a passion for technology and innovation.
                I'm currently learning HTML and CSS at SQI College of ICT, with the goal of becoming
                a software developer and building useful digital products.
            </p>

        </section>


        <!-- SKILLS SECTION -->
        <section id="skills" aria-labelledby="skills-title">

            <h2 class="section-title" id="skills-title">Skills I'm <span>building</span></h2>
            <p class="section-intro">The tools and strengths I'm developing as I grow as a programmer.</p>

            <div class="cards">

                <div class="card">
                    <h3>HTML</h3>
                    <p>Building clear, well-structured web pages.</p>
                </div>

                <div class="card">
                    <h3>CSS</h3>
                    <p>Creating responsive layouts and thoughtful visual styles.</p>
                </div>

                <div class="card">
                    <h3>Problem Solving</h3>
                    <p>Breaking down challenges and exploring practical solutions.</p>
                </div>

                <div class="card">
                    <h3>Technology</h3>
                    <p>Staying curious about technology and digital products.</p>
                </div>

            </div>

        </section>


        <!-- PROJECTS SECTION -->
        <section class="about" id="projects" aria-labelledby="projects-title">

            <h2 class="section-title" id="projects-title">Selected <span>projects</span></h2>
            <p class="section-intro">A few steps in my learning journey, with more projects to come.</p>

            <div class="cards">

                <div class="card">
                    <h3>Personal Portfolio</h3>
                    <p>This portfolio: a responsive introduction to my interests and learning journey.</p>
                </div>

                <div class="card">
                    <h3>Registration Page</h3>
                    <p>A beginner HTML project featuring a registration form.</p>
                </div>

                <div class="card">
                    <h3>Future Projects</h3>
                    <p>More creative websites and applications coming soon.</p>
                </div>

            </div>

        </section>


        <!-- GOALS SECTION -->
        <section aria-labelledby="goals-title">

            <h2 class="section-title" id="goals-title">Where I'm <span>headed</span></h2>
            <p class="section-intro">Areas I'd like to explore as I continue learning and building.</p>

            <div class="cards">

                <div class="card">
                    <h3>Web Development</h3>
                    <p>Become a professional frontend and backend developer.</p>
                </div>

                <div class="card">
                    <h3>Game Development</h3>
                    <p>Learn how to design and develop exciting games.</p>
                </div>

                <div class="card">
                    <h3>Ethical Hacking</h3>
                    <p>Understand cybersecurity and learn ethical hacking.</p>
                </div>

            </div>

        </section>


        <!-- CONTACT SECTION -->
        <section class="contact" id="contact" aria-labelledby="contact-title">

            <h2 class="section-title" id="contact-title">Let's <span>connect</span></h2>

            <p>Have a question or want to say hello? I'd be glad to hear from you.</p>

            <p><strong>Phone:</strong> <a href="tel:+2349169758534">09169758534</a></p>

            <p>
                <strong>WhatsApp:</strong>
                <a href="https://wa.me/2349169758534" target="_blank" rel="noopener noreferrer">
                    Chat with me
                </a>
            </p>

            <p><strong>Location:</strong> Nigeria</p>

            <a href="https://wa.me/2349169758534" class="btn" target="_blank" rel="noopener noreferrer">
                Let's Talk
            </a>

        </section>
    </main>


    <!-- FOOTER -->
    <footer>
        <p>© 2026 Ajadi Samuel. All Rights Reserved.</p>
        <p>Designed with passion and creativity.</p>
    </footer>



    <script>
        (() => {
            const intro = document.getElementById('introScreen');
            const skipButton = document.getElementById('skipIntro');
            let finished = false;

            function closeIntro() {
                if (finished || !intro) return;
                finished = true;
                intro.classList.add('hide');
                window.setTimeout(() => intro.remove(), 950);
            }

            skipButton?.addEventListener('click', closeIntro);
            window.setTimeout(closeIntro, 4200);
        })();
    </script>

</body>
</html>
