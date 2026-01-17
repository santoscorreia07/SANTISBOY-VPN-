<html lang="pt-BR">
<!--    @LightVVD       -->
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>DT OENYGMA</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style id="fa-fallback">
    /* Este estilo só será ativado se o script de fallback for executado */
    .fa-power-off-fallback {
      display: none;
    }
  </style>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@700&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Shippori+Mincho:wght@700&display=swap');

    :root {
      --body-bg: #0A0A10;
      --body-bg-rgb: 10, 10, 16;
      --phone-bg: #0e0e38;
      --primary-text: #ffffff;
      --secondary-text: #b0b0d0;
      --boost-color: #fdd835;
      --notification-bg: linear-gradient(90deg, #0575E6 0%, #58a6ff 100%);
      --notification-shadow: rgba(160, 68, 255, 0.2);
      --server-select-bg: rgba(30, 30, 63, 0.5);
      --server-select-border: rgba(255, 255, 255, 0.1);
      --world-map-opacity: 0.15;
      --power-btn-container-bg: #101021;
      --power-btn-container-shadow: 0 0 25px rgba(0, 0, 0, 0.7), inset 0 0 15px rgba(0, 0, 0, 0.6);
      --power-btn-bg: #08080c;
      --power-btn-bg-hover: #111;
      --power-btn-shadow: 0 5px 10px rgba(0, 0, 0, 0.5);
      --power-icon-color: #333;
      --power-icon-hover-color: #ffffff;
      --power-icon-hover-shadow: 0 0 20px #ffffff, 0 0 40px rgba(160, 68, 255, 0.7);
      --theme-icon-color: #fdd835;
      --navbar-bg: rgba(16, 16, 33, 0.95);
      --dragon-red: #c0392b;
      --success-color: #3fb950;
      --success-color-rgb: 63, 185, 80;
    }

    body.light-theme {
      --body-bg: #f8fafc;
      --body-bg-rgb: 248, 250, 252;
      --phone-bg: #ffffff;
      --primary-text: #1e293b;
      --secondary-text: #64748b;
      --boost-color: #f59e0b;
      --notification-bg: linear-gradient(90deg, #3b82f6 0%, #60a5fa 100%);
      --notification-shadow: rgba(59, 130, 246, 0.25);
      --server-select-bg: #ffffff;
      --server-select-border: rgba(0, 0, 0, 0.05);
      --world-map-opacity: 0.04;
      --power-btn-container-bg: #f1f5f9;
      --power-btn-container-shadow: 0 0 25px rgba(0, 0, 0, 0.03), inset 0 0 15px rgba(0, 0, 0, 0.02);
      --power-btn-bg: #ffffff;
      --power-btn-bg-hover: #f8fafc;
      --power-btn-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
      --power-icon-color: #94a3b8;
      --power-icon-hover-color: #0f172a;
      --power-icon-hover-shadow: 0 0 20px rgba(var(--accent-color-rgb), 0.3), 0 0 40px rgba(var(--accent-color-rgb), 0.15);
      --theme-icon-color: #f59e0b;
      --navbar-bg: rgba(255, 255, 255, 0.98);
      --dragon-red: #ef4444;
      --success-color: #10b981;
      --success-color-rgb: 16, 185, 129;
      --error-color: #ef4444;
      --warning-color: #f59e0b;
    }

    body.light-theme {
      -webkit-font-smoothing: subpixel-antialiased;
      letter-spacing: 0.015em;
    }

    /* Color Themes */
    body[data-color-theme="purple"] {
      --accent-color: #a044ff;
      --accent-color-rgb: 160, 68, 255;
    }

    body[data-color-theme="purple"].light-theme {
      --accent-color: #a044ff;
      --accent-color-rgb: 160, 68, 255;
    }

    body[data-color-theme="blue"] {
      --accent-color: #58a6ff;
      --accent-color-rgb: 88, 166, 255;
      --notification-bg: linear-gradient(90deg, #0575E6 0%, #58a6ff 100%);
      --phone-bg: #0e0e38;
    }

    body[data-color-theme="blue"].light-theme {
      --accent-color: #3b82f6;
      --accent-color-rgb: 59, 130, 246;
      --notification-bg: linear-gradient(90deg, #3b82f6 0%, #60a5fa 100%);
      --phone-bg: #ffffff;
    }

    body[data-color-theme="green"] {
      --accent-color: #34d399;
      --accent-color-rgb: 52, 211, 153;
    }

    body[data-color-theme="green"].light-theme {
      --accent-color: #10b981;
      --accent-color-rgb: 16, 185, 129;
    }

    body[data-color-theme="red"] {
      --accent-color: #e57373;
      --accent-color-rgb: 229, 115, 115;
    }

    body[data-color-theme="red"].light-theme {
      --accent-color: #ef4444;
      --accent-color-rgb: 239, 68, 68;
    }

    body {
      font-family: 'Roboto', sans-serif;
      background-color: var(--body-bg);
      color: var(--primary-text);
      margin: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      transition: background-color 0.4s ease-in-out, color 0.4s ease-in-out;
    }

    body.navbar-open .phone-mockup {
      filter: blur(2px);
      transition: filter 0.3s ease;
    }

    .phone-mockup {
      width: 375px;
      height: 812px;
      background-color: var(--phone-bg);
      border-radius: 40px;
      box-shadow: 0 10px 40px rgba(0, 0, 0, 0.5);
      padding: 20px;
      box-sizing: border-box;
      display: flex;
      flex-direction: column;
      position: relative;
      overflow: hidden;
      transition: background-color 0.3s ease, filter 0.3s ease, box-shadow 0.3s ease;
    }

    .phone-mockup::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background-image: var(--main-bg-image);
      background-repeat: no-repeat;
      background-position: center var(--main-bg-position-y, 180px);
      background-size: 488px;
      opacity: var(--world-map-opacity);
      z-index: 1;
      transition: opacity 0.3s ease;
    }

    header,
    .notification,
    .server-select,
    main {
      position: relative;
      z-index: 2;
      padding: 0 10px;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding-top: 20px;
      padding-bottom: 10px;
    }

    header h1 {
      font-family: 'Poppins', sans-serif;
      font-size: 28px;
      margin: 0;
      font-weight: 700;
      flex-grow: 1;
      text-align: center;
      letter-spacing: 1px;
      color: var(--primary-text);
    }

    header h1 .kanji {
      color: var(--accent-color);
    }

    header .boost {
      color: var(--boost-color);
      font-size: 18px;
      margin-left: 8px;
      vertical-align: middle;
    }

    header .fa-bars {
      font-size: 24px;
      color: var(--secondary-text);
    }

    #theme-toggle {
      font-size: 22px;
      cursor: pointer;
      color: var(--theme-icon-color);
      transition: color 0.3s ease, transform 0.2s ease;
    }

    #theme-toggle:hover {
      transform: rotate(12deg);
    }

    body.light-theme #theme-toggle {
      color: #E6A23C;
    }

    .notification {
      background: var(--notification-bg);
      border-radius: 12px;
      padding: 12px 15px;
      margin: 20px 0;
      text-align: center;
      box-shadow: 0 4px 15px var(--notification-shadow);
    }

    .notification p {
      margin: 0;
      font-size: 15px;
      font-weight: 500;
      color: #ffffff;
    }

    .server-select {
      background-color: var(--server-select-bg);
      backdrop-filter: blur(5px);
      border: 1px solid var(--server-select-border);
      border-radius: 12px;
      padding: 12px 15px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      cursor: pointer;
      transition: background-color 0.3s ease, border-color 0.3s ease;
    }

    .server-info {
      display: flex;
      align-items: center;
    }

    .server-info img {
      width: 35px;
      height: auto;
      margin-right: 15px;
    }

    .server-info div {
      display: flex;
      flex-direction: column;
    }

    .server-info span {
      font-size: 16px;
      font-weight: 700;
      color: var(--primary-text);
    }

    .server-info small {
      font-size: 13px;
      color: var(--secondary-text);
    }

    .fa-chevron-down {
      color: var(--secondary-text);
    }

    .server-actions {
      display: flex;
      align-items: center;
      gap: 15px;
    }

    .server-action-icon {
      color: var(--secondary-text);
      cursor: pointer;
      transition: color 0.2s ease, transform 0.2s ease;
      margin-right: 4px;
      stroke-width: 1.5;
      position: relative;
    }

    .server-action-icon:hover {
      color: var(--accent-color);
      transform: scale(1.1);
    }

    .server-action-icon::after {
      content: "Auto Conexão";
      position: absolute;
      top: -30px;
      left: 50%;
      transform: translateX(-50%);
      background: rgba(var(--body-bg-rgb), 0.95);
      color: var(--primary-text);
      padding: 4px 8px;
      border-radius: 4px;
      font-size: 12px;
      white-space: nowrap;
      opacity: 0;
      visibility: hidden;
      transition: opacity 0.2s ease, visibility 0.2s ease;
      pointer-events: none;
      border: 1px solid var(--server-select-border);
    }

    .server-action-icon:hover::after {
      opacity: 1;
      visibility: visible;
    }

    main {
      flex-grow: 1;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding-bottom: 50px;
    }

    main.connected-state .power-button-container {
      margin-top: 40px;
      width: 180px !important;
      height: 180px !important;
    }

    main.connected-state .power-button {
      width: 140px !important;
      height: 140px !important;
    }

    .power-button-container {
      width: 180px;
      height: 180px;
      min-width: 180px;
      min-height: 180px;
      background-color: var(--power-btn-container-bg);
      border-radius: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      box-shadow: var(--power-btn-container-shadow);
      margin-bottom: 25px;
      transition: background-color 0.3s ease, box-shadow 0.3s ease, border 0.3s ease;
      border: 4px solid transparent;
      flex-shrink: 0;
    }

    .power-button {
      width: 140px;
      height: 140px;
      min-width: 140px;
      min-height: 140px;
      border-radius: 50%;
      background-color: var(--power-btn-bg);
      border: none;
      display: flex;
      justify-content: center;
      align-items: center;
      cursor: pointer;
      transition: all 0.3s ease-in-out;
      box-shadow: var(--power-btn-shadow);
      flex-shrink: 0;
    }

    .power-button .fa-power-off {
      font-size: 65px;
      color: var(--power-icon-hover-color);
      text-shadow: var(--power-icon-hover-shadow);
      transition: all 0.3s ease-in-out;
    }

    .power-button:hover {
      background-color: var(--power-btn-bg-hover);
    }

    .connect-text {
      font-size: 18px;
      color: var(--secondary-text);
      font-weight: 600;
      transition: all 0.5s cubic-bezier(0.19, 1, 0.22, 1);
      padding: 10px 24px;
      border-radius: 50px;
      border: 1px solid rgba(var(--accent-color-rgb), 0.15);
      background-color: rgba(var(--body-bg-rgb), 0.3);
      backdrop-filter: blur(5px);
      -webkit-backdrop-filter: blur(5px);
      display: flex;
      align-items: center;
      justify-content: center;
      min-width: 200px;
      text-align: center;
      position: relative;
      overflow: hidden;
      letter-spacing: 0.5px;
      box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
      transform-style: preserve-3d;
      transform: translateZ(0);
    }

    .connect-text::before {
      content: "";
      position: absolute;
      left: -100%;
      top: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg,
          rgba(var(--accent-color-rgb), 0) 0%,
          rgba(var(--accent-color-rgb), 0.1) 50%,
          rgba(var(--accent-color-rgb), 0) 100%);
      transition: left 0.7s ease;
      pointer-events: none;
    }

    .connect-text:hover::before {
      left: 100%;
    }

    .connect-text.connected-status {
      color: #ffffff;
      background: linear-gradient(135deg, var(--success-color), color-mix(in srgb, var(--success-color) 70%, #5cffb1));
      border-color: transparent;
      font-weight: 700;
      box-shadow: 0 5px 15px rgba(var(--success-color-rgb), 0.25),
        0 0 0 1px rgba(var(--success-color-rgb), 0.1);
      text-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
      min-width: 160px;
    }

    .connect-text.connected-status::before {
      background: linear-gradient(90deg,
          rgba(255, 255, 255, 0) 0%,
          rgba(255, 255, 255, 0.2) 50%,
          rgba(255, 255, 255, 0) 100%);
    }

    .connect-text.connected-status::after {
      content: "";
      position: absolute;
      left: -4px;
      top: -4px;
      right: -4px;
      bottom: -4px;
      border-radius: 50px;
      background: linear-gradient(135deg, var(--success-color), transparent);
      opacity: 0;
      z-index: -1;
      transition: opacity 0.5s ease;
      animation: pulse-connect 2s infinite;
    }

    @keyframes pulse-connect {
      0% {
        opacity: 0;
        transform: scale(0.95);
      }

      50% {
        opacity: 0.2;
        transform: scale(1.02);
      }

      100% {
        opacity: 0;
        transform: scale(0.95);
      }
    }

    body.light-theme .connect-text {
      border-color: rgba(var(--accent-color-rgb), 0.1);
      background-color: #ffffff;
      box-shadow: 0 3px 10px rgba(0, 0, 0, 0.03);
    }

    .app-version {
      font-size: 11px;
      color: var(--secondary-text);
      margin-top: auto;
      opacity: 0.7;
      padding-top: 15px;
      position: absolute;
      bottom: -13px;
      left: 0;
      right: 0;
      text-align: center;
    }

    body.light-theme .app-version {
      color: var(--secondary-text);
      opacity: 0.8;
      text-shadow: 0 1px 0 rgba(255, 255, 255, 0.5);
    }

    /* Navbar styles */
    #side-navbar {
      position: fixed;
      top: 50%;
      left: 50%;
      height: auto;
      max-height: 85vh;
      width: 90%;
      max-width: 360px;
      background-color: rgba(var(--body-bg-rgb), 0.7);
      backdrop-filter: blur(15px);
      z-index: 1001;
      transform: translate(-150%, -50%);
      transition: transform 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
      display: flex;
      flex-direction: column;
      padding: 15px;
      box-sizing: border-box;
      border-radius: 20px;
      border: 1px solid var(--server-select-border);
      color: var(--primary-text);
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.25);
      opacity: 0;
      pointer-events: none;
    }

    #navbar-overlay {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.5);
      backdrop-filter: blur(3px);
      z-index: 1000;
      opacity: 0;
      visibility: hidden;
      transition: opacity 0.3s ease-in-out, visibility 0.3s ease-in-out;
      pointer-events: none;
    }

    body.navbar-open #side-navbar {
      transform: translate(-50%, -50%);
      opacity: 1;
      pointer-events: all;
    }

    body.navbar-open #navbar-overlay {
      opacity: 1;
      visibility: visible;
      pointer-events: all;
    }

    .navbar-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding-bottom: 20px;
      border-bottom: 1px solid var(--server-select-border);
      margin-bottom: 20px;
    }

    .navbar-header h3 {
      margin: 0;
      font-size: 20px;
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(90deg, var(--accent-color), color-mix(in srgb, var(--accent-color) 70%, #ffffff));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    #close-nav {
      font-size: 24px;
      cursor: pointer;
      color: var(--secondary-text);
      transition: all 0.2s ease;
      width: 32px;
      height: 32px;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 50%;
    }

    #close-nav:hover {
      color: var(--accent-color);
      background-color: rgba(var(--accent-color-rgb), 0.1);
      transform: rotate(90deg);
    }

    .navbar-profile {
      text-align: center;
      padding: 25px 0;
      border-bottom: 1px solid var(--server-select-border);
      cursor: pointer;
      transition: all 0.2s ease;
      border-radius: 12px;
      margin-bottom: 20px;
    }

    .navbar-profile:hover {
      background-color: rgba(var(--accent-color-rgb), 0.08);
      transform: translateY(-2px);
    }

    .navbar-profile img {
      width: 80px;
      height: 80px;
      border-radius: 50%;
      border: 3px solid var(--accent-color);
      margin-bottom: 10px;
      box-shadow: 0 5px 15px rgba(var(--accent-color-rgb), 0.3);
      transition: all 0.2s ease;
    }

    .navbar-profile:hover img {
      transform: scale(1.05);
      box-shadow: 0 8px 20px rgba(var(--accent-color-rgb), 0.4);
    }

    .navbar-profile h4 {
      margin: 0 0 5px 0;
      font-size: 18px;
    }

    .navbar-profile p {
      margin: 0;
      font-size: 14px;
      color: var(--secondary-text);
    }

    .navbar-links {
      list-style: none;
      padding: 5px;
      margin: 0px 0;
      flex-grow: 1;
      overflow-x: auto;
      overflow-y: hidden;
      -ms-overflow-style: none;
      /* IE and Edge */
      scrollbar-width: none;
      /* Firefox */
      display: flex;
      flex-direction: row;
      gap: 15px;
      scroll-behavior: smooth;
      -webkit-overflow-scrolling: touch;
      flex-wrap: nowrap;
    }

    .navbar-links::-webkit-scrollbar {
      display: none;
      /* Chrome, Safari, Opera */
    }

    .navbar-links li {
      min-width: 120px;
      flex: 0 0 auto;
      cursor: grab;
      user-select: none;
    }

    .navbar-links li a {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 3px;
      color: var(--primary-text);
      text-decoration: none;
      font-size: 14px;
      border-radius: 30px;
      transition: all 0.2s ease;
      height: 90px;
      width: 100%;
      text-align: center;
      background-color: rgba(var(--body-bg-rgb), 0.3);
      border: 1px solid var(--server-select-border);
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    .navbar-links.dragging {
      cursor: grabbing;
      scroll-behavior: auto;
    }

    .navbar-links li a:hover {
      background-color: rgba(var(--accent-color-rgb), 0.1);
      color: var(--accent-color);
      transform: translateY(-3px);
      border-color: var(--accent-color);
      box-shadow: 0 5px 15px rgba(var(--accent-color-rgb), 0.2);
    }

    .navbar-links li a i {
      font-size: 24px;
      margin-bottom: 8px;
      margin-right: 0;
      width: auto;
      height: 30px;
      display: flex;
      align-items: center;
      justify-content: center;
      transition: all 0.2s ease;
    }

    .navbar-links li a:hover i {
      transform: scale(1.2);
      color: var(--accent-color);
    }

    .navbar-footer {
      text-align: center;
      font-size: 12px;
      color: var(--secondary-text);
      padding-top: 15px;
      border-top: 1px solid var(--server-select-border);
    }

    .power-button-container.connecting {
      border-color: var(--warning-color, #FF9500);
    }

    .power-button-container.stopping {
      border-color: #111;
      animation: boom-orange-border 0.6s ease-out;
    }

    .power-button-container.connected {
      border-color: var(--success-color);
      animation: pulse-green-border 1.5s infinite;
    }

    .power-button-container.error {
      border-color: var(--error-color, #FF3B30);
    }

    @keyframes pulse-green-border {
      0% {
        box-shadow: 0 0 0 0 rgba(var(--success-color-rgb), 0.7);
      }

      70% {
        box-shadow: 0 0 0 20px rgba(var(--success-color-rgb), 0);
      }

      100% {
        box-shadow: 0 0 0 0 rgba(var(--success-color-rgb), 0);
      }
    }

    @keyframes boom-orange-border {
      0% {
        box-shadow: 0 0 0 0px rgba(255, 149, 0, 0.8);
      }

      100% {
        box-shadow: 0 0 0 40px rgba(255, 149, 0, 0);
      }
    }

    @keyframes pulse-dot {
      0% {
        box-shadow: 0 0 0 0 rgba(var(--success-color-rgb), 0.7);
      }

      70% {
        box-shadow: 0 0 0 6px rgba(var(--success-color-rgb), 0);
      }

      100% {
        box-shadow: 0 0 0 0 rgba(var(--success-color-rgb), 0);
      }
    }

    /* Modal styles */
    .modal {
      display: none;
      position: fixed;
      z-index: 1002;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      overflow: auto;
      background-color: rgba(30, 30, 30, 0.5);
      backdrop-filter: blur(4px);
    }

    .modal.show {
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .modal-content {
      background-color: var(--phone-bg);
      color: var(--primary-text);
      border: 1px solid var(--server-select-border);
      border-radius: 12px;
      padding: 20px 30px 30px;
      position: relative;
      width: 90%;
      max-width: 380px;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
      animation: fadeInModal 0.4s ease-out;
      overflow: hidden;
      z-index: 2;
    }

    /* Estilo específico para o modal de verificar usuário */
    #checkUserModal .modal-content {
      margin: 50px;
    }

    .modal-content::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background-image: url('https://i.pinimg.com/736x/19/0f/10/190f10fafa504ad21486c9ced6161349.jpg');
      background-repeat: no-repeat;
      background-position: center;
      background-size: cover;
      opacity: var(--world-map-opacity);
      z-index: 0;
      transition: opacity 0.3s ease;
    }

    @keyframes fadeInModal {
      from {
        transform: translateY(20px) scale(0.98);
        opacity: 0;
      }

      to {
        transform: translateY(0) scale(1);
        opacity: 1;
      }
    }

    .modal-header {
      border-bottom: none;
      padding: 0;
      margin-top: 30px;
      margin-bottom: 25px;
      text-align: center;
      position: relative;
      z-index: 1;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    /* Estilos específicos para o modal DragonLogin */
    #dragonLoginModal .modal-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 16px;
      padding-bottom: 16px;
      border-bottom: 1px solid var(--server-select-border);
    }

    .modal-title {
      font-family: var(--font-heading, 'Poppins'), sans-serif;
      font-size: 27px;
      color: var(--primary-text);
      position: relative;
      z-index: 1;
      text-shadow: 0 0 10px rgba(var(--accent-color-rgb), 0.3);
    }

    #dragonLoginModal .modal-title {
      font-family: 'Poppins', sans-serif;
      font-size: 20px;
    }

    .modal-title .kanji {
      color: var(--accent-color);
    }

    .modal-close {
      position: absolute;
      top: 15px;
      right: 15px;
      z-index: 3;
      color: var(--secondary-text);
      font-size: 24px;
      background: none;
      border: none;
      cursor: pointer;
      padding: 0;
      line-height: 1;
    }

    .modal-body {
      position: relative;
      z-index: 1;
      max-height: 60vh;
      overflow-y: auto;
    }

    .modal-footer {
      padding-top: 16px;
      border-top: 1px solid var(--server-select-border);
      margin-top: 16px;
      display: flex;
      justify-content: flex-end;
      gap: 12px;
      position: relative;
      z-index: 1;
    }

    /* Specific modal adjustments */
    #configModal .modal-content {
      max-width: 500px;
      padding: 15px;
      margin: 10px;
      background-color: rgba(var(--body-bg-rgb), 0.7);
      backdrop-filter: blur(15px);
      border: 1px solid var(--server-select-border);
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.25);
      border-radius: 20px;
    }

    #configModal .modal-content::before {
      display: none;
      /* Remove a imagem de fundo */
    }

    #configModal .modal-header {
      margin-top: 0;
      margin-bottom: 16px;
      padding-bottom: 16px;
      border-bottom: 1px solid var(--server-select-border);
      position: relative;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    #configModal .modal-title {
      font-size: 20px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background: linear-gradient(90deg, var(--accent-color), color-mix(in srgb, var(--accent-color) 70%, #ffffff));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    #configModal .modal-title::before {
      content: "";
      display: inline-block;
      width: 20px;
      height: 20px;
      background-color: var(--accent-color);
      mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M12 15V3m0 12l-4-4m4 4l4-4M2 17l.621 2.485A2 2 0 0 0 4.561 21h14.878a2 2 0 0 0 1.94-1.515L22 17'%3E%3C/path%3E%3C/svg%3E");
      mask-size: cover;
      mask-position: center;
      mask-repeat: no-repeat;
    }

    #configModal .modal-close {
      position: absolute;
      top: -8px;
      right: -5px;
      font-size: 24px;
      cursor: pointer;
      color: var(--secondary-text);
      transition: all 0.2s ease;
      width: 32px;
      height: 32px;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 50%;
      background: transparent;
      border: none;
      padding: 0;
      z-index: 10;
    }

    #configModal .modal-close:hover {
      color: var(--accent-color);
      background-color: rgba(var(--accent-color-rgb), 0.1);
      transform: rotate(90deg);
    }

    #configModal .bg-category {
      font-family: 'Poppins', sans-serif;
      font-weight: 600;
      font-size: 1.1rem;
      margin: 20px 0 10px;
      padding-bottom: 5px;
      border-bottom: 2px solid var(--accent-color);
      color: var(--accent-color);
      position: relative;
      padding-left: 10px;
    }

    #configModal .bg-category::before {
      content: "";
      position: absolute;
      left: 0;
      top: 50%;
      transform: translateY(-50%);
      width: 4px;
      height: 16px;
      background-color: var(--accent-color);
      border-radius: 2px;
    }

    #configModal .modal-body {
      max-height: 60vh;
      overflow-y: auto;
      -ms-overflow-style: none;
      /* IE and Edge */
      scrollbar-width: none;
      /* Firefox */
      flex-grow: 1;
    }

    #configModal .modal-body::-webkit-scrollbar {
      display: none;
      /* Chrome, Safari, Opera */
    }

    @keyframes fadeInConfig {
      from {
        opacity: 0;
        transform: translateY(10px);
      }

      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    #configModal .bg-config {
      transition: all 0.2s ease-in-out;
      border-radius: 12px;
      overflow: hidden;
      border: 1px solid var(--server-select-border);
      position: relative;
      background-color: rgba(var(--body-bg-rgb), 0.3);
    }

    #configModal .bg-config:hover {
      border-color: var(--accent-color);
      background: rgba(var(--accent-color-rgb), 0.08);
      transform: translateX(4px);
    }

    #configModal .bg-config.selected {
      background: rgba(var(--accent-color-rgb), 0.1);
      border-color: var(--accent-color);
      box-shadow: 0 5px 15px rgba(var(--accent-color-rgb), 0.2);
    }

    #configModal .bg-config.selected .config-mode::after {
      content: " ✓";
      color: var(--accent-color);
      font-weight: bold;
      margin-left: 4px;
    }

    #configModal .category-filter {
      border-bottom: none;
      padding: 5px;
      margin-bottom: 15px;
      justify-content: center;
      display: flex;
      flex-direction: row;
      gap: 15px;
      overflow-x: auto;
      overflow-y: hidden;
      scroll-behavior: smooth;
      -webkit-overflow-scrolling: touch;
      flex-wrap: nowrap;
      -ms-overflow-style: none;
      /* IE and Edge */
      scrollbar-width: none;
      /* Firefox */
    }

    #configModal .category-filter::-webkit-scrollbar {
      display: none;
      /* Chrome, Safari, Opera */
    }

    #configModal .category-chip {
      background: transparent;
      color: var(--secondary-text);
      font-size: 13px;
      font-weight: 500;
      padding: 5px 12px;
      border-radius: 20px;
      border: 1px solid rgba(var(--accent-color-rgb), 0.2);
      transition: all 0.3s;
      white-space: nowrap;
      cursor: pointer;
    }

    #configModal .category-chip.active {
      background: var(--accent-color);
      color: white;
      box-shadow: 0 2px 8px rgba(var(--accent-color-rgb), 0.4);
    }

    #configModal .category-chip:hover:not(.active) {
      background: rgba(var(--accent-color-rgb), 0.1);
      border-color: rgba(var(--accent-color-rgb), 0.5);
      transform: translateY(-1px);
    }

    #autoConnectModal .modal-content {
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 90%;
      max-width: 420px;
      height: auto;
      max-height: 88vh;
      background-color: rgba(var(--body-bg-rgb), 0.7);
      backdrop-filter: blur(15px);
      border: 1px solid var(--server-select-border);
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.25);
      border-radius: 20px;
      padding: 22px 25px;
      margin: 0;
      overflow-y: auto;
      will-change: transform, opacity;
    }

    #autoConnectModal .modal-header {
      margin-top: 0;
    }

    #autoConnectModal .modal-content::before {
      display: none;
      /* Remove a imagem de fundo */
    }

    #autoConnectModal .modal-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding-bottom: 16px;
      border-bottom: 1px solid var(--server-select-border);
      margin-bottom: 16px;
      position: relative;
    }

    #autoConnectModal .modal-title {
      margin: 0;
      font-size: 20px;
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(90deg, var(--accent-color), color-mix(in srgb, var(--accent-color) 70%, #ffffff));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    #autoConnectModal .modal-title::before {
      content: "";
      display: inline-block;
      width: 20px;
      height: 20px;
      background-color: var(--accent-color);
      mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M13 2L3 14h9l-1 8 10-12h-9l1-8z'%3E%3C/path%3E%3C/svg%3E");
      mask-size: cover;
      mask-position: center;
      mask-repeat: no-repeat;
    }

    #autoConnectModal .modal-body {
      flex-grow: 1;
      overflow-y: auto;
      -ms-overflow-style: none;
      /* IE and Edge */
      scrollbar-width: none;
      /* Firefox */
    }

    #autoConnectModal .modal-body::-webkit-scrollbar {
      display: none;
      /* Chrome, Safari, Opera */
    }

    #autoConnectModal #first-config-name {
      background: rgba(var(--body-bg-rgb), 0.3);
      padding: 12px;
      border-radius: 12px;
      margin-top: 12px;
      text-align: center;
      font-weight: 600;
      color: var(--accent-color);
      border: 1px dashed rgba(var(--accent-color-rgb), 0.3);
    }

    #autoConnectModal #auto-connect-logs {
      margin-top: 20px;
      border-radius: 12px;
      padding: 15px;
      max-height: 150px;
      overflow-y: auto;
      font-family: monospace;
      font-size: 12px;
      line-height: 1.5;
      color: var(--secondary-text);
      background-color: rgba(var(--body-bg-rgb), 0.3);
      border: 1px solid var(--server-select-border);
    }

    #loggerModal .modal-content {
      max-width: 500px;
    }

    /* Button styles for modals */
    .button {
      padding: 10px 20px;
      border-radius: 8px;
      font-family: var(--font-heading, 'Poppins'), sans-serif;
      font-size: 14px;
      font-weight: 600;
      letter-spacing: 0.5px;
      border: none;
      cursor: pointer;
      transition: all 0.3s ease;
      position: relative;
      overflow: hidden;
    }

    .button-primary {
      background: var(--accent-color);
      color: white;
      box-shadow: 0 4px 15px rgba(var(--accent-color-rgb), 0.3);
    }

    .button-primary:hover {
      transform: translateY(-2px);
      box-shadow: 0 5px 15px rgba(var(--accent-color-rgb), 0.5);
      filter: brightness(1.1);
    }

    .button-primary:active {
      transform: translateY(1px);
      box-shadow: 0 2px 8px rgba(var(--accent-color-rgb), 0.3);
    }

    .button-primary.stopping {
      background-color: var(--error-color, #FF3B30);
      box-shadow: 0 4px 15px rgba(255, 59, 48, 0.3);
    }

    .button-primary.stopping:hover {
      box-shadow: 0 5px 15px rgba(255, 59, 48, 0.5);
      filter: brightness(1.1);
    }

    .button-secondary {
      background: rgba(var(--body-bg-rgb), 0.5);
      color: var(--primary-text);
      border: 1px solid var(--server-select-border);
    }

    .button-secondary:hover {
      background: rgba(var(--body-bg-rgb), 0.7);
      transform: translateY(-2px);
    }

    .button-secondary:active {
      transform: translateY(1px);
    }

    /* Media query removida para evitar que modais ocupem tela cheia */

    .category-filter {
      display: flex;
      gap: 10px;
      padding-bottom: 15px;
      margin-bottom: 10px;
      border-bottom: 1px solid var(--server-select-border);
      overflow-x: auto;
      -ms-overflow-style: none;
      /* IE and Edge */
      scrollbar-width: none;
      /* Firefox */
    }

    .category-filter::-webkit-scrollbar {
      display: none;
      /* Chrome, Safari, Opera */
    }

    .category-chip {
      padding: 6px 14px;
      border-radius: 16px;
      background: var(--body-bg);
      color: var(--secondary-text);
      font-size: 14px;
      font-weight: 500;
      cursor: pointer;
      white-space: nowrap;
      border: 1px solid var(--server-select-border);
      transition: all 0.2s;
    }

    .category-chip.active,
    .category-chip:hover {
      background: var(--accent-color);
      color: white;
      border-color: var(--accent-color);
    }

    .bg-category {
      font-family: 'Poppins', sans-serif;
      font-weight: 600;
      font-size: 1.1rem;
      margin: 20px 0 10px;
      padding-bottom: 5px;
      border-bottom: 2px solid var(--accent-color);
      color: var(--accent-color);
    }

    .bg-config {
      display: grid;
      grid-template-columns: 32px 1fr auto;
      align-items: center;
      gap: 12px;
      padding: 12px;
      margin: 8px 0;
      background: var(--body-bg);
      border: 1px solid var(--server-select-border);
      border-radius: 8px;
      cursor: pointer;
      transition: all 0.2s ease-in-out;
    }

    .bg-config:hover {
      border-color: var(--accent-color);
      background: var(--phone-bg);
      transform: translateX(4px);
    }

    .bg-config img {
      width: 32px;
      height: 32px;
      border-radius: 50%;
    }

    .config-info {
      flex-grow: 1;
      min-width: 0;
      display: flex;
      flex-direction: column;
    }

    .config-name {
      font-weight: 500;
      word-wrap: break-word;
      overflow-wrap: break-word;
    }

    .config-description {
      font-size: 0.8rem;
      color: var(--secondary-text);
      word-wrap: break-word;
      overflow-wrap: break-word;
    }

    .config-mode {
      font-size: 0.8rem;
      color: var(--secondary-text);
      background: var(--server-select-border);
      padding: 4px 8px;
      border-radius: 12px;
      text-align: right;
    }

    .toast {
      visibility: hidden;
      opacity: 0;
      position: fixed;
      left: 50%;
      bottom: 30px;
      transform: translateX(-50%);
      min-width: 250px;
      background: var(--phone-bg);
      color: var(--primary-text);
      text-align: center;
      border-radius: 8px;
      padding: 16px;
      z-index: 1003;
      /* Higher than modal */
      font-size: 15px;
      transition: opacity 0.5s ease, visibility 0.5s ease;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      border: 1px solid var(--server-select-border);
    }

    .toast.show {
      visibility: visible;
      opacity: 1;
    }

    #auto-connect-logs {
      margin-top: 16px;
      background: var(--body-bg);
      border-radius: 8px;
      padding: 10px;
      height: 150px;
      overflow-y: auto;
      font-family: monospace;
      font-size: 12px;
      line-height: 1.5;
      color: var(--secondary-text);
      border: 1px solid var(--server-select-border);
    }

    /* Dragon Login Modal Styles */
    #dragonLoginModal .modal-content {
      background-color: var(--phone-bg);
      color: var(--primary-text);
      border: 1px solid var(--server-select-border);
      border-radius: 12px;
      padding: 24px;
      margin: 10px;
      position: relative;
      max-width: 380px;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
      animation: fadeInModal 0.4s ease-out;
      overflow: hidden;
    }

    body.light-theme #dragonLoginModal .modal-content {
      background-color: var(--phone-bg);
      color: var(--primary-text);
      border-color: var(--server-select-border);
      z-index: 2;
    }

    #dragonLoginModal .modal-content::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background-image: url('https://i.pinimg.com/736x/19/0f/10/190f10fafa504ad21486c9ced6161349.jpg');
      background-repeat: no-repeat;
      background-position: center;
      background-size: cover;
      opacity: var(--world-map-opacity);
      z-index: 0;
      transition: opacity 0.3s ease;
    }

    @keyframes fadeInModal {
      from {
        transform: translateY(20px) scale(0.98);
        opacity: 0;
      }

      to {
        transform: translateY(0) scale(1);
        opacity: 1;
      }
    }

    #dragonLoginModal .modal-avatar {
      width: 137px;
      height: 137px;
      border-radius: 50%;
      border: 3px solid var(--accent-color);
      position: absolute;
      top: 105px;
      left: 69%;
      transform: translate(-50%, -50%);
      background-color: var(--phone-bg);
      padding: 5px;
      z-index: 2;
      box-shadow: 0 0 20px rgba(var(--accent-color-rgb), 0.5);
    }

    body.light-theme #dragonLoginModal .modal-avatar {
      background-color: var(--phone-bg);
    }

    #dragonLoginModal .modal-avatar img {
      width: 100%;
      height: 100%;
      border-radius: 50%;
      object-fit: cover;
    }

    #dragonLoginModal .modal-header {
      border-bottom: none;
      padding: 0;
      margin-top: 30px;
      margin-bottom: 25px;
      text-align: center;
      position: relative;
      z-index: 1;
    }

    #dragonLoginModal .modal-title {
      font-family: var(--font-heading, 'Poppins'), sans-serif;
      font-size: 27px;
      color: var(--primary-text);
      position: relative;
      z-index: 1;
      text-shadow: 0 0 10px rgba(var(--accent-color-rgb), 0.3);
    }

    #dragonLoginModal .modal-title .kanji {
      color: var(--accent-color);
    }

    body.light-theme #dragonLoginModal .modal-title {
      color: var(--primary-text);
    }

    #dragonLoginModal .modal-close {
      position: absolute;
      top: 15px;
      right: 15px;
      z-index: 3;
      color: var(--secondary-text);
      font-size: 24px;
      background: none;
      border: none;
      cursor: pointer;
    }

    #dragonLoginModal .input-group {
      margin-bottom: 20px;
      position: relative;
      z-index: 1;
    }

    #dragonLoginModal .input-group input {
      background-color: rgba(var(--body-bg-rgb, 10, 10, 16), 0.7);
      backdrop-filter: blur(5px);
      border: 1px solid var(--server-select-border);
      color: var(--primary-text);
      padding: 15px;
      font-size: 15px;
      letter-spacing: 0.5px;
      border-radius: 8px;
      width: 100%;
      font-family: 'Roboto', sans-serif;
      transition: all 0.3s ease;
      box-sizing: border-box;
    }

    body.light-theme #dragonLoginModal .input-group input {
      background-color: rgba(var(--body-bg-rgb, 233, 235, 242), 0.7);
      border-color: var(--server-select-border);
      color: var(--primary-text);
    }

    #dragonLoginModal .input-group input:focus {
      border-color: var(--accent-color);
      box-shadow: 0 0 15px rgba(var(--accent-color-rgb), 0.4);
      outline: none;
    }

    #dragonLoginModal .password-toggle {
      position: absolute;
      right: 15px;
      top: 50%;
      transform: translateY(-50%);
      cursor: pointer;
      color: var(--secondary-text);
      z-index: 3;
    }

    #dragonLoginModal .dragon-button {
      width: 100%;
      padding: 14px;
      border-radius: 8px;
      background: var(--accent-color);
      color: white;
      font-family: var(--font-heading, 'Poppins'), sans-serif;
      font-size: 16px;
      font-weight: 600;
      letter-spacing: 0.5px;
      border: none;
      cursor: pointer;
      transition: all 0.3s ease;
      text-transform: uppercase;
      position: relative;
      overflow: hidden;
      z-index: 1;
      box-shadow: 0 4px 15px rgba(var(--accent-color-rgb), 0.3);
    }

    #dragonLoginModal .dragon-button::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
      transition: 0.5s;
    }

    #dragonLoginModal .dragon-button:hover::before {
      left: 100%;
    }

    #dragonLoginModal .dragon-button:hover {
      transform: translateY(-2px);
      box-shadow: 0 5px 15px rgba(var(--accent-color-rgb), 0.5);
      filter: brightness(1.1);
    }

    #dragonLoginModal .dragon-button:active {
      transform: translateY(1px);
      box-shadow: 0 2px 8px rgba(var(--accent-color-rgb), 0.3);
    }

    .main-logs-container {
      display: none;
      width: 100%;
      height: 140px;
      background: rgba(var(--body-bg-rgb), 0.5);
      backdrop-filter: blur(4px);
      border: 1px solid var(--server-select-border);
      border-radius: 12px;
      margin-top: 20px;
      padding: 10px;
      overflow-y: auto;
      font-family: monospace;
      font-size: 11px;
      color: var(--secondary-text);
      line-height: 1.5;
      box-sizing: border-box;
      transition: all 0.3s ease;
      position: relative;
      z-index: 2;
      cursor: pointer;
      -ms-overflow-style: none !important;
      /* IE and Edge */
      scrollbar-width: none !important;
      /* Firefox */
    }

    .main-logs-container::-webkit-scrollbar {
      display: none !important;
      width: 0 !important;
      height: 0 !important;
    }

    .main-logs-container div {
      padding-bottom: 4px;
    }

    /* Estilos para o modal de logs expandido */
    #logs-modal-overlay {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.5);
      backdrop-filter: blur(3px);
      z-index: 1000;
      opacity: 0;
      visibility: hidden;
      transition: opacity 0.3s ease-in-out, visibility 0.3s ease-in-out;
      pointer-events: none;
    }

    #logs-expanded {
      position: fixed;
      top: 50%;
      left: 50%;
      height: auto;
      max-height: 80vh;
      width: 90%;
      max-width: 500px;
      background-color: var(--phone-bg);
      border: 1px solid rgba(var(--accent-color-rgb), 0.2);
      z-index: 1001;
      transform: translate(-150%, -50%);
      transition: transform 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
      display: flex;
      flex-direction: column;
      padding: 24px;
      box-sizing: border-box;
      border-radius: 16px;
      color: var(--primary-text);
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.2), 0 0 1px rgba(var(--accent-color-rgb), 0.3);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      opacity: 0;
      pointer-events: none;
    }

    body.logs-open #logs-expanded {
      transform: translate(-50%, -50%);
      opacity: 1;
      pointer-events: all;
    }

    body.logs-open #logs-modal-overlay {
      opacity: 1;
      visibility: visible;
      pointer-events: all;
    }

    body.logs-open .phone-mockup {
      filter: blur(2px);
      transition: filter 0.3s ease;
    }

    #logs-expanded .logs-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding-bottom: 16px;
      border-bottom: 1px solid rgba(var(--accent-color-rgb), 0.15);
      margin-bottom: 20px;
    }

    #logs-expanded .logs-header h3 {
      margin: 0;
      font-size: 20px;
      font-family: 'Poppins', sans-serif;
      color: var(--primary-text);
      position: relative;
      padding-left: 16px;
    }

    #logs-expanded .logs-header h3::before {
      content: "";
      position: absolute;
      left: 0;
      top: 50%;
      transform: translateY(-50%);
      width: 8px;
      height: 8px;
      background-color: var(--accent-color);
      border-radius: 50%;
      box-shadow: 0 0 10px rgba(var(--accent-color-rgb), 0.6);
      animation: pulse-dot 2s infinite;
    }

    #logs-expanded #close-logs {
      color: var(--secondary-text);
      background: rgba(var(--body-bg-rgb), 0.3);
      border: none;
      font-size: 24px;
      font-weight: 400;
      cursor: pointer;
      padding: 0;
      line-height: 1;
      width: 32px;
      height: 32px;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 50%;
      transition: all 0.2s ease;
    }

    #logs-expanded #close-logs:hover {
      color: var(--primary-text);
      background: rgba(var(--accent-color-rgb), 0.2);
      transform: rotate(90deg);
    }

    #logs-expanded .logs-content {
      flex-grow: 1;
      overflow-y: auto;
      max-height: 60vh;
      font-family: 'Roboto Mono', monospace;
      font-size: 12px;
      line-height: 1.6;
      color: var(--secondary-text);
      padding: 16px;
      background: rgba(var(--body-bg-rgb), 0.3);
      border-radius: 12px;
      border: 1px solid rgba(var(--accent-color-rgb), 0.1);
      scrollbar-width: thin;
      scrollbar-color: rgba(var(--accent-color-rgb), 0.3) transparent;
    }

    #logs-expanded .logs-content::-webkit-scrollbar {
      width: 6px;
    }

    #logs-expanded .logs-content::-webkit-scrollbar-track {
      background: transparent;
    }

    #logs-expanded .logs-content::-webkit-scrollbar-thumb {
      background-color: rgba(var(--accent-color-rgb), 0.3);
      border-radius: 20px;
      border: 2px solid transparent;
    }

    #logs-expanded .logs-content div {
      padding: 6px 8px;
      margin-bottom: 4px;
      border-radius: 6px;
      white-space: pre-wrap;
      overflow-wrap: break-word;
      background: rgba(var(--body-bg-rgb), 0.2);
      border-left: 2px solid rgba(var(--accent-color-rgb), 0.4);
      transition: background 0.2s ease;
    }

    #logs-expanded .logs-content div:hover {
      background: rgba(var(--body-bg-rgb), 0.4);
    }

    #logs-expanded .logs-content div:last-child {
      border-left: 2px solid var(--accent-color);
    }

    #logs-expanded .logs-footer {
      padding-top: 16px;
      border-top: 1px solid rgba(var(--accent-color-rgb), 0.15);
      margin-top: 20px;
      display: flex;
      justify-content: flex-end;
    }

    #logs-expanded .logs-footer button {
      padding: 10px 24px;
      border-radius: 50px;
      border: none;
      background: linear-gradient(135deg, var(--accent-color), rgba(var(--accent-color-rgb), 0.8));
      color: #ffffff;
      font-size: 14px;
      font-weight: 600;
      font-family: 'Poppins', sans-serif;
      cursor: pointer;
      transition: all 0.3s ease;
      box-shadow: 0 4px 12px rgba(var(--accent-color-rgb), 0.3);
      position: relative;
      overflow: hidden;
    }

    #logs-expanded .logs-footer button::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
      transition: 0.5s;
    }

    #logs-expanded .logs-footer button:hover::before {
      left: 100%;
    }

    #logs-expanded .logs-footer button:hover {
      transform: translateY(-3px);
      box-shadow: 0 6px 15px rgba(var(--accent-color-rgb), 0.4);
    }

    .user-info-container {
      display: none;
      width: 100%;
      background: rgba(var(--body-bg-rgb, 10, 10, 16), 0.5);
      backdrop-filter: blur(4px);
      border: 1px solid var(--server-select-border);
      border-radius: 12px;
      margin-top: 20px;
      padding: 15px;
      box-sizing: border-box;
      transition: all 0.3s ease;
      position: relative;
      z-index: 2;
    }

    .user-info-container .user-header {
      display: flex;
      align-items: center;
      margin-bottom: 12px;
      flex-wrap: wrap;
    }

    .user-info-container .user-avatar {
      width: 50px;
      height: 50px;
      border-radius: 50%;
      border: 2px solid var(--accent-color);
      margin-right: 12px;
      overflow: hidden;
    }

    .user-info-container .user-avatar img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .user-info-container .user-name {
      font-size: 16px;
      font-weight: 600;
      color: var(--primary-text);
      margin-bottom: 3px;
    }

    .user-info-container .user-status {
      font-size: 12px;
      color: var(--success-color, #34C759);
      display: flex;
      align-items: center;
    }

    .user-info-container .user-status .status-dot {
      width: 8px;
      height: 8px;
      background-color: currentColor;
      border-radius: 50%;
      margin-right: 6px;
      animation: pulse-dot 2s infinite;
    }

    .user-info-container .user-version {
      font-size: 11px;
      color: var(--secondary-text);
      background-color: rgba(var(--body-bg-rgb), 0.3);
      padding: 3px 8px;
      border-radius: 12px;
      margin-left: auto;
      align-self: flex-start;
    }

    .user-info-container .user-details {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 8px;
    }

    @media (max-height: 773px) {
      .user-info-container .user-details {
        display: flex;
        flex-wrap: nowrap;
        overflow-x: auto;
        gap: 12px;
        scroll-behavior: smooth;
        -webkit-overflow-scrolling: touch;
        padding: 5px 0;
        -ms-overflow-style: none !important;
        /* IE and Edge */
        scrollbar-width: none !important;
        /* Firefox */
      }

      .user-info-container .user-details::-webkit-scrollbar {
        display: none !important;
        /* Chrome, Safari, Opera */
        width: 0 !important;
        height: 0 !important;
      }

      /* Garantir que todos os elementos dentro do user-details também não mostrem scrollbar */
      .user-info-container .user-details * {
        -ms-overflow-style: none !important;
        scrollbar-width: none !important;
      }

      .user-info-container .user-details *::-webkit-scrollbar {
        display: none !important;
        width: 0 !important;
        height: 0 !important;
      }

      .user-info-container .user-details.dragging {
        cursor: grabbing;
        scroll-behavior: auto;
      }

      .user-info-container .detail-item {
        min-width: 140px;
        flex: 0 0 auto;
        cursor: grab;
        user-select: none;
        position: relative;
      }

      .user-info-container .detail-item::after {
        content: '';
        position: absolute;
        right: 8px;
        top: 8px;
        width: 12px;
        height: 12px;
        background-color: var(--accent-color);
        mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpolyline points='9 18 15 12 9 6'%3E%3C/polyline%3E%3C/svg%3E");
        mask-size: cover;
        opacity: 0.7;
      }
    }

    .user-info-container .detail-item {
      background-color: rgba(var(--body-bg-rgb, 10, 10, 16), 0.3);
      padding: 8px 10px;
      border-radius: 8px;
      font-size: 13px;
    }

    .user-info-container .detail-item .detail-label {
      font-size: 11px;
      color: var(--secondary-text);
      margin-bottom: 3px;
    }

    .user-info-container .detail-item .detail-value {
      color: var(--primary-text);
      font-weight: 500;
    }

    /* Estilos para carregamento e erro no user-info */
    .user-loading {
      text-align: center;
      padding: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100%;
    }

    .loading-spinner {
      width: 40px;
      height: 40px;
      border: 4px solid rgba(var(--accent-color-rgb), 0.2);
      border-radius: 50%;
      border-top: 4px solid var(--accent-color);
      animation: spin 1s linear infinite;
      margin-bottom: 15px;
    }

    @keyframes spin {
      0% {
        transform: rotate(0deg);
      }

      100% {
        transform: rotate(360deg);
      }
    }

    .user-error {
      text-align: center;
      padding: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
    }

    .user-error p {
      color: var(--secondary-text);
      margin-top: 0;
    }

    @media (max-width: 398px) {
      #dragonLoginModal .modal-avatar {
        top: 79px;
        left: 52%;
        width: 115px;
        height: 115px;
      }

      #dragonLoginModal .modal-title {
        position: absolute;
        top: 58px;
        left: 50%;
        transform: translateX(-50%);
        width: 100%;
      }

      #dragonLoginModal .modal-body {
        margin-top: 160px;
      }
    }

    @media (max-width: 550px) {
      body {
        display: block;
      }

      .phone-mockup {
        width: 100vw;
        height: 100vh;
        border-radius: 0;
        box-shadow: none;
      }

      .phone-mockup::before {
        background-position: center 202px;
      }

      body.navbar-open .phone-mockup {
        filter: blur(3px);
      }

      #side-navbar {
        max-height: 80vh;
      }

      .navbar-links li {
        min-width: 100px;
      }

      .navbar-links li a {
        height: 90px;
        padding: 3px;
        font-size: 13px;
      }

      .navbar-links li a i {
        font-size: 22px;
        margin-bottom: 5px;
      }

      /* Configurações de tela cheia para configModal removidas */
    }

    @media (max-width: 480px) {
      .bg-config {
        grid-template-columns: 32px 1fr;
        gap: 10px;
        padding: 12px;
      }

      .config-mode {
        grid-column: 1 / -1;
        text-align: left;
        margin-top: 8px;
        padding-top: 8px;
        border-top: 1px solid var(--server-select-border);
        background: transparent;
        border-radius: 0;
        padding-left: 0;
        padding-right: 0;
        padding-bottom: 0;
      }

      /* Ajustes responsivos para o modal de autoconexão */
      #autoConnectModal .modal-content {
        max-width: 92%;
        padding: 18px 17px;
      }

      #autoConnectModal .modal-header {
        padding-bottom: 12px;
        margin-bottom: 12px;
      }

      #autoConnectModal #auto-connect-logs {
        max-height: 120px;
      }
    }

    @media (max-height: 806px) {
      main.connected-state {
        overflow-y: auto;
        max-height: calc(100vh - 180px);
        -ms-overflow-style: none !important;
        /* IE and Edge */
        scrollbar-width: none !important;
        /* Firefox */
      }

      main.connected-state::-webkit-scrollbar {
        display: none !important;
        width: 0 !important;
        height: 0 !important;
      }
    }

    @media (max-height: 795px) {

      #side-navbar,
      #autoConnectModal .modal-content {
        padding: 10px 15px;
        max-height: 80vh;
      }

      .navbar-header,
      .navbar-profile {
        margin-bottom: 10px;
      }

      .navbar-header {
        padding-bottom: 10px;
      }

      .navbar-profile {
        padding: 10px 0;
      }

      .navbar-profile img {
        width: 60px;
        height: 60px;
        margin-bottom: 8px;
      }

      .navbar-links {
        margin: 8px 0;
      }

      .navbar-links li {
        min-width: 100px;
      }

      .navbar-links li a {
        height: 90px;
        padding: 3px;
        font-size: 13px;
      }

      .navbar-links li a i {
        font-size: 22px;
        margin-bottom: 5px;
      }

      .theme-picker-container {
        margin-top: 10px;
        padding: 0px 10px 30px 10px;
      }

      .navbar-footer {
        padding-top: 10px;
      }
    }

    /* Ajustes para telas muito pequenas */
    @media (max-width: 360px) {
      #autoConnectModal .modal-content {
        padding: 15px 18px;
        max-height: 90vh;
      }

      #autoConnectModal .modal-header {
        padding-bottom: 10px;
        margin-bottom: 8px;
      }

      #autoConnectModal .modal-title {
        font-size: 18px;
      }

      #autoConnectModal #first-config-name {
        margin: 10px 0 15px;
        padding: 10px;
      }

      #autoConnectModal #auto-connect-logs {
        margin-top: 15px;
        padding: 10px;
        height: 120px;
        font-size: 11px;
      }

      #autoConnectModal .category-filter {
        gap: 8px;
        margin-bottom: 10px;
      }

      #autoConnectModal .category-chip {
        padding: 4px 10px;
        font-size: 12px;
      }

      #autoConnectModal .modal-footer {
        margin-top: 15px;
        padding-top: 15px;
      }

      #autoConnectModal .button {
        padding: 8px 15px;
        font-size: 13px;
      }
    }

    @media (max-height: 773px) {
      main.connected-state .power-button-container {
        margin-top: 27px;
      }

      .main-logs-container {
        height: 130px;
        margin-top: 15px;
      }
    }

    @media (max-height: 755px) {
      main.connected-state .power-button-container {
        margin-top: 49px;
      }

      .main-logs-container {
        height: 120px;
        margin-top: 13px;
      }
    }

    @media (max-height: 730px) {
      main.connected-state .power-button-container {
        margin-top: 72px;
      }

      .main-logs-container {
        height: 110px;
        margin-top: 10px;
      }
    }

    @media (max-height: 670px) {
      .main-logs-container {
        height: 90px;
        margin-top: 8px;
        font-size: 10px;
      }

      .connect-text {
        margin-bottom: 3px;
      }
    }

    @media (max-width: 324px) {
      header {
        flex-wrap: wrap;
        justify-content: center;
        gap: 10px;
        padding-top: 10px;
        padding-bottom: 0;
      }

      header h1 {
        order: 1;
        flex-grow: 0;
        width: 100%;
      }

      #open-nav {
        margin-right: 50px;
      }
    }

    .theme-picker-container {
      padding: 0px 10px 30px 10px;
      margin-top: 20px;
      margin-bottom: auto;
      border-top: 1px solid var(--server-select-border);
      text-align: center;
    }

    .theme-picker-title {
      font-family: 'Poppins', sans-serif;
      font-size: 1rem;
      color: var(--secondary-text);
      margin-bottom: 12px;
      text-align: center;
      font-weight: 500;
    }

    .theme-swatches {
      display: flex;
      gap: 16px;
      justify-content: center;
    }

    .theme-swatch {
      width: 28px;
      height: 28px;
      border-radius: 50%;
      cursor: pointer;
      border: 2px solid transparent;
      transition: all 0.2s ease;
    }

    .theme-swatch.active,
    .theme-swatch:hover {
      transform: scale(1.1);
      border-color: var(--primary-text);
    }

    body.light-theme .user-info-container {
      background: rgba(var(--body-bg-rgb), 0.6);
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
      border-color: rgba(0, 0, 0, 0.05);
    }

    body.light-theme .user-info-container .detail-item {
      background-color: rgba(255, 255, 255, 0.7);
      box-shadow: 0 1px 3px rgba(0, 0, 0, 0.03);
    }

    body.light-theme .connect-text.connected-status {
      background-color: rgba(var(--success-color-rgb), 0.08);
      border-color: rgba(var(--success-color-rgb), 0.2);
      box-shadow: 0 2px 8px rgba(var(--success-color-rgb), 0.08);
    }

    body.light-theme .modal-content {
      background-color: rgba(250, 251, 252, 0.95);
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.08);
    }

    body.light-theme .button-secondary {
      background: rgba(var(--body-bg-rgb), 0.7);
      border-color: rgba(0, 0, 0, 0.05);
    }

    body.light-theme .server-select {
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.03);
    }

    /* Estilos para o #configModal no tema claro */
    body.light-theme #configModal .modal-content {
      background-color: var(--phone-bg);
      backdrop-filter: none;
      box-shadow: 0 5px 25px rgba(0, 0, 0, 0.1);
      border-color: #e9ecef;
    }

    body.light-theme #configModal .modal-header {
      border-bottom-color: #dee2e6;
    }

    body.light-theme #configModal .category-chip {
      background-color: #e9ecef;
      color: var(--primary-text);
      border-color: transparent;
    }

    body.light-theme #configModal .category-chip:hover:not(.active) {
      background: rgba(var(--accent-color-rgb), 0.15);
      border-color: transparent;
      color: var(--accent-color);
    }

    body.light-theme #configModal .category-chip.active {
      background-color: var(--accent-color);
      color: white;
      border-color: var(--accent-color);
      box-shadow: 0 2px 8px rgba(var(--accent-color-rgb), 0.3);
    }

    body.light-theme #configModal .bg-config {
      background-color: #fff;
      border: 1px solid #dee2e6;
    }

    body.light-theme #configModal .bg-config:hover {
      background-color: rgba(var(--accent-color-rgb), 0.05);
      border-color: rgba(var(--accent-color-rgb), 0.5);
      transform: translateX(2px);
    }

    body.light-theme #configModal .bg-config.selected {
      background-color: rgba(var(--accent-color-rgb), 0.1);
      border-color: var(--accent-color);
      box-shadow: 0 0 10px rgba(var(--accent-color-rgb), 0.15);
    }

    body.light-theme #configModal .bg-config.selected .config-mode::after {
      color: var(--accent-color);
    }

    /* Estilos para carregamento e erro no user-info */
    #autoConnectModal .category-chip {
      background: transparent;
      color: var(--secondary-text);
      font-size: 13px;
      font-weight: 500;
      padding: 5px 12px;
      border-radius: 20px;
      border: 1px solid rgba(var(--accent-color-rgb), 0.2);
      transition: all 0.3s;
    }

    #autoConnectModal .category-chip.active {
      background: var(--accent-color);
      color: white;
      box-shadow: 0 2px 8px rgba(var(--accent-color-rgb), 0.4);
    }

    #autoConnectModal .category-chip:hover:not(.active) {
      background: rgba(var(--accent-color-rgb), 0.1);
      border-color: rgba(var(--accent-color-rgb), 0.5);
      transform: translateY(-1px);
    }

    #autoConnectModal .modal-close {
      position: absolute;
      top: -8px;
      right: -5px;
      font-size: 24px;
      cursor: pointer;
      color: var(--secondary-text);
      transition: all 0.2s ease;
      width: 32px;
      height: 32px;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 50%;
      background: transparent;
      border: none;
      padding: 0;
      z-index: 10;
    }

    #autoConnectModal .modal-close:hover {
      color: var(--accent-color);
      background-color: rgba(var(--accent-color-rgb), 0.1);
      transform: rotate(90deg);
    }

    #autoConnectModal #auto-connect-start-btn {
      background: var(--accent-color);
      color: white;
      box-shadow: 0 4px 15px rgba(var(--accent-color-rgb), 0.3);
      border: none;
      padding: 10px 20px;
      font-weight: 600;
    }

    #autoConnectModal #auto-connect-start-btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 5px 15px rgba(var(--accent-color-rgb), 0.5);
      filter: brightness(1.1);
    }

    #autoConnectModal .category-filter {
      border-bottom: none;
      padding: 5px;
      margin-bottom: 15px;
      justify-content: flex-start;
      display: flex;
      flex-direction: row;
      gap: 15px;
      overflow-x: auto;
      overflow-y: hidden;
      scroll-behavior: smooth;
      -webkit-overflow-scrolling: touch;
      flex-wrap: nowrap;
      -ms-overflow-style: none;
      /* IE and Edge */
      scrollbar-width: none;
      /* Firefox */
    }

    #autoConnectModal .category-filter::-webkit-scrollbar {
      display: none;
      /* Chrome, Safari, Opera */
    }

    /* Button styles for modals */
    #configModal .bg-config.selected {
      background: rgba(var(--accent-color-rgb), 0.1);
      border-color: var(--accent-color);
      box-shadow: 0 2px 8px rgba(var(--accent-color-rgb), 0.2);
    }

    body.light-theme #configModal .bg-config.selected .config-mode::after {
      color: var(--accent-color);
    }

    /* Estilos para o #autoConnectModal no tema claro */
    body.light-theme #autoConnectModal .modal-content {
      background-color: var(--phone-bg);
      backdrop-filter: none;
      box-shadow: 0 5px 25px rgba(0, 0, 0, 0.1);
      border-color: #e9ecef;
      border-width: 1px;
    }

    body.light-theme #autoConnectModal .modal-header,
    body.light-theme #autoConnectModal .modal-footer {
      border-color: #dee2e6;
    }

    body.light-theme #autoConnectModal p {
      color: var(--secondary-text);
    }

    body.light-theme #autoConnectModal .category-chip {
      background-color: #e9ecef;
      color: var(--primary-text);
      border-color: transparent;
    }

    body.light-theme #autoConnectModal .category-chip:hover:not(.active) {
      background: rgba(var(--accent-color-rgb), 0.15);
      color: var(--accent-color);
    }

    body.light-theme #autoConnectModal .category-chip.active {
      background-color: var(--accent-color);
      color: white;
      box-shadow: 0 2px 8px rgba(var(--accent-color-rgb), 0.3);
    }

    body.light-theme #autoConnectModal #first-config-name {
      background-color: #fff;
      border: 1px dashed #dee2e6;
      color: var(--primary-text);
    }

    body.light-theme #autoConnectModal #auto-connect-logs {
      background-color: #fff;
      border: 1px solid #dee2e6;
      color: var(--secondary-text);
    }

    /* Estilos para carregamento e erro no user-info */
    #autoConnectModal .category-chip {
      background: transparent;
      color: var(--secondary-text);
      font-size: 13px;
      font-weight: 500;
      padding: 5px 12px;
      border-radius: 20px;
      border: 1px solid rgba(var(--accent-color-rgb), 0.2);
      transition: all 0.3s;
    }

    #autoConnectModal .category-chip.active {
      background: var(--accent-color);
      color: white;
      box-shadow: 0 2px 8px rgba(var(--accent-color-rgb), 0.4);
    }

    #autoConnectModal .category-chip:hover:not(.active) {
      background: rgba(var(--accent-color-rgb), 0.1);
      border-color: rgba(var(--accent-color-rgb), 0.5);
      transform: translateY(-1px);
    }

    /* Melhorias no espaçamento interno e responsividade do conteúdo do modal */
    #autoConnectModal .modal-body {
      padding: 5px 0;
    }

    #autoConnectModal #first-config-name {
      margin: 18px 0 20px;
      padding: 15px;
      font-weight: 600;
      border-radius: 15px;
    }

    #autoConnectModal #auto-connect-logs {
      margin-top: 22px;
      height: 170px;
      max-height: 25vh;
      padding: 15px;
      font-size: 12.5px;
      line-height: 1.6;
      border-radius: 15px;
    }

    #autoConnectModal .modal-footer {
      margin-top: 20px;
      padding-top: 20px;
    }

    #autoConnectModal .category-chip.active {
      background: var(--accent-color);
      color: white;
      box-shadow: 0 2px 8px rgba(var(--accent-color-rgb), 0.4);
    }

    #hotspotModal .modal-content::before {
      display: none;
      /* Remove a imagem de fundo */
    }

    #autoConnectModal .modal-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding-bottom: 16px;
      border-bottom: 1px solid var(--server-select-border);
      margin-bottom: 16px;
      position: relative;
    }

    body.light-theme #autoConnectModal #auto-connect-logs {
      background-color: #fff;
      border: 1px solid #dee2e6;
      color: var(--secondary-text);
    }

    /* Estilos para o hotspotModal no tema claro */
    body.light-theme #hotspotModal .modal-content {
      background-color: var(--phone-bg);
      backdrop-filter: none;
      box-shadow: 0 5px 25px rgba(0, 0, 0, 0.1);
      border-color: #e9ecef;
    }

    body.light-theme #hotspotModal .modal-content::before {
      display: none;
      /* Remove a imagem de fundo no tema claro */
    }

    /* Animações para modais */
    @keyframes slideInModal {
      from {
        transform: translate(-150%, -50%);
        opacity: 0;
      }

      to {
        transform: translate(-50%, -50%);
        opacity: 1;
      }
    }

    @keyframes slideOutModal {
      from {
        transform: translate(-50%, -50%);
        opacity: 1;
      }

      to {
        transform: translate(-150%, -50%);
        opacity: 0;
      }
    }

    #hotspotModal .modal-content,
    #autoConnectModal .modal-content {
      animation: slideInModal 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
      opacity: 1;
    }

    #hotspotModal .modal-content.hiding,
    #autoConnectModal .modal-content.hiding {
      animation: slideOutModal 0.3s cubic-bezier(0.6, -0.28, 0.735, 0.045) forwards;
    }

    /* Estilos para carregamento e erro no user-info */
    .user-loading {
      text-align: center;
      padding: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100%;
    }

    .loading-spinner {
      width: 40px;
      height: 40px;
      border: 4px solid rgba(var(--accent-color-rgb), 0.2);
      border-radius: 50%;
      border-top: 4px solid var(--accent-color);
      animation: spin 1s linear infinite;
      margin-bottom: 15px;
    }

    @keyframes spin {
      0% {
        transform: rotate(0deg);
      }

      100% {
        transform: rotate(360deg);
      }
    }

    .user-error {
      text-align: center;
      padding: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
    }

    .user-error p {
      color: var(--secondary-text);
      margin-top: 0;
    }

    body.light-theme #autoConnectModal #auto-connect-logs {
      background-color: #fff;
      border: 1px solid #dee2e6;
      color: var(--secondary-text);
    }

    /* Remover highlight de toque em elementos interativos */
    a,
    button,
    .server-select,
    .power-button,
    .navbar-links li a,
    .bg-config,
    .category-chip,
    .theme-swatch,
    .server-action-icon {
      -webkit-tap-highlight-color: transparent;
      outline: none;
      -webkit-touch-callout: none;
      user-select: none;
    }

    button:focus,
    a:focus,
    .server-select:focus,
    .power-button:focus,
    .navbar-links li a:focus,
    .bg-config:focus,
    .category-chip:focus,
    .theme-swatch:focus,
    .server-action-icon:focus {
      outline: none;
    }

    input:focus {
      outline-color: var(--accent-color);
    }

    /* Estilos para o hotspotModal no tema claro */
    body.light-theme #hotspotModal .modal-content {
      background-color: var(--phone-bg);
      backdrop-filter: none;
      box-shadow: 0 5px 25px rgba(0, 0, 0, 0.1);
      border-color: #e9ecef;
    }

    /* 添加额外的浅色主题优化 */
    body.light-theme .phone-mockup {
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1), 0 0 0 1px rgba(0, 0, 0, 0.02);
    }

    body.light-theme .server-select {
      box-shadow: 0 3px 10px rgba(0, 0, 0, 0.03);
      border: 1px solid rgba(0, 0, 0, 0.04);
    }

    body.light-theme .notification {
      box-shadow: 0 4px 15px rgba(59, 130, 246, 0.15);
    }

    body.light-theme .power-button-container {
      background-color: #f1f5f9;
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.05), inset 0 0 15px rgba(0, 0, 0, 0.02);
    }

    body.light-theme .power-button {
      background-color: #ffffff;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
    }

    body.light-theme .power-button .fa-power-off {
      color: var(--power-icon-color);
    }

    body.light-theme .power-button:hover .fa-power-off {
      color: var(--power-icon-hover-color);
    }

    body.light-theme .user-info-container {
      background: #ffffff;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.03);
      border-color: rgba(0, 0, 0, 0.03);
    }

    body.light-theme .user-info-container .detail-item {
      background-color: #f8fafc;
      box-shadow: 0 1px 3px rgba(0, 0, 0, 0.02);
    }

    body.light-theme #side-navbar {
      background-color: rgba(255, 255, 255, 0.95);
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
    }

    body.light-theme .navbar-links li a {
      background-color: #f8fafc;
      border: 1px solid rgba(0, 0, 0, 0.03);
    }

    body.light-theme .navbar-links li a:hover {
      background-color: rgba(var(--accent-color-rgb), 0.05);
      border-color: rgba(var(--accent-color-rgb), 0.2);
      box-shadow: 0 5px 15px rgba(var(--accent-color-rgb), 0.1);
    }

    body.light-theme #configModal .modal-content,
    body.light-theme #autoConnectModal .modal-content,
    body.light-theme #dragonLoginModal .modal-content {
      background-color: rgba(255, 255, 255, 0.95);
      backdrop-filter: blur(15px);
      -webkit-backdrop-filter: blur(15px);
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08), 0 0 0 1px rgba(0, 0, 0, 0.02);
      border-color: rgba(0, 0, 0, 0.02);
    }

    body.light-theme #configModal .bg-config {
      background-color: #ffffff;
      border: 1px solid rgba(0, 0, 0, 0.03);
    }

    body.light-theme #configModal .bg-config:hover {
      background-color: rgba(var(--accent-color-rgb), 0.04);
      border-color: rgba(var(--accent-color-rgb), 0.15);
    }

    body.light-theme .power-button-container.connected {
      border-color: var(--success-color);
    }

    body.light-theme .connect-text.connected-status {
      background: linear-gradient(135deg, var(--success-color), color-mix(in srgb, var(--success-color) 70%, #5cffb1));
      color: white;
      box-shadow: 0 5px 15px rgba(var(--success-color-rgb), 0.15);
    }

    body.light-theme .app-version {
      color: var(--secondary-text);
      opacity: 0.7;
    }

    body.light-theme .button-primary {
      box-shadow: 0 4px 12px rgba(var(--accent-color-rgb), 0.15);
    }

    body.light-theme .button-primary:hover {
      box-shadow: 0 6px 15px rgba(var(--accent-color-rgb), 0.25);
    }

    body.light-theme .button-secondary {
      background-color: #f8fafc;
      border: 1px solid rgba(0, 0, 0, 0.04);
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.02);
    }

    body.light-theme .toast {
      background-color: rgba(255, 255, 255, 0.98);
      box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
      border: 1px solid rgba(0, 0, 0, 0.03);
    }
  </style>




</head>

<body class="dark-theme" data-color-theme="blue">
  <div id="navbar-overlay"></div>
  <nav id="side-navbar">
    <div class="navbar-header">
      <h3>Menu</h3>
      <i class="fas fa-times" id="close-nav"></i>
    </div>
    <div class="navbar-profile" id="nav-profile-section">
      <img src="https://i.postimg.cc/76Pqnycb/banner-sem-fundo.png" alt="User Avatar">
      <h4>Login</h4>
      <p>Clique para entrar</p>
    </div>
    <ul class="navbar-links" id="dynamic-navbar-links">
      <li><a href="#" id="nav-home"><i class="fas fa-home"></i> Início</a></li>
      <li><a href="#" id="nav-auto"><i class="fas fa-magic"></i> Auto Conexão</a></li>
      <li><a href="#" id="nav-update"><i class="fas fa-sync-alt"></i> Atualizar</a></li>
      <li><a href="#" id="nav-speedtest"><i class="fas fa-tachometer-alt"></i> Speedtest</a></li>
      <li><a href="#" id="nav-hostshare"><i class="fas fa-wifi"></i> Hostshare</a></li>
      <li><a href="#" id="nav-terms"><i class="fas fa-file-contract"></i> Termos</a></li>
    </ul>
    <div class="theme-picker-container">
      <h6 class="theme-picker-title">Temas de Cores</h6>
      <div class="theme-swatches">
        <div class="theme-swatch" data-theme="purple" style="background-color: #a044ff;"></div>
        <div class="theme-swatch active" data-theme="blue" style="background-color: #007AFF;"></div>
        <div class="theme-swatch" data-theme="green" style="background-color: #34d399;"></div>
        <div class="theme-swatch" data-theme="red" style="background-color: #C7384D;"></div>
      </div>
    </div>
    <div class="navbar-footer">
      <p>Versão <span id="navbar-version">3.0.0</span></p>
    </div>
  </nav>

  <div class="phone-mockup" style="--main-bg-image: url('https://i.ibb.co/8nyJHdKJ/photo-2025-07-08-14-33-31.jpg'); --main-bg-position-y: 180px;">
    <header>
      <i class="fas fa-bars" id="open-nav"></i>
      <h1>SOUZA<span class="kanji">NET</span> </h1>
      <i class="fas fa-sun" id="theme-toggle"></i>
    </header>

    <div class="notification">
      <p>Navegue com total liberdade.</p>
    </div>

    <div class="server-select">
      <div class="server-info">
        <img src="https://cdn-icons-png.flaticon.com/128/4625/4625178.png" alt="Bandeira do Brasil">
        <div>
          <span>Servidor Brasileiro</span>
          <small>Servidor otimizado</small>
        </div>
      </div>
      <div class="server-actions">
        <svg id="auto-connect-icon" xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="server-action-icon">
          <path d="M13 2L3 14h9l-1 8 10-12h-9l1-8z"></path>
        </svg>
        <i class="fas fa-chevron-down"></i>
      </div>
    </div>

    <main>
      <div class="power-button-container">
        <button class="power-button">
          <i class="fas fa-power-off"></i>
          <svg class="fa-power-off-fallback" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" width="65px" height="65px" fill="currentColor">
            <path d="M400 54.1c63 45 104 118.6 104 201.9 0 136.8-110.8 247.7-247.5 248C120 504.3 8.2 393 8 256.4 7.9 173.1 48.9 99.3 111.8 54.2c11.7-8.3 28-4.8 35 7.7L162.6 90c5.9 10.5 3.1 23.8-6.6 31-41.5 30.8-68 79.6-68 134.9-.1 92.3 74.5 168.1 168 168.1 91.6 0 168.6-74.2 168-169.1-.3-51.8-24.7-101.8-68.1-134-9.7-7.2-12.4-20.5-6.5-30.9l15.8-28.1c7-12.4 23.2-16.1 34.8-7.8zM296 264V24c0-13.3-10.7-24-24-24h-32c-13.3 0-24 10.7-24 24v240c0 13.3 10.7 24 24 24h32c13.3 0 24-10.7 24-24z"></path>
          </svg>
        </button>
      </div>
      <p class="connect-text">Clique aqui para conectar</p>
      <div id="main-screen-logs" class="main-logs-container" style="display: none;">
        <div><strong style="color:var(--accent-color)">[INFO]</strong> Mock log entry 1</div>
        <div><strong style="color:var(--accent-color)">[DEBUG]</strong> Another mock log entry</div>
      </div>
      <div id="user-info" class="user-info-container" style="display: none;">
        <div class="user-header">
          <div class="user-avatar">
            <img src="https://i.postimg.cc/76Pqnycb/banner-sem-fundo.png" alt="Avatar">
          </div>
          <div>
            <div class="user-name" id="info-username">Usuário</div>
            <div class="user-status">
              <div class="status-dot"></div>
              Conectado
            </div>
          </div>
          <div class="user-version" id="user-version-display">v3.0.0</div>
        </div>
        <div class="user-details">
          <div class="detail-item">
            <div class="detail-label">Ping</div>
            <div class="detail-value" id="info-ping">-- ms</div>
          </div>
          <div class="detail-item">
            <div class="detail-label">Validade</div>
            <div class="detail-value" id="info-days">--</div>
          </div>
          <div class="detail-item">
            <div class="detail-label">Conexões</div>
            <div class="detail-value" id="info-connections">0/0</div>
          </div>
          <div class="detail-item">
            <div class="detail-label">IP Local</div>
            <div class="detail-value" id="info-ip">0.0.0.0</div>
          </div>
        </div>
      </div>
      <div class="app-version" id="main-version" style="display: block;">v3.0.0</div>
    </main>
  </div>


  <div id="checkUserModal" class="modal">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title chk-title">Verificar Usuário</h5>
        <button class="modal-close" data-modal-id="checkUserModal">×</button>
      </div>
      <div class="modal-body chk-message">
      </div>
    </div>
  </div>

  <div id="configModal" class="modal">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Selecionar Configuração</h5>
        <button class="modal-close" data-modal-id="configModal">×</button>
      </div>
      <div class="modal-body config-body">

      </div>
    </div>
  </div>

  <div id="dragonLoginModal" class="modal">
    <div class="modal-content">
      <div class="modal-avatar">
        <img src="https://i.postimg.cc/76Pqnycb/banner-sem-fundo.png" alt="Dragon Avatar">
      </div>
      <button class="modal-close" data-modal-id="dragonLoginModal">×</button>
      <div class="modal-header">
        <h5 class="modal-title">Acesso <span class="kanji">SSH</span></h5>
      </div>
      <div class="modal-body">
        <div class="input-group">
          <input type="text" id="dragon-modal-username" placeholder="Usuário">
        </div>
        <div class="input-group">
          <input type="password" id="dragon-modal-password" placeholder="Senha">
          <i class="fas fa-eye password-toggle"></i>
        </div>
        <div class="input-group" id="uuid-group" style="display: none;">
          <input type="text" id="uuid" placeholder="UUID">
        </div>
        <button class="dragon-button" id="dragon-modal-login-btn">Entrar</button>
      </div>
    </div>
  </div>

  <div id="autoConnectModal" class="modal">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Conexão Automática</h5>
        <button class="modal-close" data-modal-id="autoConnectModal">×</button>
      </div>
      <div class="modal-body">
        <p style="color: var(--secondary-text); text-align: center;">O modo automático testará várias configurações até encontrar uma que conecte com sucesso.</p>
        <div id="auto-connect-category-filter" class="category-filter" style="margin-bottom: 16px; margin-top: 16px;"></div>
        <p style="color: var(--secondary-text); text-align: center; font-size: 13px; margin-bottom: 5px;">A primeira tentativa será com:</p>
        <div id="first-config-name" style="text-align: center; font-weight: 500;">
          Carregando...
        </div>
        <div id="auto-connect-logs">

        </div>
      </div>
      <div class="modal-footer" style="padding-top: 16px; border-top: 1px solid var(--server-select-border); margin-top: 16px; display: flex; justify-content: space-between; gap: 12px;">
        <button type="button" class="button button-secondary" id="auto-connect-cancel-btn">Cancelar</button>
        <button type="button" class="button button-primary" id="auto-connect-start-btn">Iniciar</button>
      </div>
    </div>
  </div>

  <div id="loggerModal" class="modal">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Logs</h5>
        <button type="button" class="modal-close" data-modal-id="loggerModal">×</button>
      </div>
      <div class="modal-body">
        <ul class="logger-content" style="list-style: none; padding: 0; font-family: monospace; font-size: 12px;">
          <li><strong style="color:var(--accent-color)">[INFO]</strong>: Mock log entry 1</li>
          <li><strong style="color:var(--accent-color)">[DEBUG]</strong>: Another mock log entry</li>
        </ul>
      </div>
      <div class="modal-footer" style="padding-top: 16px; border-top: 1px solid var(--server-select-border); margin-top: 16px;">
        <button type="button" class="button button-secondary clear-logger">Limpar</button>
      </div>
    </div>
  </div>

  <div id="hotspotModal" class="modal">
    <div class="modal-content" style="position: fixed; top: 50%; left: 50%; height: auto; max-height: 85vh; width: 90%; max-width: 360px; background-color: rgba(var(--body-bg-rgb), 0.86); backdrop-filter: blur(15px); z-index: 1001; transform: translate(-50%, -50%); display: flex; flex-direction: column; padding: 15px; box-sizing: border-box; border-radius: 20px; border: 1px solid var(--server-select-border); color: var(--primary-text); box-shadow: 0 10px 30px rgba(0,0,0,0.25); overflow: hidden; will-change: transform, opacity;">
      <div class="modal-header" style="display: flex; justify-content: space-between; align-items: center; padding-bottom: 20px; border-bottom: 1px solid var(--server-select-border); margin-bottom: 20px;">
        <h5 class="modal-title" style="margin: 0; font-size: 20px; font-family: 'Poppins', sans-serif; background: linear-gradient(90deg, var(--accent-color), color-mix(in srgb, var(--accent-color) 70%, #ffffff)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;">Roteador Hotspot</h5>
        <button class="modal-close" data-modal-id="hotspotModal" style="font-size: 24px; cursor: pointer; color: var(--secondary-text); transition: all 0.2s ease; width: 32px; height: 32px; display: flex; align-items: center; justify-content: center; border-radius: 50%; background: transparent; border: none; padding: 0;" onmouseover="this.style.color='var(--accent-color)'; this.style.backgroundColor='rgba(var(--accent-color-rgb), 0.1)'; this.style.transform='rotate(90deg)';" onmouseout="this.style.color='var(--secondary-text)'; this.style.backgroundColor='transparent'; this.style.transform='rotate(0deg)';">×</button>
      </div>
      <div class="modal-body" style="text-align: center; flex-grow: 1; overflow-y: auto; -ms-overflow-style: none; scrollbar-width: none;">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" style="width: 50px; height: 50px; color: var(--accent-color); margin-bottom: 16px;">
          <path d="M5.05 4.05a7 7 0 119.9 9.9L10 18.9l-4.95-4.95a7 7 0 010-9.9zM10 11a2 2 0 100-4 2 2 0 000 4z" clip-rule="evenodd"></path>
        </svg>
        <p style="color: var(--secondary-text-color); margin-bottom: 16px;">Compartilhe sua conexão VPN com outros dispositivos através de um ponto de acesso Wi-Fi.</p>
        <p style="color: var(--secondary-text-color); margin-bottom: 16px; background: rgba(var(--body-bg-rgb), 0.3); padding: 12px; border-radius: 12px; border: 1px solid var(--server-select-border);">
          A porta do hotspot será exibida em uma notificação.
        </p>
        <button class="button button-primary" id="toggleHotspotButton" style="width: 100%;">Ativar Hotspot</button>
      </div>
    </div>
  </div>

  <div id="toast" class="toast"></div>


  <div id="logs-modal-overlay"></div>
  <div id="logs-expanded">
    <div class="logs-header">
      <h3 class="modal-title">Logs</h3>
      <button type="button" class="modal-close" id="close-logs">×</button>
    </div>
    <div class="logs-content">
      <div><strong style="color:var(--accent-color)">[INFO]</strong>: Mock log entry 1</div>
      <div><strong style="color:var(--accent-color)">[DEBUG]</strong>: Another mock log entry</div>
    </div>
    <div class="logs-footer">
      <button type="button" class="button button-secondary" id="clear-logs-btn">Limpar</button>
    </div>
  </div>


  <div id="termsModal" class="modal">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Termos de Uso</h5>
        <button class="modal-close" data-modal-id="termsModal">×</button>
      </div>
      <div class="modal-body" style="max-height: 70vh; overflow-y: auto; padding: 0 10px;">
        <h3 style="text-align: center; margin-bottom: 20px;">📄 Termos de Uso — Internet Ilimitada com VPN</h3>
        <p style="text-align: center; color: var(--secondary-text); margin-bottom: 20px;">Souza NET<br>Última atualização: 08 de julho de 2025</p>
        <p>Bem-vindo ao serviço de Internet Ilimitada com VPN da Souza NET. Ao adquirir ou utilizar nosso serviço, você concorda com os termos e condições descritos abaixo.</p>

        <h4 style="color: var(--accent-color); margin-top: 20px; margin-bottom: 10px;">1. Objetivo do Serviço</h4>
        <p>A Souza NET oferece acesso à internet móvel com uso ilimitado de dados, utilizando uma conexão VPN segura e estável, com base em redes móveis das operadoras Claro, TIM e Vivo, conforme a cobertura disponível.</p>

        <h4 style="color: var(--accent-color); margin-top: 20px; margin-bottom: 10px;">2. Funcionamento do Serviço</h4>
        <p>O serviço funciona por meio de chip ativado ou configuração especial de APN, em conjunto com uma VPN pré-configurada.<br>
          A conexão à internet é realizada por meio da VPN, proporcionando maior estabilidade e continuidade do tráfego de dados.<br>
          O serviço depende da cobertura da operadora na região do usuário.</p>

        <h4 style="color: var(--accent-color); margin-top: 20px; margin-bottom: 10px;">3. Uso Aceitável</h4>
        <p>Ao utilizar o serviço, você se compromete a:</p>
        <ul style="padding-left: 20px; margin-bottom: 15px;">
          <li>Utilizar o acesso apenas para fins pessoais e legais;</li>
          <li>Não redistribuir ou revender a conexão de forma comercial;</li>
          <li>Não utilizar o serviço para práticas ilegais, como envio de spam, ataques, mineração de criptomoedas ou automações abusivas.</li>
        </ul>

        <h4 style="color: var(--accent-color); margin-top: 20px; margin-bottom: 10px;">4. Limitações Técnicas</h4>
        <p>A velocidade de conexão pode variar de acordo com:</p>
        <ul style="padding-left: 20px; margin-bottom: 15px;">
          <li>Sinal da operadora;</li>
          <li>Congestionamento de rede;</li>
          <li>Condições técnicas dos servidores VPN.</li>
        </ul>
        <p>O serviço pode passar por manutenções ou instabilidades ocasionais, sem garantia de uptime contínuo.</p>

        <h4 style="color: var(--accent-color); margin-top: 20px; margin-bottom: 10px;">5. Operadoras e Responsabilidade</h4>
        <p>A Souza NET não possui vínculo direto com as operadoras Claro, TIM ou Vivo; utilizamos conexões permitidas dentro dos parâmetros legais e técnicos.<br>
          Em casos de limitação, bloqueio ou restrição de uso por parte da operadora, a Souza NET não se responsabiliza por possíveis interrupções.</p>

        <h4 style="color: var(--accent-color); margin-top: 20px; margin-bottom: 10px;">6. Privacidade e Segurança</h4>
        <p>O tráfego de dados é criptografado via VPN, garantindo maior privacidade.<br>
          A Souza NET não monitora conteúdos acessados e mantém apenas logs técnicos mínimos, para fins de suporte e estabilidade do serviço.</p>

        <h4 style="color: var(--accent-color); margin-top: 20px; margin-bottom: 10px;">7. Cancelamento</h4>
        <p>O serviço pode ser cancelado a qualquer momento por iniciativa do cliente. O cancelamento suspende o acesso imediato à VPN e configurações associadas.</p>

        <h4 style="color: var(--accent-color); margin-top: 20px; margin-bottom: 10px;">8. Alterações dos Termos</h4>
        <p>A Souza NET pode atualizar estes Termos de Uso a qualquer momento, sem aviso prévio. A continuidade do uso do serviço implica concordância com as versões atualizadas.</p>
      </div>
      <div class="modal-footer">
        <button type="button" class="button button-primary" id="accept-terms-btn">Aceitar</button>
      </div>
    </div>
  </div>


  <script>
    let appVersion = '3.0.0';

    // --- Start of Combined and Adapted JavaScript ---

    // Mock data and constants

    let mainBackgroundImageUrl = 'https://i.ibb.co/8nyJHdKJ/photo-2025-07-08-14-33-31.jpg';
    let mainBgPositionY = '180px';
    let userAvatarUrl = 'https://i.postimg.cc/76Pqnycb/banner-sem-fundo.png';
    const renewalUrl = '';
    const termsUrl = 'https://pastebin.com/raw/XRpJZyfx';
    const supportUrl = '';
    const speedTestUrl = 'https://www.speedtest.net/pt';
    const hostshareUrl = 'hostshare'; // Definir como string vazia para desabilitar

    const MOCK_CONFIGS = `[
          {"name": "Servidores BR", "items": [
            {"mode":"V2RAY", "name":"Servidor Brasileiro", "id":1, "icon":"https://cdn-icons-png.flaticon.com/128/4625/4625178.png"},
            {"mode":"SSH", "name":"BR TIM", "id":2, "icon":"https://cdn-icons-png.flaticon.com/128/4625/4625178.png"},
            {"mode":"OVPN", "name":"BR CLARO", "id":3, "icon":"https://cdn-icons-png.flaticon.com/128/4625/4625178.png"}
          ]},
          {"name": "Servidores USA", "items": [
            {"mode":"V2RAY", "name":"USA Games", "id":4, "icon":"https://cdn-icons-png.flaticon.com/512/1040/1040221.png"},
            {"mode":"SSH", "name":"USA Streaming", "id":5, "icon":"https://cdn-icons-png.flaticon.com/512/1040/1040221.png"}
          ]},
          {"name": "Servidores VIP", "items": [
            {"mode":"V2RAY", "name":"VIP 1", "id":6, "icon":"https://cdn-icons-png.flaticon.com/512/1040/1040221.png"}
          ]}
        ]`;

    let checkUserTimeout;
    let allConfigs = [];
    let filteredAutoConnectConfigs = [];
    let autoConnectConfigs = [];
    let currentConfigIndex = 0;
    let isAutoConnecting = false;
    let connectionTimeoutId;
    let connectionTimedOut = false;
    let isHotspotActive = false;
    let pingInterval;

    // --- Utility Functions ---
    function showToast(message) {
      const toast = document.getElementById('toast');
      if (!toast) return;
      toast.textContent = message;
      toast.classList.add('show');
      setTimeout(() => {
        toast.classList.remove('show');
      }, 3500);
    }

    // --- Modal Management ---
    class Modal {
      constructor(id) {
        this.modal = document.getElementById(id);
        if (!this.modal) return;
        this.modal.addEventListener('click', (e) => {
          if (e.target === this.modal) this.hide();
        });
        const closeButton = this.modal.querySelector(`[data-modal-id="${id}"]`);
        if (closeButton) {
          closeButton.addEventListener('click', () => this.hide());
        }
      }
      show() {
        if (this.modal) {
          // Aplicar animação para hotspotModal e autoConnectModal
          if (this.modal.id === 'hotspotModal' || this.modal.id === 'autoConnectModal') {
            const content = this.modal.querySelector('.modal-content');
            if (content) {
              // Resetar animação
              content.style.animation = 'none';
              content.offsetHeight; // Trigger reflow
              content.style.animation = 'slideInModal 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275)';
            }
          }
          this.modal.classList.add('show');
        }
      }
      hide() {
        if (this.modal) {
          // Aplicar animação de saída para hotspotModal e autoConnectModal
          if (this.modal.id === 'hotspotModal' || this.modal.id === 'autoConnectModal') {
            const content = this.modal.querySelector('.modal-content');
            if (content) {
              content.classList.add('hiding');
              // Remover a classe show após a animação terminar
              setTimeout(() => {
                this.modal.classList.remove('show');
                content.classList.remove('hiding');
              }, 300); // Tempo da animação
              return;
            }
          }
          this.modal.classList.remove('show');
        }
      }
    }
    const configModal = new Modal('configModal');
    const loggerModal = new Modal('loggerModal');
    const autoConnectModal = new Modal('autoConnectModal');
    const dragonLoginModal = new Modal('dragonLoginModal');
    const hotspotModal = new Modal('hotspotModal');
    const termsModal = new Modal('termsModal');


    // --- VPN Connection Logic ---
    const startStopVpn = e => {
      const state = window?.DtGetVpnState?.execute() ?? 'DISCONNECTED';
      if (state !== 'DISCONNECTED') {
        window?.DtExecuteVpnStop?.execute();
      } else {
        const savedUser = window?.DtUsername?.get() || '';
        const savedPass = window?.DtPassword?.get() || '';
        const savedUuid = window?.DtUuid?.get() || '';
        document.getElementById('dragon-modal-username').value = savedUser;
        document.getElementById('dragon-modal-password').value = savedPass;
        document.getElementById('uuid').value = savedUuid;

        // Verificar se a configuração atual é V2RAY
        try {
          const currentConfigData = window?.DtGetDefaultConfig?.execute();
          const selectedConfig = currentConfigData ? JSON.parse(currentConfigData) : null;

          const uuidGroup = document.getElementById('uuid-group');
          // Seleção mais compatível dos grupos de input
          const inputGroups = document.querySelectorAll('#dragonLoginModal .input-group');
          const usernameGroup = inputGroups[0]; // Primeiro input-group (username)
          const passwordGroup = inputGroups[1]; // Segundo input-group (password)

          if (selectedConfig && selectedConfig.mode.toLowerCase().startsWith('v2ray')) {
            // Para V2RAY: mostrar UUID e esconder username/password
            uuidGroup.style.display = 'block';
            usernameGroup.style.display = 'none';
            passwordGroup.style.display = 'none';
          } else {
            // Para outros modos: esconder UUID e mostrar username/password
            uuidGroup.style.display = 'none';
            usernameGroup.style.display = 'block';
            passwordGroup.style.display = 'block';
          }
        } catch (e) {
          console.error("Error checking config mode:", e);
        }

        dragonLoginModal.show();
      }
    }

    // --- UI State Listener ---
    const dtVpnStateListener = state => {
      const powerButton = document.querySelector('.power-button');
      const powerButtonContainer = document.querySelector('.power-button-container');
      const connectText = document.querySelector('.connect-text');
      const logsContainer = document.getElementById('main-screen-logs');
      const userInfoContainer = document.getElementById('user-info');
      const mainContainer = document.querySelector('main');
      const appVersion = document.querySelector('.app-version');
      if (!powerButton || !connectText || !logsContainer || !userInfoContainer || !mainContainer) return;

      powerButtonContainer.classList.remove('connecting', 'connected', 'error', 'stopping');
      connectText.classList.remove('connected-status');

      logsContainer.style.display = state === 'CONNECTING' ? 'block' : 'none';
      userInfoContainer.style.display = state === 'CONNECTED' ? 'block' : 'none';

      // Mostrar/esconder versão baseado no status
      if (appVersion) {
        appVersion.style.display = state === 'CONNECTED' ? 'none' : 'block';
      }

      // Adicionar/remover classe para reposicionar o botão quando conectado
      if (state === 'CONNECTED') {
        mainContainer.classList.add('connected-state');
      } else {
        mainContainer.classList.remove('connected-state');
      }

      switch (state) {
        case 'DISCONNECTED':
          connectText.textContent = 'Clique aqui para conectar';
          if (isAutoConnecting) {
            if (connectionTimedOut) {
              addAutoConnectLog(`Tempo esgotado. Tentando o próximo...`);
            } else {
              addAutoConnectLog("Falhou. Tentando próximo servidor...");
            }
            currentConfigIndex++;
            setTimeout(tryNextConfig, 1000);
          }
          if (pingInterval) clearInterval(pingInterval);
          break;
        case 'CONNECTING':
          powerButtonContainer.classList.add('connecting');
          connectText.textContent = 'Conectando...';
          if (pingInterval) clearInterval(pingInterval);
          break;
        case 'CONNECTED':
          powerButtonContainer.classList.add('connected');
          connectText.classList.add('connected-status');
          const localIP = window?.DtGetLocalIP?.execute() || '10.8.0.2';
          connectText.textContent = `Conectado`;
          showToast('Conectado com sucesso!');

          // Atualizar informações do usuário
          updateSelectedServerInfo();
          document.getElementById('info-ip').textContent = localIP;
          updateUserInfo();

          if (pingInterval) clearInterval(pingInterval);
          pingInterval = setInterval(() => {
            const pingValue = window?.DtGetPingResult?.execute() ?? '--';
            const pingElement = document.getElementById('info-ping');
            if (pingElement) {
              pingElement.textContent = `${pingValue} ms`;
            }
          }, 5000);

          if (isAutoConnecting) {
            const connectedConfig = autoConnectConfigs[currentConfigIndex];
            addAutoConnectLog(`Conectado com sucesso em: ${connectedConfig.name}!`);
            isAutoConnecting = false;
            resetAutoConnectModal();
            setTimeout(() => {
              autoConnectModal.hide();
            }, 2000);
          }
          break;
        case 'STOPPING':
          powerButtonContainer.classList.add('stopping');
          connectText.textContent = 'Desconectando...';
          if (pingInterval) clearInterval(pingInterval);
          break;
        case 'AUTH_FAILED':
          powerButtonContainer.classList.add('error');
          connectText.textContent = 'Erro de Autenticação';
          if (pingInterval) clearInterval(pingInterval);
          if (isAutoConnecting) {
            addAutoConnectLog("Falha na autenticação. Tentando próximo servidor...");
            currentConfigIndex++;
            setTimeout(tryNextConfig, 1000);
          }
          break;
        default:
          connectText.textContent = 'Clique aqui para conectar';
          if (pingInterval) clearInterval(pingInterval);
          break;
      }
    };

    // Função para atualizar informações do usuário conectado
    function updateUserInfo() {
      const username = window?.DtUsername?.get() || 'Usuário';
      document.getElementById('info-username').textContent = username;

      // Solicitar verificação do usuário para obter os detalhes
      window?.DtStartCheckUser?.execute();
    }

    // --- Hotspot Functions ---
    function updateHotspotStatus() {
      // Se hostshare não estiver configurado, não faz nada
      if (!hostshareUrl) {
        return;
      }

      const status = window?.DtGetStatusHotSpotService?.execute() || 'INACTIVE';
      isHotspotActive = status.toUpperCase() === 'ACTIVE';

      const toggleHotspotButton = document.getElementById('toggleHotspotButton');
      if (toggleHotspotButton) {
        if (isHotspotActive) {
          toggleHotspotButton.textContent = 'Parar';
          toggleHotspotButton.classList.add('stopping');
        } else {
          toggleHotspotButton.textContent = 'Ativar Hotspot';
          toggleHotspotButton.classList.remove('stopping');
        }
      }
    }

    window.onHotspotStateListener = (state) => {
      // Se hostshare não estiver configurado, não faz nada
      if (!hostshareUrl) {
        return;
      }

      updateHotspotStatus();
      const isActive = state.toUpperCase() === 'ACTIVE';
      if (isActive) {
        showToast('Hotspot ativado! Verifique a notificação para a porta.');
      } else {
        showToast('Hotspot desativado.');
      }
    };

    // --- Config Modal Logic ---
    const showConfigsModal = () => {
      try {
        const data = JSON.parse(window?.DtGetConfigs?.execute() || MOCK_CONFIGS);
        const modalContent = configModal.modal.querySelector('.modal-content');
        // Obter o ID da configuração atual
        const currentConfigData = window?.DtGetDefaultConfig?.execute();
        const currentConfig = currentConfigData ? JSON.parse(currentConfigData) : null;
        const currentConfigId = currentConfig ? currentConfig.id : 0;

        let oldFilter = modalContent.querySelector('.category-filter');
        if (oldFilter) oldFilter.remove();

        const configBody = modalContent.querySelector('.config-body');
        configBody.innerHTML = '';

        // Lógica de agrupamento de categorias idêntica ao temaNgma
        const groups = new Map();
        data.forEach(category => {
          const groupName = category.name.trim().split(' ')[0].toUpperCase();
          if (!groups.has(groupName)) {
            groups.set(groupName, []);
          }
          groups.get(groupName).push(category);
        });

        const categoryFilter = document.createElement('div');
        categoryFilter.className = 'category-filter';

        let filterHtml = `<div class="category-chip active" data-category="ALL">Todas</div>`;

        groups.forEach((categoriesInGroup, groupName) => {
          if (groupName.length >= 3) {
            const count = categoriesInGroup.length;
            const displayName = count > 1 ? `${groupName} (${count})` : groupName;
            filterHtml += `<div class="category-chip" data-category="${groupName}">${displayName}</div>`;
          }
        });

        categoryFilter.innerHTML = filterHtml;
        modalContent.querySelector('.modal-header').after(categoryFilter);

        const updateConfigList = (selectedGroup) => {
          configBody.innerHTML = '';

          const categoriesToShow = selectedGroup === 'ALL' ?
            data :
            (groups.get(selectedGroup) || []);

          categoriesToShow.forEach(category => {
            const items = category.items;
            if (items.length > 0) {
              const categoryHeader = document.createElement('div');
              categoryHeader.className = 'bg-category';
              categoryHeader.textContent = category.name;
              configBody.appendChild(categoryHeader);

              items.forEach(item => {
                const configElement = document.createElement('div');
                configElement.className = 'bg-config';
                // Destacar a configuração atual
                if (item.id === currentConfigId) {
                  configElement.classList.add('selected');
                }
                configElement.innerHTML = `
                                    <img src="${item.icon}" alt="">
                                    <div class="config-info">
                                        <span class="config-name">${item.name}</span>
                                        <span class="config-description">${item.description || 'Servidor otimizado'}</span>
                                    </div>
                                    <span class="config-mode">${item.mode}</span>`;
                configElement.onclick = () => {
                  window?.DtSetConfig?.execute(item.id);

                  const serverNameEl = document.querySelector('.server-info span');
                  const serverFlagEl = document.querySelector('.server-info img');
                  const serverDescEl = document.querySelector('.server-info small');
                  if (serverNameEl) serverNameEl.textContent = item.name;
                  if (serverFlagEl && item.icon) serverFlagEl.src = item.icon;
                  if (serverDescEl) serverDescEl.textContent = item.description || 'Servidor otimizado';

                  // Atualizar a interface para mostrar a nova seleção
                  document.querySelectorAll('#configModal .bg-config').forEach(el => {
                    el.classList.remove('selected');
                  });
                  configElement.classList.add('selected');

                  // Fechar o modal imediatamente
                  configModal.hide();
                };
                configBody.appendChild(configElement);
              });
            }
          });
        };

        categoryFilter.querySelectorAll('.category-chip').forEach(chip => {
          chip.onclick = () => {
            categoryFilter.querySelector('.active').classList.remove('active');
            chip.classList.add('active');
            updateConfigList(chip.dataset.category);
          };
        });

        updateConfigList('ALL');
        configModal.show();
      } catch (e) {
        console.error('Error showing configs:', e);
        showToast('Erro ao carregar configurações.');
      }
    };

    // --- Check User Modal Logic ---
    function showCheckUserModal() {
      window?.dtCheckUserStartedListener?.();
      window?.DtStartCheckUser?.execute();

      if (checkUserTimeout) clearTimeout(checkUserTimeout);

      checkUserTimeout = setTimeout(() => {
        showToast('Verificação de usuário expirou.');
      }, 5000);
    }

    window.dtCheckUserStartedListener = () => {
      const messageArea = document.querySelector('#user-info');
      if (messageArea) {
        const loadingHtml = `
                    <div class="user-loading">
                        <div class="loading-spinner"></div>
                        <p>Verificando dados do usuário...</p>
                    </div>
                `;
        messageArea.innerHTML = loadingHtml;
        messageArea.style.display = 'block';
      }
    }

    window.dtCheckUserModelListener = (model) => {
      if (checkUserTimeout) clearTimeout(checkUserTimeout);
      try {
        const data = JSON.parse(model);

        // Se não houver dados ou usuário estiver vazio, mostrar mensagem
        if (!data || !data.username) {
          const messageArea = document.querySelector('#user-info');
          if (messageArea) {
            messageArea.innerHTML = `
                            <div class="user-error">
                                <i class="fas fa-exclamation-circle" style="color: var(--error-color, #FF3B30); font-size: 24px; margin-bottom: 10px;"></i>
                                <p>Não foi possível obter os dados do usuário.</p>
                            </div>
                        `;
            messageArea.style.display = 'block';
          }
          return;
        }

        const html = `
                    <div class="user-header">
                        <div class="user-avatar">
                            <img src="${userAvatarUrl}" alt="Avatar">
                        </div>
                        <div>
                            <div class="user-name" id="info-username">${data.username}</div>
                            <div class="user-status">
                                <div class="status-dot"></div>
                                Conectado
                            </div>
                        </div>
                        <div class="user-version">v${appVersion}</div>
                    </div>
                    <div class="user-details">
                        <div class="detail-item">
                            <div class="detail-label">Ping</div>
                            <div class="detail-value" id="info-ping">-- ms</div>
                        </div>
                        <div class="detail-item">
                            <div class="detail-label">Validade</div>
                            <div class="detail-value" id="info-days">${data.expiration_date || '--'}</div>
                        </div>
                        <div class="detail-item">
                            <div class="detail-label">Conexões</div>
                            <div class="detail-value" id="info-connections">${data.count_connections || '0'}/${data.limit_connections || '0'}</div>
                        </div>
                        <div class="detail-item">
                            <div class="detail-label">IP Local</div>
                            <div class="detail-value" id="info-ip">${window?.DtGetLocalIP?.execute() || '0.0.0.0'}</div>
                        </div>
                    </div>
                `;

        // Atualizar informações na tela principal
        const userInfoContainer = document.getElementById('user-info');
        if (userInfoContainer) {
          userInfoContainer.innerHTML = html;
        }

        // Iniciar a atualização do ping
        if (pingInterval) clearInterval(pingInterval);
        pingInterval = setInterval(() => {
          const pingValue = window?.DtGetPingResult?.execute() ?? '--';
          const pingElement = document.getElementById('info-ping');
          if (pingElement) {
            pingElement.textContent = `${pingValue} ms`;
          }
        }, 3000);

      } catch (e) {
        console.error('Error processing CheckUser:', e);
        const messageArea = document.querySelector('#user-info');
        if (messageArea) {
          messageArea.innerHTML = `
                        <div class="user-error">
                            <i class="fas fa-exclamation-circle" style="color: var(--error-color, #FF3B30); font-size: 24px; margin-bottom: 10px;"></i>
                            <p>Erro ao processar os dados do usuário.</p>
                        </div>
                    `;
          messageArea.style.display = 'block';
        }
      }
    };

    // --- Auto-Connect Logic ---
    function addAutoConnectLog(message) {
      const logContainer = document.getElementById('auto-connect-logs');
      if (logContainer) {
        if (logContainer.innerHTML.includes('<!--')) {
          logContainer.innerHTML = '';
        }
        const time = new Date().toLocaleTimeString();
        logContainer.innerHTML += `<div><span style="color: var(--accent-color);">[${time}]</span> ${message}</div>`;
        logContainer.scrollTop = logContainer.scrollHeight;
      }
    }

    // Event handler para DtNewLogEvent
    window.DtNewLogEvent = function() {
      const log = window?.DtGetLogs?.execute() || '[]';
      try {
        const data = JSON.parse(log);
        if (data.length > 0) {
          // Pegar o log mais recente
          const lastLog = data[data.length - 1];
          const key = Object.keys(lastLog)[0];
          const message = lastLog[key];
          // Adicionar ao container de auto-connect-logs se estiver visível
          if (document.getElementById('autoConnectModal').classList.contains('show')) {
            addAutoConnectLog(`${key}: ${message}`);
          }
        }
      } catch (e) {
        console.error("Erro ao processar logs:", e);
      }
    };

    function startAutoConnection() {
      isAutoConnecting = true;
      currentConfigIndex = 0;
      autoConnectConfigs = filteredAutoConnectConfigs;

      if (autoConnectConfigs.length === 0) {
        showToast("Nenhuma configuração selecionada para testar.");
        isAutoConnecting = false;
        return;
      }

      document.getElementById('auto-connect-start-btn').disabled = true;
      document.getElementById('auto-connect-cancel-btn').textContent = 'Parar';
      document.querySelectorAll('#auto-connect-category-filter .category-chip').forEach(chip => chip.style.pointerEvents = 'none');
      const logContainer = document.getElementById('auto-connect-logs');
      logContainer.innerHTML = '';
      addAutoConnectLog("Iniciando conexão automática...");
      tryNextConfig();
    }

    function tryNextConfig() {
      if (!isAutoConnecting || currentConfigIndex >= autoConnectConfigs.length) {
        if (isAutoConnecting) {
          showToast("Não foi possível conectar a nenhum servidor.");
          addAutoConnectLog("Fim dos testes. Nenhum servidor conectou.");
        }
        isAutoConnecting = false;
        resetAutoConnectModal();
        window?.DtExecuteVpnStop?.execute();
        return;
      }

      connectionTimedOut = false;
      const config = autoConnectConfigs[currentConfigIndex];
      window?.DtSetConfig?.execute(config.id);
      addAutoConnectLog(`Testando: ${config.name}`);
      window?.DtExecuteVpnStart?.execute();

      connectionTimeoutId = setTimeout(() => {
        if (!isAutoConnecting) return;
        connectionTimedOut = true;
        window?.DtExecuteVpnStop?.execute();
      }, 8000); // 8 second timeout per connection
    }

    function resetAutoConnectModal() {
      const startButton = document.getElementById('auto-connect-start-btn');
      if (startButton) startButton.disabled = false;
      const cancelButton = document.getElementById('auto-connect-cancel-btn');
      if (cancelButton) cancelButton.textContent = 'Cancelar';
      document.querySelectorAll('#auto-connect-category-filter .category-chip').forEach(chip => chip.style.pointerEvents = 'auto');
    }

    function stopAutoConnection() {
      isAutoConnecting = false;
      clearTimeout(connectionTimeoutId);
      window?.DtExecuteVpnStop?.execute();
      addAutoConnectLog("Processo de conexão automática parado.");
      resetAutoConnectModal();
    }

    // --- Logger Logic ---
    window.dtOnNewLogListener = () => {
      const modalLogContent = loggerModal.modal?.querySelector('.logger-content');
      const mainLogContent = document.getElementById('main-screen-logs');
      const expandedLogContent = document.querySelector('#logs-expanded .logs-content');

      const log = window?.DtGetLogs?.execute() || '[]';

      try {
        const data = JSON.parse(log);
        let modalContent = '';
        let mainContent = '';
        let expandedContent = '';

        data.forEach(item => {
          const key = Object.keys(item)[0];
          const message = item[key];
          modalContent += `<li><strong style="color:var(--accent-color)">${key}</strong>: ${message}</li>`;
          mainContent += `<div><strong style="color:var(--accent-color)">${key}</strong> ${message}</div>`;
          expandedContent += `<div><strong style="color:var(--accent-color)">${key}</strong>: ${message}</div>`;
        });

        if (modalLogContent) {
          modalLogContent.innerHTML = modalContent;
          modalLogContent.scrollTop = modalLogContent.scrollHeight;
        }
        if (mainLogContent) {
          mainLogContent.innerHTML = mainContent;
          mainLogContent.scrollTop = mainLogContent.scrollHeight;
        }
        if (expandedLogContent) {
          expandedLogContent.innerHTML = expandedContent;
          expandedLogContent.scrollTop = expandedLogContent.scrollHeight;
        }
      } catch (e) {
        console.error("Error parsing logs:", e);
      }
    }

    // Função para abrir o modal de logs expandido
    function openLogsModal() {
      document.body.classList.add('logs-open');
    }

    // Função para fechar o modal de logs expandido
    function closeLogsModal() {
      document.body.classList.remove('logs-open');
    }

    // --- Theme Management ---
    const themeToggle = document.getElementById('theme-toggle');
    const body = document.body;

    const setDarkMode = (isDark) => {
      if (isDark) {
        body.classList.remove('light-theme');
        body.classList.add('dark-theme');
      } else {
        body.classList.remove('dark-theme');
        body.classList.add('light-theme');
      }
      themeToggle.classList.toggle('fa-sun', isDark);
      themeToggle.classList.toggle('fa-moon', !isDark);
      localStorage.setItem('theme', isDark ? 'dark' : 'light');
    };

    themeToggle.addEventListener('click', () => {
      setDarkMode(!body.classList.contains('dark-theme'));
    });

    // --- Side Navbar Logic ---
    const openNavButton = document.getElementById('open-nav');
    const closeNavButton = document.getElementById('close-nav');
    const navOverlay = document.getElementById('navbar-overlay');

    const closeNav = () => body.classList.remove('navbar-open');
    openNavButton.addEventListener('click', () => body.classList.add('navbar-open'));
    closeNavButton.addEventListener('click', closeNav);
    navOverlay.addEventListener('click', closeNav);

    // Handler para o evento de VPN iniciada com sucesso
    window.DtVpnStartedSuccessEvent = function() {
      // Verificar se auto-conexão está ativa e pará-la
      if (isAutoConnecting) {
        clearTimeout(connectionTimeoutId); // Limpar o timeout de conexão
        isAutoConnecting = false; // Desativar flag de auto-conexão

        // Adicionar mensagem aos logs de autoconexão
        addAutoConnectLog('VPN iniciada com sucesso. Parando auto-conexão...');

        // Resetar a interface do modal de auto-conexão
        resetAutoConnectModal();
      }

      // Procurar por modais abertos e fechá-los
      const openModals = document.querySelectorAll('.modal.show');
      openModals.forEach(modal => {
        // Obter o objeto Modal correspondente e usar o método hide
        const modalId = modal.id;
        if (modalId === 'configModal') configModal.hide();
        else if (modalId === 'autoConnectModal') autoConnectModal.hide();
        else if (modalId === 'dragonLoginModal') dragonLoginModal.hide();
        else if (modalId === 'loggerModal') loggerModal.hide();
        else if (modalId === 'hotspotModal') hotspotModal.hide();
        else modal.classList.remove('show'); // Fallback para outros modais
      });

      showToast('VPN iniciada com sucesso!');
    };

    // --- Event Listeners Setup ---

    function updateSelectedServerInfo() {
      try {
        const currentConfigJSON = window?.DtGetDefaultConfig?.execute();
        let currentConfig = null;

        if (currentConfigJSON) {
          currentConfig = JSON.parse(currentConfigJSON);
        }

        if (currentConfig && currentConfig.id) {
          const serverNameEl = document.querySelector('.server-info span');
          const serverFlagEl = document.querySelector('.server-info img');
          const serverDescEl = document.querySelector('.server-info small');

          if (serverNameEl) serverNameEl.textContent = currentConfig.name;
          if (serverFlagEl && currentConfig.icon) serverFlagEl.src = currentConfig.icon;
          if (serverDescEl) serverDescEl.textContent = currentConfig.description || 'Servidor otimizado';
        } else {
          // Fallback to first config if none is selected
          const allConfigsData = window?.DtGetConfigs?.execute() || MOCK_CONFIGS;
          const allConfigs = JSON.parse(allConfigsData);
          if (allConfigs.length > 0 && allConfigs[0].items.length > 0) {
            const defaultConfig = allConfigs[0].items[0];
            const serverNameEl = document.querySelector('.server-info span');
            const serverFlagEl = document.querySelector('.server-info img');
            const serverDescEl = document.querySelector('.server-info small');

            if (serverNameEl) serverNameEl.textContent = defaultConfig.name;
            if (serverFlagEl && defaultConfig.icon) serverFlagEl.src = defaultConfig.icon;
            if (serverDescEl) serverDescEl.textContent = defaultConfig.description || 'Servidor otimizado';
          }
        }
      } catch (e) {
        console.error("Failed to update selected server info:", e);
      }
    }

    document.addEventListener('DOMContentLoaded', () => {
      // Set App Version
      document.getElementById('navbar-version').textContent = appVersion;
      document.getElementById('main-version').textContent = `v${appVersion}`;
      document.getElementById('user-version-display').textContent = `v${appVersion}`;

      // Set background image and position
      const phoneMockup = document.querySelector('.phone-mockup');
      if (phoneMockup) {
        if (mainBackgroundImageUrl) {
          phoneMockup.style.setProperty('--main-bg-image', `url('${mainBackgroundImageUrl}')`);
        }
        if (mainBgPositionY) {
          phoneMockup.style.setProperty('--main-bg-position-y', mainBgPositionY);
        }
      }

      // Construir menu dinamicamente com base nas constantes
      const dynamicNavbar = document.getElementById('dynamic-navbar-links');

      // Adicionar itens condicionalmente com base nas constantes
      if (speedTestUrl) {
        const speedtestItem = document.createElement('li');
        speedtestItem.innerHTML = `<a href="#" id="nav-speedtest"><i class="fas fa-tachometer-alt"></i> Speedtest</a>`;
        dynamicNavbar.appendChild(speedtestItem);
      }

      if (renewalUrl) {
        const renewalItem = document.createElement('li');
        renewalItem.innerHTML = `<a href="#" id="nav-renewal"><i class="fas fa-credit-card"></i> Renovar</a>`;
        dynamicNavbar.appendChild(renewalItem);
      }

      if (hostshareUrl) {
        const hostshareItem = document.createElement('li');
        hostshareItem.innerHTML = `<a href="#" id="nav-hostshare"><i class="fas fa-wifi"></i> Hostshare</a>`;
        dynamicNavbar.appendChild(hostshareItem);
      }

      if (supportUrl) {
        const supportItem = document.createElement('li');
        supportItem.innerHTML = `<a href="#" id="nav-support"><i class="fas fa-headset"></i> Suporte</a>`;
        dynamicNavbar.appendChild(supportItem);
      }

      if (termsUrl) {
        const termsItem = document.createElement('li');
        termsItem.innerHTML = `<a href="#" id="nav-terms"><i class="fas fa-file-contract"></i> Termos</a>`;
        dynamicNavbar.appendChild(termsItem);
      }

      // Set avatar images from a single source
      document.querySelector('.navbar-profile img').src = userAvatarUrl;
      document.querySelector('#dragonLoginModal .modal-avatar img').src = userAvatarUrl;
      document.querySelector('#user-info .user-avatar img').src = userAvatarUrl;

      // Configurar eventos para o modal de logs expandido
      const mainLogsContainer = document.getElementById('main-screen-logs');
      const closeLogsBtn = document.getElementById('close-logs');
      const logsModalOverlay = document.getElementById('logs-modal-overlay');
      const clearLogsBtn = document.getElementById('clear-logs-btn');

      if (mainLogsContainer) {
        mainLogsContainer.addEventListener('click', openLogsModal);
      }

      if (closeLogsBtn) {
        closeLogsBtn.addEventListener('click', closeLogsModal);
      }

      if (logsModalOverlay) {
        logsModalOverlay.addEventListener('click', closeLogsModal);
      }

      if (clearLogsBtn) {
        clearLogsBtn.addEventListener('click', () => {
          window?.DtClearLogs?.execute();
          const expandedLogContent = document.querySelector('#logs-expanded .logs-content');
          const mainLogContent = document.getElementById('main-screen-logs');
          if (expandedLogContent) expandedLogContent.innerHTML = '';
          if (mainLogContent) mainLogContent.innerHTML = '';
          showToast('Logs limpos com sucesso!');
        });
      }



      // Main connection button
      const powerButton = document.querySelector('.power-button');
      if (powerButton) powerButton.onclick = startStopVpn;

      // Server selection
      const serverSelect = document.querySelector('.server-select');
      if (serverSelect) serverSelect.onclick = function(e) {
        // Verifica se o clique foi no ícone de auto conexão
        if (e.target.closest('#auto-connect-icon')) {
          e.stopPropagation();

          // Lógica do modal de auto conexão
          allConfigs = JSON.parse(window?.DtGetConfigs?.execute() || MOCK_CONFIGS);
          const categoryFilterContainer = document.getElementById('auto-connect-category-filter');
          categoryFilterContainer.innerHTML = '';

          let filterHtml = `<div class="category-chip active" data-category="ALL">Todas</div>`;

          // Lógica de filtro idêntica ao temaNgma
          allConfigs.forEach(category => {
            filterHtml += `<div class="category-chip" data-category="${category.name}">${category.name}</div>`;
          });

          categoryFilterContainer.innerHTML = filterHtml;

          const updateSelection = (categoryName) => {
            if (categoryName === 'ALL') {
              filteredAutoConnectConfigs = allConfigs.flatMap(c => c.items);
            } else {
              const foundCategory = allConfigs.find(c => c.name === categoryName);
              filteredAutoConnectConfigs = foundCategory ? foundCategory.items : [];
            }

            const firstConfigNameEl = document.getElementById('first-config-name');
            if (filteredAutoConnectConfigs.length > 0) {
              firstConfigNameEl.textContent = filteredAutoConnectConfigs[0].name;
            } else {
              firstConfigNameEl.textContent = 'Nenhuma configuração nesta categoria.';
            }
          };

          categoryFilterContainer.querySelectorAll('.category-chip').forEach(chip => {
            chip.addEventListener('click', () => {
              categoryFilterContainer.querySelector('.active').classList.remove('active');
              chip.classList.add('active');
              updateSelection(chip.dataset.category);
            });
          });

          updateSelection('ALL');
          resetAutoConnectModal();
          autoConnectModal.show();
        } else {
          // Mostrar o modal de configuração normal
          showConfigsModal();
        }
      };

      // Navbar links
      const navSupport = document.getElementById('nav-support');
      if (navSupport && supportUrl) navSupport.addEventListener('click', (e) => {
        e.preventDefault();
        window.open(supportUrl, '_blank');
        closeNav();
      });

      const navTerms = document.getElementById('nav-terms');
      if (navTerms) navTerms.addEventListener('click', (e) => {
        e.preventDefault();
        termsModal.show();
        closeNav();
      });

      const navRenewal = document.getElementById('nav-renewal');
      if (navRenewal && renewalUrl) navRenewal.addEventListener('click', (e) => {
        e.preventDefault();
        window.open(renewalUrl, '_blank');
        closeNav();
      });

      const navSpeedtest = document.getElementById('nav-speedtest');
      if (navSpeedtest && speedTestUrl) navSpeedtest.addEventListener('click', (e) => {
        e.preventDefault();
        window?.DtStartWebViewActivity?.execute(speedTestUrl);
        closeNav();
      });

      const navHostshare = document.getElementById('nav-hostshare');
      if (navHostshare) navHostshare.addEventListener('click', (e) => {
        e.preventDefault();
        if (!hostshareUrl) {
          showToast('Funcionalidade não disponível');
          closeNav();
          return;
        }
        updateHotspotStatus();
        hotspotModal.show();
        closeNav();
      });

      const toggleHotspotButton = document.getElementById('toggleHotspotButton');
      if (toggleHotspotButton) {
        toggleHotspotButton.addEventListener('click', () => {
          if (!hostshareUrl) {
            showToast('Funcionalidade não disponível');
            hotspotModal.hide();
            return;
          }

          const wasActive = isHotspotActive;

          if (wasActive) {
            window?.DtStopHotSpotService?.execute();
            toggleHotspotButton.textContent = 'Ativar Hotspot';
            toggleHotspotButton.classList.remove('stopping');
            isHotspotActive = false;
          } else {
            window?.DtStartHotSpotService?.execute();
            toggleHotspotButton.textContent = 'Parar';
            toggleHotspotButton.classList.add('stopping');
            isHotspotActive = true;
          }
        });
      }

      const navUpdate = document.getElementById('nav-update');
      if (navUpdate) navUpdate.addEventListener('click', (e) => {
        e.preventDefault();
        window?.DtStartAppUpdate?.execute();
        showToast('Procurando por atualizações...');
        closeNav();
      });

      // Adicionar funcionalidade de arrastar para o menu
      const navbarLinks = document.querySelector('.navbar-links');
      if (navbarLinks) {
        let isDown = false;
        let startX;
        let scrollLeft;

        navbarLinks.addEventListener('mousedown', (e) => {
          isDown = true;
          navbarLinks.classList.add('dragging');
          startX = e.pageX - navbarLinks.offsetLeft;
          scrollLeft = navbarLinks.scrollLeft;
        });

        navbarLinks.addEventListener('mouseleave', () => {
          isDown = false;
          navbarLinks.classList.remove('dragging');
        });

        navbarLinks.addEventListener('mouseup', () => {
          isDown = false;
          navbarLinks.classList.remove('dragging');
        });

        navbarLinks.addEventListener('mousemove', (e) => {
          if (!isDown) return;
          e.preventDefault();
          const x = e.pageX - navbarLinks.offsetLeft;
          const walk = (x - startX) * 2; // Velocidade do arrasto
          navbarLinks.scrollLeft = scrollLeft - walk;
        });

        // Suporte para dispositivos móveis
        navbarLinks.addEventListener('touchstart', (e) => {
          isDown = true;
          navbarLinks.classList.add('dragging');
          startX = e.touches[0].pageX - navbarLinks.offsetLeft;
          scrollLeft = navbarLinks.scrollLeft;
        }, {
          passive: true
        });

        navbarLinks.addEventListener('touchend', () => {
          isDown = false;
          navbarLinks.classList.remove('dragging');
        });

        navbarLinks.addEventListener('touchmove', (e) => {
          if (!isDown) return;
          const x = e.touches[0].pageX - navbarLinks.offsetLeft;
          const walk = (x - startX) * 2;
          navbarLinks.scrollLeft = scrollLeft - walk;
        }, {
          passive: true
        });
      }

      const navAuto = document.getElementById('nav-auto');
      if (navAuto) navAuto.addEventListener('click', (e) => {
        e.preventDefault();
        allConfigs = JSON.parse(window?.DtGetConfigs?.execute() || MOCK_CONFIGS);
        const categoryFilterContainer = document.getElementById('auto-connect-category-filter');
        categoryFilterContainer.innerHTML = '';

        let filterHtml = `<div class="category-chip active" data-category="ALL">Todas</div>`;

        // Lógica de filtro idêntica ao temaNgma
        allConfigs.forEach(category => {
          filterHtml += `<div class="category-chip" data-category="${category.name}">${category.name}</div>`;
        });

        categoryFilterContainer.innerHTML = filterHtml;

        const updateSelection = (categoryName) => {
          if (categoryName === 'ALL') {
            filteredAutoConnectConfigs = allConfigs.flatMap(c => c.items);
          } else {
            const foundCategory = allConfigs.find(c => c.name === categoryName);
            filteredAutoConnectConfigs = foundCategory ? foundCategory.items : [];
          }

          const firstConfigNameEl = document.getElementById('first-config-name');
          if (filteredAutoConnectConfigs.length > 0) {
            firstConfigNameEl.textContent = filteredAutoConnectConfigs[0].name;
          } else {
            firstConfigNameEl.textContent = 'Nenhuma configuração nesta categoria.';
          }
        };

        categoryFilterContainer.querySelectorAll('.category-chip').forEach(chip => {
          chip.addEventListener('click', () => {
            categoryFilterContainer.querySelector('.active').classList.remove('active');
            chip.classList.add('active');
            updateSelection(chip.dataset.category);
          });
        });

        updateSelection('ALL');
        resetAutoConnectModal();
        autoConnectModal.show();
        closeNav();
      });

      const autoStartBtn = document.getElementById('auto-connect-start-btn');
      if (autoStartBtn) autoStartBtn.addEventListener('click', startAutoConnection);

      const autoCancelBtn = document.getElementById('auto-connect-cancel-btn');
      if (autoCancelBtn) autoCancelBtn.addEventListener('click', () => {
        if (isAutoConnecting) {
          stopAutoConnection();
        } else {
          autoConnectModal.hide();
        }
      });

      // Navbar Profile Click
      const navProfile = document.getElementById('nav-profile-section');
      if (navProfile) {
        navProfile.addEventListener('click', () => {
          const savedUser = window?.DtUsername?.get() || '';
          const savedPass = window?.DtPassword?.get() || '';
          document.getElementById('dragon-modal-username').value = savedUser;
          document.getElementById('dragon-modal-password').value = savedPass;
          dragonLoginModal.show();
          closeNav();
        });
      }

      // Login Modal Logic
      const loginBtn = document.getElementById('dragon-modal-login-btn');
      if (loginBtn) {
        loginBtn.addEventListener('click', () => {
          const user = document.getElementById('dragon-modal-username').value;
          const pass = document.getElementById('dragon-modal-password').value;
          const uuid = document.getElementById('uuid').value;
          const uuidGroup = document.getElementById('uuid-group');

          // Verificar se a configuração atual é V2RAY
          try {
            const currentConfigData = window?.DtGetDefaultConfig?.execute();
            const currentConfig = currentConfigData ? JSON.parse(currentConfigData) : null;
            let isV2ray = false;

            if (currentConfig && currentConfig.mode.toLowerCase().startsWith('v2ray')) {
              isV2ray = true;
            }

            if (isV2ray) {
              // Para V2RAY: verificar apenas UUID
              if (!uuid) {
                showToast('Por favor, insira o UUID para conexão V2RAY.');
                return;
              }
            } else {
              // Para outros modos: verificar username e password
              if (!user || !pass) {
                showToast('Por favor, insira o usuário e a senha.');
                return;
              }
            }
          } catch (e) {
            console.error("Error checking config mode:", e);
            // Fallback para verificação padrão
            if (!user || !pass) {
              showToast('Por favor, insira o usuário e a senha.');
              return;
            }
          }

          window?.DtUsername?.set(user);
          window?.DtPassword?.set(pass);

          // Salvar UUID se fornecido
          if (uuid) {
            window?.DtUuid?.set(uuid);
          }

          const profileName = document.querySelector('.navbar-profile h4');
          const profileEmail = document.querySelector('.navbar-profile p');
          if (profileName) profileName.textContent = user;
          if (profileEmail) profileEmail.textContent = 'Usuário Autenticado';

          dragonLoginModal.hide();
          window?.DtExecuteVpnStart?.execute();
        });
      }
      const passwordToggle = document.querySelector('#dragonLoginModal .password-toggle');
      if (passwordToggle) {
        passwordToggle.addEventListener('click', (e) => {
          const input = e.target.closest('.input-group').querySelector('input');
          const isPassword = input.type === 'password';
          input.type = isPassword ? 'text' : 'password';
          e.target.classList.toggle('fa-eye', !isPassword);
          e.target.classList.toggle('fa-eye-slash', isPassword);
        });
      }

      // Initial state setup
      const savedTheme = localStorage.getItem('theme') || 'dark';
      setDarkMode(savedTheme === 'dark');

      const savedUserForProfile = window?.DtUsername?.get() || '';
      if (savedUserForProfile) {
        const profileName = document.querySelector('.navbar-profile h4');
        const profileEmail = document.querySelector('.navbar-profile p');
        if (profileName) profileName.textContent = savedUserForProfile;
        if (profileEmail) profileEmail.textContent = 'Usuário Autenticado';
      }

      // Verificar status do hotspot
      updateHotspotStatus();

      // Ocultar opção de hotspot se a URL estiver vazia
      const navHostshareItem = document.getElementById('nav-hostshare');
      if (navHostshareItem && !hostshareUrl) {
        navHostshareItem.style.display = 'none';
      }

      // Theme switcher logic
      const setColorTheme = (theme) => {
        document.body.dataset.colorTheme = theme;
        localStorage.setItem('colorTheme', theme);

        document.querySelectorAll('.theme-swatch').forEach(swatch => {
          swatch.classList.remove('active');
        });

        const activeSwatch = document.querySelector(`.theme-swatch[data-theme="${theme}"]`);
        if (activeSwatch) activeSwatch.classList.add('active');
      };

      document.querySelectorAll('.theme-swatch').forEach(swatch => {
        swatch.addEventListener('click', () => {
          setColorTheme(swatch.dataset.theme);
        });
      });

      // 添加接受条款按钮的事件处理程序
      const acceptTermsBtn = document.getElementById('accept-terms-btn');
      if (acceptTermsBtn) {
        acceptTermsBtn.addEventListener('click', () => {
          termsModal.hide();
          showToast('Termos aceitos com sucesso!');
        });
      }

      const savedColorTheme = localStorage.getItem('colorTheme') || 'blue';
      setColorTheme(savedColorTheme);

      updateSelectedServerInfo();
      dtVpnStateListener(window?.DtGetVpnState?.execute() ?? 'DISCONNECTED');
      window?.dtOnNewLogListener?.();

      // Adicionar funcionalidade de arrastar para o user-details em telas pequenas
      function setupUserDetailsDrag() {
        const userDetails = document.querySelector('.user-info-container .user-details');
        if (!userDetails) return;

        let isDown = false;
        let startX;
        let scrollLeft;

        userDetails.addEventListener('mousedown', (e) => {
          isDown = true;
          userDetails.classList.add('dragging');
          startX = e.pageX - userDetails.offsetLeft;
          scrollLeft = userDetails.scrollLeft;
        });

        userDetails.addEventListener('mouseleave', () => {
          isDown = false;
          userDetails.classList.remove('dragging');
        });

        userDetails.addEventListener('mouseup', () => {
          isDown = false;
          userDetails.classList.remove('dragging');
        });

        userDetails.addEventListener('mousemove', (e) => {
          if (!isDown) return;
          e.preventDefault();
          const x = e.pageX - userDetails.offsetLeft;
          const walk = (x - startX) * 2; // Velocidade do arrasto
          userDetails.scrollLeft = scrollLeft - walk;
        });

        // Suporte para dispositivos móveis
        userDetails.addEventListener('touchstart', (e) => {
          isDown = true;
          userDetails.classList.add('dragging');
          startX = e.touches[0].pageX - userDetails.offsetLeft;
          scrollLeft = userDetails.scrollLeft;
        }, {
          passive: true
        });

        userDetails.addEventListener('touchend', () => {
          isDown = false;
          userDetails.classList.remove('dragging');
        });

        userDetails.addEventListener('touchmove', (e) => {
          if (!isDown) return;
          const x = e.touches[0].pageX - userDetails.offsetLeft;
          const walk = (x - startX) * 2;
          userDetails.scrollLeft = scrollLeft - walk;
        }, {
          passive: true
        });
      }

      // Inicializa o arrasto nos detalhes do usuário
      setupUserDetailsDrag();

      // Reconfigurar se o user-info for atualizado dinamicamente
      const observer = new MutationObserver(mutations => {
        mutations.forEach(mutation => {
          if (mutation.type === 'childList' &&
            (mutation.target.classList.contains('user-info-container') ||
              mutation.target.querySelector('.user-details'))) {
            setupUserDetailsDrag();
          }
        });
      });

      const userInfoContainer = document.querySelector('.user-info-container');
      if (userInfoContainer) {
        observer.observe(userInfoContainer, {
          childList: true,
          subtree: true
        });
      }
    });


    // --- Mock API for Browser Testing ---
    if (!window.DtGetVpnState) {
      console.log("Mocking DT API for browser testing.");
      let mockState = 'DISCONNECTED';
      const states = ['CONNECTING', 'CONNECTED'];
      let currentStateIndex = 0;

      window.DtGetVpnState = {
        execute: () => mockState
      };
      window.DtExecuteVpnStart = {
        execute: () => {
          mockState = states[0]; // CONNECTING
          dtVpnStateListener(mockState);
          setTimeout(() => {
            mockState = states[1]; // CONNECTED
            dtVpnStateListener(mockState);
          }, 2000);
        }
      };
      window.DtExecuteVpnStop = {
        execute: () => {
          mockState = 'STOPPING';
          dtVpnStateListener(mockState);
          setTimeout(() => {
            mockState = 'DISCONNECTED';
            dtVpnStateListener(mockState);
          }, 1000);
        }
      };
      window.DtGetLocalIP = {
        execute: () => '10.8.0.2'
      };
      window.DtGetConfigs = {
        execute: () => MOCK_CONFIGS
      };
      window.DtSetConfig = {
        execute: (id) => console.log(`Config set to ${id}`)
      };
      window.DtStartCheckUser = {
        execute: () => {
          window.dtCheckUserStartedListener();
          setTimeout(() => {
            window.dtCheckUserModelListener(JSON.stringify({
              username: 'mock_user',
              expiration_date: '2025-12-31',
              expiration_days: '365',
              count_connections: '1',
              limit_connections: '2'
            }));
          }, 1000);
        }
      };
      window.DtStartWebViewActivity = {
        execute: (url) => {
          console.log(`Opening WebView: ${url}`);
          showToast(`Abrindo: ${url.substring(0,30)}...`)
        }
      };
      window.DtGetLogs = {
        execute: () => JSON.stringify([{
          '[INFO]': 'Mock log entry 1'
        }, {
          '[DEBUG]': 'Another mock log entry'
        }])
      };
      window.DtStartAppUpdate = {
        execute: () => console.log('Checking for app updates...')
      };
      window.DtUsername = {
        get: () => localStorage.getItem('mockUser') || '',
        set: (val) => localStorage.setItem('mockUser', val)
      };
      window.DtPassword = {
        get: () => localStorage.getItem('mockPass') || '',
        set: (val) => localStorage.setItem('mockPass', val)
      };
      window.DtUuid = {
        get: () => localStorage.getItem('mockUuid') || '',
        set: (val) => localStorage.setItem('mockUuid', val)
      };
      window.DtClearLogs = {
        execute: () => console.log('Logs cleared.')
      };

      // Mock para hotspot
      let mockHotspotState = 'INACTIVE';
      window.DtGetStatusHotSpotService = {
        execute: () => mockHotspotState
      };
      window.DtStartHotSpotService = {
        execute: () => {
          console.log('Starting hotspot service...');
          mockHotspotState = 'ACTIVE';
          setTimeout(() => {
            window.onHotspotStateListener('ACTIVE');
          }, 1000);
        }
      };
      window.DtStopHotSpotService = {
        execute: () => {
          console.log('Stopping hotspot service...');
          mockHotspotState = 'INACTIVE';
          setTimeout(() => {
            window.onHotspotStateListener('INACTIVE');
          }, 1000);
        }
      };

      // Mock para gerenciar a configuração atual
      let mockCurrentConfig = JSON.parse(MOCK_CONFIGS)[0].items[0]; // Default to first item

      try {
        const savedConfig = localStorage.getItem('mockCurrentConfig');
        if (savedConfig) {
          mockCurrentConfig = JSON.parse(savedConfig);
        }
      } catch (e) {
        /* ignore */
      }

      window.DtGetDefaultConfig = {
        execute: () => JSON.stringify(mockCurrentConfig)
      };

      const originalDtSetConfig = window.DtSetConfig;
      if (!originalDtSetConfig) {
        window.DtSetConfig = {
          execute: (id) => {
            console.log(`Config set to ${id}`);
            const allConfigs = JSON.parse(MOCK_CONFIGS);
            for (const category of allConfigs) {
              const found = category.items.find(item => item.id === id);
              if (found) {
                mockCurrentConfig = found;
                localStorage.setItem('mockCurrentConfig', JSON.stringify(mockCurrentConfig));
                break;
              }
            }
          }
        };
      } else {
        // Estender a implementação original
        const originalExecute = originalDtSetConfig.execute;
        window.DtSetConfig.execute = (id) => {
          originalExecute(id);
          const allConfigs = JSON.parse(MOCK_CONFIGS);
          for (const category of allConfigs) {
            const found = category.items.find(item => item.id === id);
            if (found) {
              mockCurrentConfig = found;
              localStorage.setItem('mockCurrentConfig', JSON.stringify(mockCurrentConfig));
              break;
            }
          }
        };
      }
    }
  </script>

</body>
</html>
