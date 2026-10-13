# velixa-media
Official website for velixa media

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="theme-color" content="#f7f2eb">
  <meta name="description" content="Velixa Media creates thoughtful social media designs, advertisements and brand visuals.">
  <title>Velixa Media | Create. Elevate. Inspire.</title>

  <style>
    :root {
      --cream: #f7f2eb;
      --paper: #fffdf9;
      --brown: #392820;
      --taupe: #a18c7d;
      --muted: #776c64;
      --line: #e3d9cf;
      --serif: Georgia, "Times New Roman", serif;
    }

    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      background: var(--cream);
      color: var(--brown);
      font-family: Arial, Helvetica, sans-serif;
      line-height: 1.7;
    }
    a { color: inherit; text-decoration: none; }
    .wrap { width: min(1080px, 90%); margin: auto; }

    .announcement {
      background: var(--brown);
      color: var(--cream);
      text-align: center;
      padding: 9px;
      font-size: 10px;
      letter-spacing: 2px;
      text-transform: uppercase;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 10;
      background: rgba(247,242,235,.96);
      border-bottom: 1px solid var(--line);
    }
    nav {
      min-height: 78px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }
    .brand {
      display: flex;
      align-items: center;
      gap: 10px;
      font-size: 12px;
      font-weight: bold;
      letter-spacing: 2px;
    }
    .brand-mark {
      width: 39px;
      height: 39px;
      border: 1px solid var(--brown);
      border-radius: 50%;
      display: grid;
      place-items: center;
      font: 22px var(--serif);
    }
    .tagline {
      display: block;
      color: var(--muted);
      font-size: 8px;
      letter-spacing: 2px;
      font-weight: normal;
    }
    .links {
      display: flex;
      align-items: center;
      gap: 25px;
      font-size: 12px;
    }
    .links a:hover { color: var(--taupe); }
    .button {
      display: inline-block;
      padding: 12px 19px;
      background: var(--brown);
      color: var(--cream);
      border: 1px solid var(--brown);
      font-size: 11px;
      letter-spacing: 1px;
      text-transform: uppercase;
      transition: .2s;
    }
    .button:hover {
      background: transparent;
      color: var(--brown);
    }
    .menu {
      display: none;
      background: transparent;
      border: 1px solid var(--line);
      padding: 8px 12px;
      color: var(--brown);
      font-size: 20px;
    }

    .hero { padding: 85px 0; }
    .hero-grid {
      display: grid;
      grid-template-columns: 1.1fr .9fr;
      gap: 55px;
      align-items: center;
    }
    .eyebrow {
      font-size: 10px;
      letter-spacing: 2px;
      text-transform: uppercase;
      color: var(--taupe);
      font-weight: bold;
    }
    h1, h2, h3 { font-family: var(--serif); font-weight: normal; }
    h1 {
      font-size: clamp(48px, 6.5vw, 78px);
      line-height: 1.04;
      letter-spacing: -2px;
      margin: 20px 0;
    }
    h1 em { color: #765849; }
    .intro {
      color: var(--muted);
      max-width: 440px;
      font-size: 14px;
      margin-bottom: 28px;
    }
    .hero-actions {
      display: flex;
      align-items: center;
      flex-wrap: wrap;
      gap: 18px;
    }
    .text-link {
      font-size: 12px;
      border-bottom: 1px solid var(--taupe);
      padding-bottom: 3px;
    }
    .art {
      min-height: 400px;
      background: #e9ddd0;
      display: grid;
      place-items: center;
      position: relative;
      padding: 25px;
    }
    .art-card {
      width: 86%;
      min-height: 335px;
      background: var(--paper);
      padding: 20px;
      box-shadow: 0 18px 40px #39282012;
      transform: rotate(-3deg);
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }
    .art-top, .art-bottom {
      display: flex;
      justify-content: space-between;
      gap: 10px;
    }
    .art-top {
      font-size: 8px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      color: var(--muted);
    }
    .art-center {
      background: linear-gradient(140deg, #d2b9a4, #f0e4d7, #bca18d);
      min-height: 205px;
      display: grid;
      place-items: center;
      font: 70px var(--serif);
      color: var(--brown);
    }
    .art-bottom strong {
      font: 22px/1.2 var(--serif);
    }
    .art-bottom small {
      font-size: 9px;
      text-transform: uppercase;
      letter-spacing: 1px;
      color: var(--muted);
    }
    .floating {
      position: absolute;
      right: 0;
      bottom: 28px;
      background: var(--brown);
      color: var(--cream);
      padding: 12px 16px;
      font: 17px var(--serif);
    }

    .specialties {
      border-top: 1px solid var(--line);
      border-bottom: 1px solid var(--line);
      padding: 20px 0;
    }
    .specialties .wrap {
      display: flex;
      justify-content: space-between;
      gap: 15px;
      flex-wrap: wrap;
      color: var(--muted);
      font-size: 10px;
      text-transform: uppercase;
      letter-spacing: 1.4px;
    }

    section { padding: 80px 0; }
    .services { background: var(--paper); }
    .section-heading {
      display: flex;
      align-items: end;
      justify-content: space-between;
      gap: 25px;
      margin-bottom: 35px;
    }
    h2 {
      font-size: clamp(36px, 4.5vw, 52px);
      line-height: 1.15;
      margin: 10px 0 0;
      letter-spacing: -1px;
    }
    .section-desc {
      color: var(--muted);
      font-size: 13px;
      max-width: 350px;
    }
    .service-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 16px;
    }
    .service {
      border: 1px solid var(--line);
      padding: 25px;
      min-height: 230px;
      transition: .2s;
    }
    .service:hover {
      transform: translateY(-4px);
      box-shadow: 0 12px 35px #3928200c;
    }
    .number { color: var(--taupe); font: 17px var(--serif); }
    .service h3 { font-size: 25px; margin: 27px 0 8px; }
    .service p { color: var(--muted); font-size: 12px; }

    .portfolio-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 17px;
    }
    .project-art {
      aspect-ratio: 4 / 4.6;
      display: grid;
      place-items: center;
      padding: 20px;
      text-align: center;
    }
    .project-art.one { background: #d9c6b5; }
    .project-art.two { background: #b6aaa0; }
    .project-art.three { background: #eadbd0; }
    .project-inner {
      width: 90%;
      min-height: 75%;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 15px;
      border: 1px solid #654a3d70;
    }
    .project-inner span {
      font: clamp(22px, 3vw, 34px)/1.15 var(--serif);
      color: var(--brown);
    }
    .project-info { padding-top: 12px; }
    .project-info h3 { font-size: 21px; margin: 0; }
    .project-info p { color: var(--muted); font-size: 11px; margin: 3px 0; }
    .note { color: var(--muted); font-size: 11px; margin-top: 20px; }

    .process { background: #eee4d9; }
    .process-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 22px;
      margin-top: 38px;
    }
    .step {
      border-top: 1px solid #b8a596;
      padding-top: 15px;
    }
    .step span { color: var(--taupe); font: 18px var(--serif); }
    .step h3 { font-size: 21px; margin: 12px 0 6px; }
    .step p { color: var(--muted); font-size: 12px; }

    .about-grid {
      display: grid;
      grid-template-columns: .8fr 1.2fr;
      gap: 60px;
      align-items: center;
    }
    .about-art {
      min-height: 260px;
      background: #eee4d9;
      border: 1px solid var(--line);
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      padding: 30px;
    }
    .about-art strong { font: 65px var(--serif); }
    .about-art small {
      font-size: 10px;
      letter-spacing: 2px;
      color: var(--muted);
    }
    .about-copy p { color: var(--muted); font-size: 13px; }
    .about-copy .lead {
      color: var(--brown);
      font: 25px/1.4 var(--serif);
    }

    .contact { background: var(--brown); color: var(--cream); }
    .contact .eyebrow { color: #d5bdab; }
    .contact-grid {
      display: grid;
      grid-template-columns: 1.2fr .8fr;
      gap: 40px;
      align-items: end;
    }
    .contact h2 { font-size: clamp(42px, 6vw, 65px); }
    .contact p { color: #d6c8bd; font-size: 13px; max-width: 440px; }
    .contact .button {
      background: var(--cream);
      color: var(--brown);
      border-color: var(--cream);
    }
    .contact .button:hover {
      background: transparent;
      color: var(--cream);
    }
    .contact-actions { display: flex; flex-direction: column; align-items: start; gap: 15px; }
    .contact .text-link { color: var(--cream); border-color: #b49b89; }

    footer {
      background: var(--brown);
      border-top: 1px solid #ffffff30;
      color: #d6c8bd;
      padding: 22px 0;
      font-size: 10px;
    }
    .footer-inner {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 15px;
      flex-wrap: wrap;
    }
    .footer-links { display: flex; gap: 18px; }

    @media (max-width: 760px) {
      .menu { display: block; }
      .links {
        display: none;
        position: absolute;
        top: 78px;
        left: 0;
        right: 0;
        background: var(--cream);
        padding: 20px 5%;
        border-bottom: 1px solid var(--line);
        flex-direction: column;
        align-items: stretch;
      }
      .links.open { display: flex; }
      .hero { padding: 55px 0; }
      .hero-grid, .about-grid, .contact-grid { grid-template-columns: 1fr; gap: 30px; }
      .art { min-height: 350px; }
      .art-card { min-height: 300px; }
      section { padding: 60px 0; }
      .section-heading { display: block; }
      .section-desc { margin-top: 15px; }
      .service-grid { grid-template-columns: 1fr; }
      .service { min-height: auto; }
      .service h3 { margin-top: 15px; }
      .portfolio-grid { grid-template-columns: 1fr 1fr; gap: 20px 12px; }
      .portfolio-item:last-child { grid-column: 1 / -1; width: calc(50% - 6px); }
      .process-grid { grid-template-columns: 1fr 1fr; row-gap: 25px; }
    }
    @media (max-width: 430px) {
      h1 { font-size: 47px; }
      .portfolio-grid, .process-grid { grid-template-columns: 1fr; }
      .portfolio-item:last-child { grid-column: auto; width: 100%; }
      .project-art { aspect-ratio: 1 / 1; }
      .hero-actions { align-items: flex-start; flex-direction: column; }
      .footer-inner { align-items: flex-start; flex-direction: column; }
    }
  </style>
</head>

<body>
  <div class="announcement">Thoughtful visuals for brands with something to say</div>

  <header>
    <div class="wrap">
      <nav aria-label="Main navigation">
        <a class="brand" href="#home">
          <span class="brand-mark">V.</span>
          <span>VELIXA MEDIA
            <small class="tagline">CREATE · ELEVATE · INSPIRE</small>
          </span>
        </a>

        <button class="menu" id="menu" aria-label="Open menu" aria-expanded="false">☰</button>

        <div class="links" id="links">
          <a href="#services">Services</a>
          <a href="#portfolio">Portfolio</a>
          <a href="#about">About</a>
          <a class="button" href="#contact">Let's talk ↗</a>
        </div>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="wrap hero-grid">
        <div>
          <div class="eyebrow">Creative studio · Digital presence</div>
          <h1>Make your brand feel <em>unforgettable.</em></h1>
          <p class="intro">
            We create thoughtful social media designs and polished brand visuals
            that help small businesses show up with clarity, consistency, and confidence.
          </p>
          <div class="hero-actions">
            <a class="button" href="https://www.instagram.com/velixamedia/"
               target="_blank" rel="noopener noreferrer">Start a conversation ↗</a>
            <a class="text-link" href="#portfolio">Explore our work ↓</a>
          </div>
        </div>

        <div class="art" aria-label="Velixa Media sample artwork">
          <div class="art-card">
            <div class="art-top"><span>Velixa Studio</span><span>Visual concept 01</span></div>
            <div class="art-center">VM</div>
            <div class="art-bottom">
              <strong>Quietly bold.<br>Always considered.</strong>
              <small>Creative<br>with purpose</small>
            </div>
          </div>
          <div class="floating">Create. Elevate. Inspire.</div>
        </div>
      </div>
    </section>

    <div class="specialties">
      <div class="wrap">
        <span>Social media design</span>
        <span>✳</span>
        <span>Brand visuals</span>
        <span>✳</span>
        <span>Promotional creatives</span>
        <span>✳</span>
        <span>Content design</span>
      </div>
    </div>

    <section class="services" id="services">
      <div class="wrap">
        <div class="section-heading">
          <div>
            <div class="eyebrow">What we can create together</div>
            <h2>Creative that works<br>as hard as you do.</h2>
          </div>
          <p class="section-desc">
            From a single promotional post to a consistent visual identity,
            we help bring your ideas to life with a clear, cohesive look.
          </p>
        </div>

        <div class="service-grid">
          <article class="service">
            <span class="number">01 / Design</span>
            <h3>Social Media Designs</h3>
            <p>Feed posts, carousels, story creatives, and layouts designed to feel consistent with your brand.</p>
          </article>
          <article class="service">
            <span class="number">02 / Promotion</span>
            <h3>Ads & Promotions</h3>
            <p>Eye-catching graphics for launches, special offers, new arrivals, and important announcements.</p>
          </article>
          <article class="service">
            <span class="number">03 / Identity</span>
            <h3>Brand Visuals</h3>
            <p>Logo concepts, visual direction, and brand-style elements that help your business look put-together.</p>
          </article>
        </div>
      </div>
    </section>

    <section id="portfolio">
      <div class="wrap">
        <div class="section-heading">
          <div>
            <div class="eyebrow">A look at our style</div>
            <h2>Selected visual concepts.</h2>
          </div>
          <p class="section-desc">
            Sample layouts showing our approach to tone, spacing, and visual storytelling.
            Replace these concepts with your own designs as your portfolio grows.
          </p>
        </div>

        <div class="portfolio-grid">
          <article class="portfolio-item">
            <div class="project-art one">
              <div class="project-inner"><span>SOFT<br>FORM</span></div>
            </div>
            <div class="project-info">
              <h3>Soft Form</h3>
              <p>Product-led visual concept</p>
            </div>
          </article>

          <article class="portfolio-item">
            <div class="project-art two">
              <div class="project-inner"><span>LESS,<br>BUT BETTER.</span></div>
            </div>
            <div class="project-info">
              <h3>Less, But Better</h3>
              <p>Minimal campaign concept</p>
            </div>
          </article>

          <article class="portfolio-item">
            <div class="project-art three">
              <div class="project-inner"><span>Your brand<br>deserves to shine.</span></div>
            </div>
            <div class="project-info">
              <h3>Made to Stand Out</h3>
              <p>Small-business promotional concept</p>
            </div>
          </article>
        </div>

        <p class="note">
          These are sample concepts, not client case studies. Add your completed work here when ready.
        </p>
      </div>
    </section>

    <section class="process" id="process">
      <div class="wrap">
        <div class="eyebrow">Simple from start to finish</div>
        <h2>A clear process.<br>A considered result.</h2>

        <div class="process-grid">
          <article class="step">
            <span>01</span><h3>Tell us your idea</h3>
            <p>Share your goals, audience, references, and what you need designed.</p>
          </article>
          <article class="step">
            <span>02</span><h3>Plan the look</h3>
            <p>We align on the style, message, and creative direction.</p>
          </article>
          <article class="step">
            <span>03</span><h3>Design & refine</h3>
            <p>Your design is created and refined with the agreed revision.</p>
          </article>
          <article class="step">
            <span>04</span><h3>Ready to post</h3>
            <p>Receive your finished design and use it across your chosen channels.</p>
          </article>
        </div>
      </div>
    </section>

    <section id="about">
      <div class="wrap about-grid">
        <div class="about-art">
          <strong>V.</strong>
          <small>CREATE · ELEVATE · INSPIRE</small>
        </div>
        <div class="about-copy">
          <div class="eyebrow">A little about Velixa</div>
          <h2>Good design makes your message easier to feel.</h2>
          <p class="lead">Velixa Media is a creative space for thoughtful visuals, purposeful design, and growing brands.</p>
          <p>
            We believe a business doesn't need to be big to look considered.
            Our focus is helping small businesses present their products and ideas
            in a way that feels clear, cohesive, and true to them.
          </p>
          <a class="text-link" href="https://www.instagram.com/velixamedia/"
             target="_blank" rel="noopener noreferrer">Meet us on Instagram ↗</a>
        </div>
      </div>
    </section>

    <section class="contact" id="contact">
      <div class="wrap contact-grid">
        <div>
          <div class="eyebrow">Have a project in mind?</div>
          <h2>Let's make something meaningful.</h2>
          <p>
            Tell us about your business, the design you need, or the idea
            you've been thinking about. Let's start with a conversation.
          </p>
        </div>
        <div class="contact-actions">
          <a class="button" href="https://www.instagram.com/velixamedia/"
             target="_blank" rel="noopener noreferrer">DM @velixamedia ↗</a>
          <a class="text-link" href="https://www.instagram.com/velixamedia/"
             target="_blank" rel="noopener noreferrer">Instagram · @velixamedia</a>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="wrap footer-inner">
      <span>© <span id="year"></span> Velixa Media. Create · Elevate · Inspire.</span>
      <div class="footer-links">
        <a href="#services">Services</a>
        <a href="#portfolio">Portfolio</a>
        <a href="https://www.instagram.com/velixamedia/" target="_blank" rel="noopener noreferrer">Instagram ↗</a>
      </div>
    </div>
  </footer>

  <script>
    const menu = document.getElementById("menu");
    const links = document.getElementById("links");

    menu.addEventListener("click", function () {
      const open = links.classList.toggle("open");
      menu.setAttribute("aria-expanded", String(open));
      menu.setAttribute("aria-label", open ? "Close menu" : "Open menu");
      menu.textContent = open ? "×" : "☰";
    });

    links.querySelectorAll("a").forEach(function (link) {
      link.addEventListener("click", function () {
        links.classList.remove("open");
        menu.setAttribute("aria-expanded", "false");
        menu.setAttribute("aria-label", "Open menu");
        menu.textContent = "☰";
      });
    });

    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
