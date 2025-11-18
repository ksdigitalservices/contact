<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>KS DIGITAL SERVICES</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700;400&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #00e5ff; /* Neon Blue */
      --accent: #ff4081;  /* Neon Pink */
      --bg-dark: #121212; /* Dark Background */
      --white: #fff;
      --radius: 12px;
      --shadow: 0 12px 48px rgba(0, 0, 0, 0.3);
      --glow: rgba(0, 229, 255, 0.3);
    }
    body {
      margin: 0;
      padding: 0;
      font-family: 'Montserrat', Arial, sans-serif;
      background: linear-gradient(135deg, #121212 0%, #222222 100%);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      overflow: hidden;
      position: relative;
    }
    
    /* 3D Particle Animation Background */
    .particle-background {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: radial-gradient(circle, rgba(0, 0, 0, 0.5), transparent);
      z-index: -1;
      animation: particleMovement 5s infinite alternate;
    }

    @keyframes particleMovement {
      0% {
        transform: translate3d(0, 0, 0);
      }
      100% {
        transform: translate3d(50%, -50%, 0);
      }
    }

    header {
      width: 100%;
      padding: 40px 0;
      background: #1e1e1e;
      text-align: center;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.6);
      position: relative;
    }
    
    h1 {
      color: var(--white);
      font-size: 2.8rem;
      font-weight: 700;
      margin: 0;
      letter-spacing: 1px;
      text-shadow: 0 0 8px var(--primary), 0 0 16px var(--primary);
    }
    
    .top-btn {
      position: absolute;
      left: 30px;
      top: 36px;
      padding: 10px 20px;
      background: var(--primary);
      color: var(--white);
      border: none;
      border-radius: var(--radius);
      font-size: 1rem;
      font-weight: 600;
      box-shadow: var(--shadow);
      text-decoration: none;
      transition: background 0.3s, box-shadow 0.3s, transform 0.3s;
      cursor: pointer;
    }

    .top-btn:hover {
      background: var(--accent);
      box-shadow: 0 4px 20px rgba(255, 64, 129, 0.5);
      transform: translateY(-3px);
    }

    main {
      width: 100%;
      padding: 40px 10px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    .btn-group {
      display: flex;
      flex-direction: column;
      gap: 20px;
      margin-top: 40px;
      width: 100%;
      max-width: 480px;
    }

    .btn-row {
      display: flex;
      justify-content: center;
      gap: 15px;
      flex-wrap: wrap;
    }

    .action-btn {
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.1rem;
      font-weight: 500;
      background: linear-gradient(45deg, var(--primary), var(--accent));
      color: var(--white);
      border: none;
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 24px;
      cursor: pointer;
      transition: transform 0.3s ease, box-shadow 0.4s ease;
      text-decoration: none;
      position: relative;
    }

    .action-btn::before {
      content: "";
      position: absolute;
      top: 0;
      left: -200%;
      width: 100%;
      height: 100%;
      background: rgba(255, 255, 255, 0.15);
      transform: skewX(-45deg);
      animation: buttonShine 2.5s infinite linear;
    }

    @keyframes buttonShine {
      0% { left: -200%; }
      100% { left: 100%; }
    }

    .action-btn:hover {
      transform: translateY(-6px) scale(1.05);
      box-shadow: 0 12px 36px rgba(255, 64, 129, 0.6);
    }

    .icon {
      width: 24px;
      height: 24px;
      margin-right: 12px;
      filter: drop-shadow(0 2px 10px rgba(0, 229, 255, 0.3));
    }

    /* Responsive Design */
    @media (max-width: 600px) {
      h1 {
        font-size: 1.6rem;
      }
      .top-btn {
        position: static;
        margin-top: 20px;
        width: 90%;
        max-width: 320px;
      }
      .btn-group {
        gap: 10px;
      }
      .btn-row {
        flex-direction: column;
        gap: 12px;
      }
    }
  </style>
</head>

<body>
  <div class="particle-background"></div> <!-- 3D particle background -->
  <header>
    <h1>KS DIGITAL SERVICES</h1>
    <a class="top-btn" href="https://ksdigitalservice.pw/">HOME PAGE</a>
  </header>

  <main>
    <div class="btn-group">
      <div class="btn-row">
        <a class="action-btn" href="tel:+917893845696">
          <svg class="icon" fill="none" viewBox="0 0 24 24">
            <circle cx="12" cy="12" r="12" fill="#00e5ff"/>
            <path d="M16 13l-2.5.5a8.2 8.2 0 01-3-3L11 8c.2-.4.1-.9-.3-1.1l-2-1.2A1 1 0 007 6.8C7 13 11 17 17.2 17c.3 0 .7-.2.9-.6l1-2a1 1 0 00-.5-1.3l-2.9-1.1a1 1 0 00-1.5 1.1z" fill="#fff"/>
          </svg>
          <span>Call</span>
        </a>

        <a class="action-btn" href="https://maps.app.goo.gl/VfZ4fHYw6nYFTavB6" target="_blank" rel="noopener">
          <svg class="icon" fill="none" viewBox="0 0 24 24">
            <circle cx="12" cy="12" r="12" fill="#ff4081"/>
            <path d="M12 6c-2.5 0-4.5 2-4.5 4.7 0 3.5 3.8 6.6 4 6.8.2.2.6.2.8 0 0 0 4-3.2 4-6.8C16.5 8 14.5 6 12 6zm0 6.2c-.8 0-1.5-.7-1.5-1.5S11.2 9.2 12 9.2s1.5.7 1.5 1.5-.7 1.5-1.5 1.5z" fill="#fff"/>
          </svg>
          <span>Get Directions</span>
        </a>
      </div>

      <div class="btn-row">
        <a class="action-btn" href="https://wa.me/7893845696" target="_blank" rel="noopener">
          <svg class="icon" fill="none" viewBox="0 0 24 24">
            <circle cx="12" cy="12" r="12" fill="#25D366"/>
            <path d="M16.2 13.7c-.2-.1-1.2-.6-1.4-.7-.2-.1-.4-.2-.6.2-.2.3-.6.7-.8.8-.1.1-.3.1-.5 0-.3-.1-1.1-.4-2.1-1.4-.8-.8-1.4-1.8-1.6-2.1-.1-.2 0-.4.1-.5.1-.1.2-.2.3-.4.1-.1.2-.2.3-.3.1-.1.1-.2.2-.4.1-.2 0-.3-.1-.4-.1-.1-1.4-1.4-1.6-1.5-.2-.1-.4-.2-.5-.2s-.3 0-.5.1c-.2.2-.9.8-.9 2 .1 1.7 1.8 3.6 2.2 4 .3.3.7.6 1.1.9.8.6 2.5 1.4 3.3 1.4.7 0 1.2-.4 1.4-.7.2-.3.9-1 .4-1.2z" fill="#FFF"/>
          </svg>
          <span>WhatsApp</span>
        </a>
        
        
         <a class="action-btn" href="https://www.instagram.com/ksdigitalservice/" target="_blank" rel="noopener">
          <svg class="icon" viewBox="0 0 24 24" fill="none">
            <circle cx="12" cy="12" r="12" fill="#e1306c"/>
            <rect x="6.6" y="6.6" width="10.8" height="10.8" rx="3.2" fill="#fff"/>
            <circle cx="12" cy="12" r="3" fill="#e1306c"/>
            <circle cx="15.4" cy="8.8" r="0.8" fill="#e1306c"/>
          </svg>
          <span>Instagram</span>
        </a>
      </div>

      <div class="btn-row">
        <a class="action-btn" href="https://www.youtube.com/@ksdigitalservice" target="_blank" rel="noopener">
          <svg class="icon" fill="none" viewBox="0 0 24 24">
            <circle cx="12" cy="12" r="12" fill="#ff0000"/>
            <polygon points="10,8 16,12 10,16" fill="#fff"/>
          </svg>
          <span>YouTube</span>
        </a>

        <a class="action-btn" href="https://ksdigitalservice.pw/print/1" target="_blank" rel="noopener">
          <svg class="icon" viewBox="0 0 24 24" fill="none">
            <circle cx="12" cy="12" r="12" fill="#3b82f6"/>
            <rect x="7" y="10" width="10" height="7" rx="1" fill="#fff"/>
            <rect x="9.5" y="7" width="5" height="4" rx="0.5" fill="#e5e7eb"/>
          </svg>
          <span>Self Printer</span>
        </a>
      </div>
    </div>
  </main>
</body>
</html>
