<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>KS DIGITAL SERVICES</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700;400&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #1E90FF;   /* Deep Sky Blue */
      --accent: #00CED1;    /* Vibrant Teal */
      --bg: #f0f4f8;        /* Light Gray-Blue */
      --white: #fff;
      --text-dark: #333333;
      --radius: 16px;
      --shadow: 0 8px 24px rgba(0, 0, 0, 0.1);
      --highlight: rgba(0, 206, 209, 0.2);
    }
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #f0f4f8, #e8f0f5);
      min-height: 100vh;
      font-family: 'Montserrat', Arial, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      animation: backgroundAnimation 20s ease-in-out infinite;
    }
    @keyframes backgroundAnimation {
      0% {
        background: linear-gradient(135deg, #f0f4f8, #e8f0f5);
      }
      50% {
        background: linear-gradient(135deg, #e8f0f5, #c1d9e2);
      }
      100% {
        background: linear-gradient(135deg, #f0f4f8, #e8f0f5);
      }
    }
    header {
      width: 100%;
      padding: 40px 0;
      background-color: var(--primary);
      color: var(--white);
      text-align: center;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
      border-radius: 0 0 30px 30px;
      margin-bottom: 30px;
      position: relative;
    }
    h1 {
      font-size: 2.6rem;
      font-weight: 700;
      letter-spacing: 1px;
      margin: 0;
      text-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
    }
    .top-btn {
      position: absolute;
      left: 30px;
      top: 36px;
      padding: 12px 25px;
      background: var(--white);
      color: var(--primary);
      border: none;
      border-radius: var(--radius);
      font-size: 1.1rem;
      font-weight: 600;
      box-shadow: var(--shadow);
      text-decoration: none;
      transition: background 0.2s, color 0.2s, box-shadow 0.2s;
      cursor: pointer;
    }
    .top-btn:hover, .top-btn:focus {
      background: var(--accent);
      color: var(--white);
      box-shadow: 0 4px 24px rgba(0, 206, 209, 0.3);
    }
    .btn-group {
      display: flex;
      flex-direction: column;
      gap: 24px;
      width: 100%;
      max-width: 600px;
      align-items: center;
      margin-top: 20px;
    }
    .btn-row {
      display: flex;
      gap: 16px;
      justify-content: center;
      flex-wrap: wrap;
      width: 100%;
    }
    .action-btn {
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.1rem;
      font-weight: 500;
      background: var(--primary);
      color: var(--white);
      border: none;
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 18px 30px;
      cursor: pointer;
      transition: transform 0.15s, box-shadow 0.3s, background-color 0.3s;
      text-decoration: none;
      outline: none;
      gap: 12px;
      max-width: 240px;
      width: 100%;
      position: relative;
      overflow: hidden;
    }
    .action-btn:hover, .action-btn:focus {
      transform: scale(1.05);
      background-color: var(--accent);
      box-shadow: 0 8px 24px rgba(0, 206, 209, 0.3);
    }
    .action-btn::before {
      content: "";
      position: absolute;
      z-index: 1;
      left: -100px;
      top: 0;
      width: 50px;
      height: 100%;
      background: var(--highlight);
      transform: skewX(-20deg);
      animation: btnShine 3s infinite linear;
      opacity: 0.6;
    }
    @keyframes btnShine {
      0% { left: -100px; }
      100% { left: 100%; }
    }
    .icon {
      width: 28px;
      height: 28px;
    }
    .icon path {
      fill: var(--white);
    }
    @media (max-width: 600px) {
      body {
        padding: 10px;
      }
      header {
        padding: 20px 0;
      }
      h1 {
        font-size: 1.8rem;
      }
      .btn-group {
        margin-top: 20px;
        gap: 16px;
        width: 90%;
      }
      .top-btn {
        position: static;
        margin-bottom: 16px;
        font-size: 1rem;
        width: 100%;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>KS DIGITAL SERVICES</h1>
    <div style="text-align: center; margin-top: 20px;">
      <a class="top-btn" href="https://ksdigitalservice.pw/">HOME PAGE</a>
    </div>
  </header>

  <main>
    <div class="btn-group">
      <div class="btn-row">
        <a class="action-btn" href="tel:+917893845696">
          <svg class="icon" fill="none" viewBox="0 0 24 24">
            <circle cx="12" cy="12" r="12" fill="#00CED1"/>
            <path d="M16 13l-2.5.5a8.2 8.2 0 01-3-3L11 8c.2-.4.1-.9-.3-1.1l-2-1.2A1 1 0 007 6.8C7 13 11 17 17.2 17c.3 0 .7-.2.9-.6l1-2a1 1 0 00-.5-1.3l-2.9-1.1a1 1 0 00-1.5 1.1z" fill="#fff"/>
          </svg>
          <span>Call</span>
        </a>
        <a class="action-btn" href="https://maps.app.goo.gl/VfZ4fHYw6nYFTavB6" target="_blank" rel="noopener">
          <svg class="icon" fill="none" viewBox="0 0 24 24">
            <circle cx="12" cy="12" r="12" fill="#1E90FF"/>
            <path d="M12 6c-2.5 0-4.5 2-4.5 4.7 0 3.5 3.8 6.6 4 6.8.2.2.6.2.8 0 0 0 4-3.2 4-6.8C1            4-3.2 4-6.8C16.5 8 14.5 6 12 6zm0 6.2c-.8 0-1.5-.7-1.5-1.5S11.2 9.2 12 9.2s1.5.7 1.5 1.5-.7 1.5-1.5 1.5z" fill="#fff"/>
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

