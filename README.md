<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta
    name="description"
    content="A Spider-Man-inspired Teacher's Day letter for Sir Randy Bello."
  >
  <title>Teacher's Day Letter for Sir Randy Bello</title>

  <style>
    :root {
      color-scheme: dark;

      --background: #08090d;
      --background-secondary: #12141a;
      --surface: rgba(20, 22, 29, 0.9);
      --paper: #171a21;
      --paper-secondary: #20242d;
      --text: #f7f7f9;
      --muted: #b8bdc8;
      --accent: #e50924;
      --accent-bright: #ff2947;
      --accent-dark: #8c0015;
      --border: rgba(255, 255, 255, 0.12);
      --shadow: rgba(0, 0, 0, 0.55);
      --web: rgba(255, 255, 255, 0.07);
      --button-text: #ffffff;
    }

    body.light-mode {
      color-scheme: light;

      --background: #f5f6f8;
      --background-secondary: #e5e8ed;
      --surface: rgba(255, 255, 255, 0.92);
      --paper: #fffdf8;
      --paper-secondary: #f0f1f4;
      --text: #17181c;
      --muted: #565b66;
      --accent: #c90020;
      --accent-bright: #ec1737;
      --accent-dark: #760012;
      --border: rgba(10, 12, 18, 0.14);
      --shadow: rgba(22, 25, 33, 0.2);
      --web: rgba(15, 17, 23, 0.07);
      --button-text: #ffffff;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      min-height: 100vh;
      overflow-x: hidden;
      font-family:
        Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont,
        "Segoe UI", sans-serif;
      color: var(--text);
      background:
        radial-gradient(circle at 15% 15%, rgba(229, 9, 36, 0.22), transparent 28rem),
        radial-gradient(circle at 85% 80%, rgba(229, 9, 36, 0.14), transparent 24rem),
        linear-gradient(135deg, var(--background), var(--background-secondary));
      transition:
        color 0.5s ease,
        background 0.5s ease;
    }

    body::before,
    body::after {
      position: fixed;
      z-index: -2;
      width: 24rem;
      height: 24rem;
      border: 1px solid var(--web);
      border-radius: 50%;
      content: "";
      opacity: 0.85;
      transition: border-color 0.5s ease;
    }

    body::before {
      top: -12rem;
      left: -12rem;
      box-shadow:
        0 0 0 3rem var(--web),
        0 0 0 7rem var(--web),
        0 0 0 11rem var(--web),
        0 0 0 15rem var(--web);
    }

    body::after {
      right: -12rem;
      bottom: -12rem;
      box-shadow:
        0 0 0 3rem var(--web),
        0 0 0 7rem var(--web),
        0 0 0 11rem var(--web),
        0 0 0 15rem var(--web);
    }

    button {
      font: inherit;
    }

    .web-lines {
      position: fixed;
      z-index: -1;
      inset: 0;
      overflow: hidden;
      pointer-events: none;
    }

    .web-lines span {
      position: absolute;
      top: 50%;
      left: 50%;
      width: 160vmax;
      height: 1px;
      background: linear-gradient(
        90deg,
        transparent,
        var(--web),
        transparent
      );
      transform-origin: center;
      transition: background 0.5s ease;
    }

    .web-lines span:nth-child(1) {
      transform: translate(-50%, -50%) rotate(15deg);
    }

    .web-lines span:nth-child(2) {
      transform: translate(-50%, -50%) rotate(45deg);
    }

    .web-lines span:nth-child(3) {
      transform: translate(-50%, -50%) rotate(75deg);
    }

    .web-lines span:nth-child(4) {
      transform: translate(-50%, -50%) rotate(105deg);
    }

    .web-lines span:nth-child(5) {
      transform: translate(-50%, -50%) rotate(135deg);
    }

    .web-lines span:nth-child(6) {
      transform: translate(-50%, -50%) rotate(165deg);
    }

    .page-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      width: min(1100px, calc(100% - 2rem));
      margin-inline: auto;
      padding-top: 1.25rem;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 0.75rem;
      font-weight: 800;
      letter-spacing: 0.04em;
    }

    .brand-mark {
      display: grid;
      width: 2.6rem;
      height: 2.6rem;
      place-items: center;
      color: #ffffff;
      background: linear-gradient(135deg, var(--accent-bright), var(--accent-dark));
      border: 1px solid rgba(255, 255, 255, 0.24);
      border-radius: 50%;
      box-shadow: 0 0 1.5rem rgba(229, 9, 36, 0.32);
    }

    .brand-mark svg {
      width: 1.45rem;
      height: 1.45rem;
      fill: currentColor;
    }

    .theme-toggle {
      display: flex;
      position: relative;
      align-items: center;
      gap: 0.55rem;
      min-width: 7.6rem;
      padding: 0.55rem 0.75rem;
      color: var(--text);
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 999px;
      box-shadow: 0 0.75rem 2rem var(--shadow);
      cursor: pointer;
      transition:
        color 0.35s ease,
        background 0.35s ease,
        border-color 0.35s ease,
        transform 0.25s ease;
    }

    .theme-toggle:hover {
      transform: translateY(-2px);
    }

    .toggle-track {
      display: flex;
      position: relative;
      align-items: center;
      justify-content: space-between;
      width: 2.85rem;
      height: 1.55rem;
      padding-inline: 0.25rem;
      color: rgba(255, 255, 255, 0.9);
      background: #0a0b0f;
      border: 1px solid var(--border);
      border-radius: 999px;
    }

    .toggle-track::after {
      position: absolute;
      top: 0.16rem;
      left: 0.18rem;
      width: 1.08rem;
      height: 1.08rem;
      background: var(--accent);
      border-radius: 50%;
      box-shadow: 0 0 0.75rem rgba(229, 9, 36, 0.65);
      content: "";
      transition:
        left 0.35s cubic-bezier(0.34, 1.56, 0.64, 1),
        background 0.35s ease;
    }

    .light-mode .toggle-track::after {
      left: 1.42rem;
    }

    .toggle-track span {
      z-index: 1;
      font-size: 0.7rem;
    }

    .toggle-label {
      font-size: 0.82rem;
      font-weight: 700;
    }

    main {
      display: grid;
      min-height: calc(100vh - 5rem);
      padding: 2rem 1rem 4rem;
      place-items: center;
    }

    .hero {
      width: min(960px, 100%);
      text-align: center;
    }

    .eyebrow {
      margin-bottom: 0.85rem;
      color: var(--accent-bright);
      font-size: clamp(0.72rem, 2vw, 0.9rem);
      font-weight: 800;
      letter-spacing: 0.22em;
      text-transform: uppercase;
    }

    h1 {
      max-width: 850px;
      margin-inline: auto;
      font-size: clamp(2rem, 7vw, 5rem);
      line-height: 0.98;
      letter-spacing: -0.055em;
    }

    h1 span {
      display: block;
      color: var(--accent-bright);
      text-shadow: 0 0 2rem rgba(229, 9, 36, 0.3);
    }

    .intro {
      max-width: 630px;
      margin: 1.25rem auto 2rem;
      color: var(--muted);
      font-size: clamp(0.95rem, 2.5vw, 1.12rem);
      line-height: 1.75;
    }

    .letter-stage {
      position: relative;
      width: min(760px, 100%);
      min-height: 490px;
      margin-inline: auto;
      perspective: 1800px;
    }

    .envelope {
      position: absolute;
      z-index: 4;
      top: 50%;
      left: 50%;
      width: min(560px, 92vw);
      height: min(340px, 55vw);
      min-height: 270px;
      overflow: hidden;
      background: linear-gradient(145deg, #13151b, #08090d);
      border: 1px solid rgba(255, 255, 255, 0.1);
      border-radius: 0.75rem;
      box-shadow:
        0 2rem 5rem var(--shadow),
        0 0 3rem rgba(229, 9, 36, 0.16);
      cursor: pointer;
      transform: translate(-50%, -50%);
      transition:
        opacity 0.65s ease 0.75s,
        visibility 0s linear 1.4s,
        transform 0.85s cubic-bezier(0.2, 0.75, 0.2, 1);
    }

    .envelope:hover {
      transform: translate(-50%, -52%) scale(1.015);
    }

    .envelope.open {
      opacity: 0;
      visibility: hidden;
      transform: translate(-50%, 18%) scale(0.84);
    }

    .envelope-front {
      position: absolute;
      z-index: 3;
      inset: 0;
      overflow: hidden;
      border-radius: inherit;
    }

    .envelope-front::before,
    .envelope-front::after {
      position: absolute;
      bottom: -48%;
      width: 74%;
      height: 115%;
      background: #111319;
      border: 1px solid rgba(255, 255, 255, 0.05);
      content: "";
    }

    .envelope-front::before {
      left: -12%;
      transform: rotate(37deg);
    }

    .envelope-front::after {
      right: -12%;
      transform: rotate(-37deg);
    }

    .envelope-flap {
      position: absolute;
      z-index: 5;
      top: 0;
      left: 0;
      width: 100%;
      height: 58%;
      background: linear-gradient(160deg, #252832, #101218);
      clip-path: polygon(0 0, 100% 0, 50% 100%);
      transform-origin: top;
      transition:
        z-index 0s linear 0.42s,
        transform 0.8s cubic-bezier(0.65, 0, 0.35, 1);
    }

    .envelope.open .envelope-flap {
      z-index: 1;
      transform: rotateX(180deg);
    }

    .envelope-content {
      position: absolute;
      z-index: 4;
      inset: 0;
      display: grid;
      padding: 1.5rem;
      place-items: center;
    }

    .seal {
      display: grid;
      width: 5.5rem;
      height: 5.5rem;
      place-items: center;
      color: #ffffff;
      background:
        radial-gradient(circle at 35% 25%, #ff415d, transparent 30%),
        linear-gradient(145deg, var(--accent-bright), var(--accent-dark));
      border: 0.35rem solid rgba(255, 255, 255, 0.12);
      border-radius: 50%;
      box-shadow:
        0 0.75rem 1.4rem rgba(0, 0, 0, 0.4),
        0 0 2rem rgba(229, 9, 36, 0.36);
      animation: sealPulse 2.2s ease-in-out infinite;
    }

    .seal svg {
      width: 2.9rem;
      height: 2.9rem;
      fill: currentColor;
    }

    .open-hint {
      position: absolute;
      z-index: 6;
      right: 0;
      bottom: 1rem;
      left: 0;
      color: #ffffff;
      font-size: 0.78rem;
      font-weight: 800;
      letter-spacing: 0.18em;
      text-transform: uppercase;
    }

    .letter {
      position: relative;
      z-index: 2;
      width: min(700px, 100%);
      min-height: 450px;
      padding: clamp(1.5rem, 5vw, 3.4rem);
      color: var(--text);
      text-align: left;
      background:
        linear-gradient(var(--paper), var(--paper)) padding-box,
        linear-gradient(135deg, var(--accent-bright), transparent 35%, var(--accent-dark))
        border-box;
      border: 1px solid transparent;
      border-radius: 1rem;
      box-shadow:
        0 2rem 5rem var(--shadow),
        0 0 3rem rgba(229, 9, 36, 0.12);
      opacity: 0;
      transform: translateY(65px) rotateX(-8deg) scale(0.93);
      transition:
        opacity 0.75s ease 0.7s,
        transform 1s cubic-bezier(0.2, 0.8, 0.2, 1) 0.6s,
        color 0.45s ease,
        background 0.45s ease,
        box-shadow 0.45s ease;
    }

    .letter.show {
      opacity: 1;
      transform: translateY(0) rotateX(0) scale(1);
    }

    .letter::before {
      position: absolute;
      top: 0;
      right: 0;
      width: 8rem;
      height: 8rem;
      background:
        repeating-radial-gradient(
          circle at 100% 0,
          transparent 0 1rem,
          var(--web) 1.05rem 1.1rem
        );
      border-radius: 0 1rem 0 100%;
      content: "";
      pointer-events: none;
    }

    .letter-tag {
      display: inline-block;
      margin-bottom: 1.2rem;
      padding: 0.42rem 0.75rem;
      color: var(--button-text);
      background: var(--accent);
      border-radius: 999px;
      font-size: 0.72rem;
      font-weight: 800;
      letter-spacing: 0.12em;
      text-transform: uppercase;
    }

    .letter h2 {
      margin-bottom: 1.4rem;
      font-size: clamp(1.55rem, 4.5vw, 2.4rem);
      letter-spacing: -0.03em;
    }

    .letter p {
      margin-bottom: 1rem;
      color: var(--muted);
      font-size: clamp(0.93rem, 2vw, 1.03rem);
      line-height: 1.78;
    }

    .letter strong {
      color: var(--text);
    }

    .signature {
      margin-top: 1.7rem;
      color: var(--text);
    }

    .signature span {
      display: block;
      margin-top: 0.25rem;
      color: var(--accent-bright);
      font-size: 1.35rem;
      font-weight: 800;
    }

    .actions {
      display: flex;
      flex-wrap: wrap;
      gap: 0.75rem;
      justify-content: center;
      margin-top: 1.35rem;
      opacity: 0;
      transform: translateY(1rem);
      transition:
        opacity 0.5s ease 1.35s,
        transform 0.5s ease 1.35s;
    }

    .actions.show {
      opacity: 1;
      transform: translateY(0);
    }

    .action-button {
      padding: 0.72rem 1rem;
      color: var(--text);
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 999px;
      cursor: pointer;
      transition:
        color 0.25s ease,
        background 0.25s ease,
        border-color 0.25s ease,
        transform 0.25s ease;
    }

    .action-button:hover {
      color: var(--button-text);
      background: var(--accent);
      border-color: var(--accent);
      transform: translateY(-2px);
    }

    .particle {
      position: fixed;
      z-index: 20;
      width: 0.55rem;
      height: 0.55rem;
      background: var(--accent-bright);
      border-radius: 50%;
      pointer-events: none;
      animation: burst 1.15s ease-out forwards;
    }

    @keyframes sealPulse {
      0%,
      100% {
        transform: scale(1);
      }

      50% {
        transform: scale(1.06);
      }
    }

    @keyframes burst {
      from {
        opacity: 1;
        transform: translate(0, 0) scale(1);
      }

      to {
        opacity: 0;
        transform:
          translate(var(--move-x), var(--move-y))
          scale(0.15)
          rotate(360deg);
      }
    }

    @media (max-width: 600px) {
      .brand-text {
        display: none;
      }

      .page-header {
        padding-top: 0.85rem;
      }

      main {
        padding-top: 1.5rem;
      }

      .intro {
        margin-bottom: 1.4rem;
      }

      .letter-stage {
        min-height: 560px;
      }

      .letter {
        padding: 1.5rem;
      }
    }

    @media (prefers-reduced-motion: reduce) {
      *,
      *::before,
      *::after {
        scroll-behavior: auto !important;
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
        transition-delay: 0ms !important;
      }
    }
  </style>
</head>

<body>
  <div class="web-lines" aria-hidden="true">
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
  </div>

  <header class="page-header">
    <div class="brand">
      <div class="brand-mark" aria-hidden="true">
        <svg viewBox="0 0 100 100">
          <path d="M44 8h12v22l14-14 8 9-17 16h28v12H62l17 17-9 8-14-15v29H44V63L30 78l-9-8 17-17H11V41h28L22 25l8-9 14 14V8Z"/>
        </svg>
      </div>
      <span class="brand-text">A Heroic Teacher</span>
    </div>

    <button
      class="theme-toggle"
      id="themeToggle"
      type="button"
      aria-label="Switch to light mode"
      aria-pressed="false"
    >
      <span class="toggle-track" aria-hidden="true">
        <span>☾</span>
        <span>☀</span>
      </span>
      <span class="toggle-label" id="themeLabel">Dark</span>
    </button>
  </header>

  <main>
    <section class="hero" aria-labelledby="pageTitle">
      <p class="eyebrow">For our web development hero</p>

      <h1 id="pageTitle">
        Happy Teacher's Day,
        <span>Sir Randy Bello!</span>
      </h1>

      <p class="intro">
        Behind every skilled developer is a teacher who helped them take the
        first leap. This message is especially for you.
      </p>

      <div class="letter-stage">
        <button
          class="envelope"
          id="envelope"
          type="button"
          aria-label="Open Teacher's Day letter"
          aria-expanded="false"
          aria-controls="letter"
        >
          <span class="envelope-flap" aria-hidden="true"></span>
          <span class="envelope-front" aria-hidden="true"></span>

          <span class="envelope-content">
            <span class="seal" aria-hidden="true">
              <svg viewBox="0 0 100 100">
                <path d="M44 8h12v22l14-14 8 9-17 16h28v12H62l17 17-9 8-14-15v29H44V63L30 78l-9-8 17-17H11V41h28L22 25l8-9 14 14V8Z"/>
              </svg>
            </span>

            <span class="open-hint">Click to open the letter</span>
          </span>
        </button>

        <article class="letter" id="letter" aria-hidden="true">
          <span class="letter-tag">Teacher's Day 2026</span>

          <h2>Dear Sir Randy Bello,</h2>

          <p>
            Happy Teacher's Day! Thank you for guiding us through the exciting
            world of web development. You have taught us that building a website
            is not only about writing code - it is also about creativity,
            patience, problem-solving, and creating something meaningful.
          </p>

          <p>
            Like a hero who helps others discover their own strength, you
            encourage us to face every bug, error, and difficult lesson with
            courage. Because of your guidance, every challenge has become a new
            opportunity to learn and improve.
          </p>

          <p>
            Thank you for sharing your knowledge, answering our questions, and
            believing in what we can create. Your lessons will remain part of
            every project and every line of code we write.
          </p>

          <p>
            We appreciate everything you do, Sir Randy. May you continue to
            inspire many more students and future developers.
          </p>

          <p class="signature">
            With gratitude and respect,
            Justin Brix Adigue
            <span>Your Web Development Student</span>
          </p>
        </article>
      </div>

      <div class="actions" id="actions">
        <button class="action-button" id="closeLetter" type="button">
          Close letter
        </button>

        <button class="action-button" id="celebrate" type="button">
          Celebrate!
        </button>
      </div>
    </section>
  </main>

  <script>
    const body = document.body;
    const envelope = document.getElementById("envelope");
    const letter = document.getElementById("letter");
    const actions = document.getElementById("actions");
    const closeLetterButton = document.getElementById("closeLetter");
    const celebrateButton = document.getElementById("celebrate");
    const themeToggle = document.getElementById("themeToggle");
    const themeLabel = document.getElementById("themeLabel");

    const savedTheme = localStorage.getItem("teachers-day-theme");
    const systemPrefersLight = window.matchMedia(
      "(prefers-color-scheme: light)"
    ).matches;

    function setTheme(theme) {
      const isLight = theme === "light";

      body.classList.toggle("light-mode", isLight);
      themeToggle.setAttribute("aria-pressed", String(isLight));
      themeToggle.setAttribute(
        "aria-label",
        isLight ? "Switch to dark mode" : "Switch to light mode"
      );
      themeLabel.textContent = isLight ? "Light" : "Dark";

      localStorage.setItem("teachers-day-theme", theme);
    }

    setTheme(savedTheme || (systemPrefersLight ? "light" : "dark"));

    themeToggle.addEventListener("click", () => {
      setTheme(body.classList.contains("light-mode") ? "dark" : "light");
    });

    function openLetter() {
      envelope.classList.add("open");
      letter.classList.add("show");
      actions.classList.add("show");

      envelope.setAttribute("aria-expanded", "true");
      letter.setAttribute("aria-hidden", "false");

      createCelebration(24);
    }

    function closeLetter() {
      envelope.classList.remove("open");
      letter.classList.remove("show");
      actions.classList.remove("show");

      envelope.setAttribute("aria-expanded", "false");
      letter.setAttribute("aria-hidden", "true");

      window.setTimeout(() => envelope.focus(), 850);
    }

    function createCelebration(amount = 36) {
      const originX = window.innerWidth / 2;
      const originY = Math.min(window.innerHeight * 0.6, 600);

      for (let i = 0; i < amount; i += 1) {
        const particle = document.createElement("span");
        const angle = Math.random() * Math.PI * 2;
        const distance = 70 + Math.random() * 230;
        const size = 4 + Math.random() * 8;

        particle.className = "particle";
        particle.style.left = `${originX}px`;
        particle.style.top = `${originY}px`;
        particle.style.width = `${size}px`;
        particle.style.height = `${size}px`;
        particle.style.background =
          Math.random() > 0.35 ? "var(--accent-bright)" : "var(--text)";
        particle.style.setProperty(
          "--move-x",
          `${Math.cos(angle) * distance}px`
        );
        particle.style.setProperty(
          "--move-y",
          `${Math.sin(angle) * distance}px`
        );

        document.body.appendChild(particle);

        particle.addEventListener("animationend", () => {
          particle.remove();
        });
      }
    }

    envelope.addEventListener("click", openLetter);
    closeLetterButton.addEventListener("click", closeLetter);
    celebrateButton.addEventListener("click", () => createCelebration(48));

    document.addEventListener("keydown", (event) => {
      if (event.key === "Escape" && letter.classList.contains("show")) {
        closeLetter();
      }
    });
  </script>
</body>
</html>
