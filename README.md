<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Ayu Cintya Nirmala ✦ Ruang Kecil Penuh Warna</title>

  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,600;9..144,700;9..144,900&family=Quicksand:wght@400;500;600;700&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" />

  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

    :root {
      --navy: #0a1a3c;
      --blue: #1e4fa3;
      --blue-soft: #4a7fd4;
      --sky: #dce9ff;
      --sky-soft: #eef4ff;
      --cream: #fffdf7;
      --sun: #ffc93c;
      --sun-soft: #ffe9a8;
      --sun-glow: #fff4cf;
      --honey: #e8a921;
      --pastel-yellow: #ffe9a8;
      --pink: #ffb3c6;
      --mint: #b8e6d9;
      --ink: #0a1a3c;
      --muted: #5a6b8c;
      --radius: 28px;
      --radius-sm: 16px;
      --shadow-soft: 0 20px 40px -20px rgba(30, 79, 163, 0.25);
    }

    html { scroll-behavior: smooth; }

    body {
      font-family: 'Quicksand', sans-serif;
      background: var(--cream);
      color: var(--ink);
      overflow-x: hidden;
      line-height: 1.6;
      position: relative;
      min-height: 100vh;
      overscroll-behavior-y: contain;
    }

    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background:
        radial-gradient(circle at 12% 18%, rgba(255, 233, 168, 0.2) 0%, transparent 35%),
        radial-gradient(circle at 88% 8%, rgba(74, 127, 212, 0.15) 0%, transparent 40%),
        radial-gradient(circle at 78% 92%, rgba(255, 233, 168, 0.15) 0%, transparent 35%),
        radial-gradient(circle at 5% 88%, rgba(30, 79, 163, 0.08) 0%, transparent 40%);
      z-index: -2;
      pointer-events: none;
    }

    .container { max-width: 1180px; margin: 0 auto; padding: 0 1.5rem; }

    h1, h2, h3 {
      font-family: 'Fraunces', serif;
      font-weight: 700;
      letter-spacing: -0.02em;
      line-height: 1.1;
      color: var(--navy);
    }

    @keyframes twinkle {
      0%, 100% { transform: scale(1) rotate(0deg); opacity: 0.8; }
      50% { transform: scale(1.25) rotate(20deg); opacity: 1; }
    }
    @keyframes float {
      0%, 100% { transform: translateY(0px) rotate(0deg); }
      50% { transform: translateY(-14px) rotate(4deg); }
    }
    @keyframes spin { to { transform: rotate(360deg); } }
    @keyframes beat {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.25); }
    }
    @keyframes sparkle {
      0%, 100% { opacity: 0.4; transform: scale(0.9); }
      50% { opacity: 1; transform: scale(1.1); }
    }
    @keyframes slideIn {
      from { opacity: 0; transform: translateY(20px) scale(0.95); }
      to { opacity: 1; transform: translateY(0) scale(1); }
    }
    @keyframes eq {
      0%, 100% { height: 6px; }
      50% { height: 18px; }
    }
    @keyframes fall {
      0%   { transform: translateY(0) rotate(0deg); opacity: 0; }
      10%  { opacity: 0.85; }
      90%  { opacity: 0.85; }
      100% { transform: translateY(105vh) rotate(720deg); opacity: 0; }
    }
    @keyframes floatCream {
      0%, 100% { transform: translateY(0) rotate(-3deg); }
      50%      { transform: translateY(-18px) rotate(3deg); }
    }
    @keyframes floatStar {
      0%, 100% { transform: translateY(0) rotate(0deg); }
      50%      { transform: translateY(-20px) rotate(8deg); }
    }

    .doodle-star {
      color: var(--sun);
      font-size: 1.4rem;
      animation: twinkle 3s ease-in-out infinite;
    }

    .sparkle {
      position: absolute;
      color: var(--sun);
      animation: sparkle 2.5s ease-in-out infinite;
      pointer-events: none;
      z-index: 2;
      font-size: 1.2rem;
    }

    /* ============ BINTANG POLKADOT HALFTONE (LAYER BELAKANG) ============ */
    .star-deco {
      position: absolute;
      pointer-events: none;
      z-index: 0;
      opacity: 0.55;
      filter: drop-shadow(0 8px 20px rgba(74, 127, 212, 0.15));
      animation: floatStar 10s ease-in-out infinite;
    }
    .star-deco svg { display: block; width: 100%; height: 100%; }
    .star-deco.s-1 { top: 400px; left: 4%; width: 90px; height: 90px; animation-delay: 0s; }
    .star-deco.s-2 { top: 900px; right: 5%; width: 80px; height: 80px; animation-delay: 1s; }
    .star-deco.s-3 { top: 1500px; left: 3%; width: 85px; height: 85px; animation-delay: 2s; }
    .star-deco.s-4 { top: 2100px; right: 4%; width: 100px; height: 100px; animation-delay: 1.5s; }
    .star-deco.s-5 { top: 2800px; left: 6%; width: 75px; height: 75px; animation-delay: 2.5s; }
    .star-deco.s-6 { top: 3400px; left: 48%; width: 70px; height: 70px; animation-delay: 3s; }

    /* ============ INTRO ANIMASI NAMA AYU ============ */
    .intro-overlay {
      position: fixed;
      inset: 0;
      background: linear-gradient(135deg, #fffdf7 0%, #eef4ff 50%, #fff4cf 100%);
      z-index: 99999;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
      transition: opacity 0.8s ease, visibility 0.8s ease;
    }
    .intro-overlay.hide { opacity: 0; visibility: hidden; }
    .intro-overlay::before {
      content: '';
      position: absolute;
      inset: 0;
      background-color: #ffe9a8;
      background-image:
        radial-gradient(circle, #a8c8ff 18%, transparent 20%),
        radial-gradient(circle, #b8e6d9 18%, transparent 20%);
      background-size: 40px 40px, 40px 40px;
      background-position: 0 0, 20px 20px;
      opacity: 0.5;
      z-index: 0;
    }
    .intro-overlay::after {
      content: '';
      position: absolute;
      inset: 0;
      background: radial-gradient(circle at center,
        rgba(255, 253, 247, 0.95) 0%,
        rgba(255, 253, 247, 0.7) 40%,
        rgba(255, 253, 247, 0.4) 100%);
      z-index: 1;
    }
    .intro-content {
      position: relative;
      z-index: 3;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 0.3rem;
      padding: 2rem;
      transform-origin: center center;
    }
    .intro-content.jelly {
      animation: jellyBounce 1.5s ease-in-out 3.7s;
    }
    @keyframes jellyBounce {
      0%   { transform: scale(1, 1); }
      15%  { transform: scale(1.1, 0.9); }
      30%  { transform: scale(0.9, 1.1); }
      45%  { transform: scale(1.05, 0.95); }
      60%  { transform: scale(0.95, 1.05); }
      75%  { transform: scale(1.02, 0.98); }
      100% { transform: scale(1, 1); }
    }
    .intro-letter {
      font-family: 'Fraunces', serif;
      font-weight: 900;
      font-size: clamp(5rem, 18vw, 12rem);
      color: #1e4fa3;
      line-height: 1;
      display: inline-block;
      opacity: 0;
      transform: scale(0.3);
      text-shadow:
        0 8px 30px rgba(30, 79, 163, 0.4),
        0 0 40px rgba(74, 127, 212, 0.3);
      position: relative;
      transform-origin: center;
      will-change: transform, opacity, filter;
    }
    .intro-letter.letter-a {
      animation: waveFromLeft 2.8s cubic-bezier(0.45, 0, 0.55, 1) 0.3s forwards;
    }
    .intro-letter.letter-y {
      animation: waveFromTop 2.8s cubic-bezier(0.45, 0, 0.55, 1) 0.7s forwards;
    }
    .intro-letter.letter-u {
      animation: waveFromRight 2.8s cubic-bezier(0.45, 0, 0.55, 1) 1.1s forwards;
    }

    @keyframes waveFromLeft {
      0%   { opacity: 0; transform: translate(-500px, 100px) rotate(-200deg) scale(0.1); filter: blur(20px); }
      10%  { opacity: 0.3; transform: translate(-420px, -120px) rotate(-160deg) scale(0.25); filter: blur(14px); }
      20%  { opacity: 0.5; transform: translate(-350px, 150px) rotate(-120deg) scale(0.4); filter: blur(10px); }
      30%  { opacity: 0.7; transform: translate(-280px, -100px) rotate(-80deg) scale(0.55); filter: blur(7px); }
      40%  { opacity: 0.85; transform: translate(-210px, 120px) rotate(-40deg) scale(0.7); filter: blur(4px); }
      50%  { transform: translate(-150px, -80px) rotate(0deg) scale(0.82); filter: blur(2px); }
      60%  { transform: translate(-100px, 90px) rotate(30deg) scale(0.9); filter: blur(1px); }
      70%  { transform: translate(-60px, -50px) rotate(50deg) scale(0.96); filter: blur(0); }
      80%  { transform: translate(-30px, 40px) rotate(30deg) scale(1.02); filter: blur(0); }
      90%  { transform: translate(-10px, -15px) rotate(10deg) scale(1.04); filter: blur(0); }
      100% { opacity: 1; transform: translate(0, 0) rotate(0deg) scale(1); filter: blur(0); }
    }
    @keyframes waveFromTop {
      0%   { opacity: 0; transform: translate(150px, -500px) rotate(200deg) scale(0.1); filter: blur(20px); }
      10%  { opacity: 0.3; transform: translate(-180px, -420px) rotate(160deg) scale(0.25); filter: blur(14px); }
      20%  { opacity: 0.5; transform: translate(200px, -350px) rotate(120deg) scale(0.4); filter: blur(10px); }
      30%  { opacity: 0.7; transform: translate(-150px, -280px) rotate(80deg) scale(0.55); filter: blur(7px); }
      40%  { opacity: 0.85; transform: translate(170px, -210px) rotate(40deg) scale(0.7); filter: blur(4px); }
      50%  { transform: translate(-120px, -150px) rotate(0deg) scale(0.82); filter: blur(2px); }
      60%  { transform: translate(130px, -100px) rotate(-30deg) scale(0.9); filter: blur(1px); }
      70%  { transform: translate(-70px, -60px) rotate(-50deg) scale(0.96); filter: blur(0); }
      80%  { transform: translate(60px, -30px) rotate(-30deg) scale(1.02); filter: blur(0); }
      90%  { transform: translate(-20px, -10px) rotate(-10deg) scale(1.04); filter: blur(0); }
      100% { opacity: 1; transform: translate(0, 0) rotate(0deg) scale(1); filter: blur(0); }
    }
    @keyframes waveFromRight {
      0%   { opacity: 0; transform: translate(500px, 100px) rotate(200deg) scale(0.1); filter: blur(20px); }
      10%  { opacity: 0.3; transform: translate(420px, -120px) rotate(160deg) scale(0.25); filter: blur(14px); }
      20%  { opacity: 0.5; transform: translate(350px, 150px) rotate(120deg) scale(0.4); filter: blur(10px); }
      30%  { opacity: 0.7; transform: translate(280px, -100px) rotate(80deg) scale(0.55); filter: blur(7px); }
      40%  { opacity: 0.85; transform: translate(210px, 120px) rotate(40deg) scale(0.7); filter: blur(4px); }
      50%  { transform: translate(150px, -80px) rotate(0deg) scale(0.82); filter: blur(2px); }
      60%  { transform: translate(100px, 90px) rotate(-30deg) scale(0.9); filter: blur(1px); }
      70%  { transform: translate(60px, -50px) rotate(-50deg) scale(0.96); filter: blur(0); }
      80%  { transform: translate(30px, 40px) rotate(-30deg) scale(1.02); filter: blur(0); }
      90%  { transform: translate(10px, -15px) rotate(-10deg) scale(1.04); filter: blur(0); }
      100% { opacity: 1; transform: translate(0, 0) rotate(0deg) scale(1); filter: blur(0); }
    }

    .intro-sparkle {
      position: absolute;
      width: 20px; height: 20px;
      background: #ffc93c;
      border-radius: 50%;
      opacity: 0;
      box-shadow: 0 0 20px #ffc93c, 0 0 40px #ffd93d, 0 0 60px rgba(255, 201, 60, 0.6);
      animation: sparklePopup 2s ease-out infinite;
      z-index: 2;
      pointer-events: none;
    }
    .intro-sparkle::before,
    .intro-sparkle::after {
      content: '';
      position: absolute; top: 50%; left: 50%;
      background: #ffc93c; border-radius: 50%;
      transform: translate(-50%, -50%);
      box-shadow: 0 0 15px #ffc93c;
    }
    .intro-sparkle::before { width: 4px; height: 100%; }
    .intro-sparkle::after { width: 100%; height: 4px; }
    .intro-sparkle.s1  { top: 15%; left: 10%; animation-delay: 0.2s; }
    .intro-sparkle.s2  { top: 25%; right: 12%; animation-delay: 0.5s; }
    .intro-sparkle.s3  { bottom: 20%; left: 15%; animation-delay: 0.8s; }
    .intro-sparkle.s4  { bottom: 15%; right: 18%; animation-delay: 1.1s; }
    .intro-sparkle.s5  { top: 10%; left: 50%; animation-delay: 1.4s; }
    .intro-sparkle.s6  { bottom: 10%; left: 40%; animation-delay: 1.7s; }
    .intro-sparkle.s7  { top: 50%; left: 8%;  animation-delay: 0.9s; }
    .intro-sparkle.s8  { top: 55%; right: 8%; animation-delay: 1.3s; }
    .intro-sparkle.s9  { top: 70%; left: 25%; animation-delay: 0.6s; }
    .intro-sparkle.s10 { top: 75%; right: 30%; animation-delay: 1.9s; }
    @keyframes sparklePopup {
      0%   { transform: scale(0) rotate(0deg); opacity: 0; }
      30%  { transform: scale(1.3) rotate(90deg); opacity: 1; }
      50%  { transform: scale(1) rotate(180deg); opacity: 0.9; }
      100% { transform: scale(0.4) rotate(360deg); opacity: 0; }
    }
    .intro-star {
      position: absolute;
      color: #ffc93c;
      font-size: 2rem;
      animation: starBlink 1.5s ease-in-out infinite;
      z-index: 2;
      pointer-events: none;
      filter: drop-shadow(0 0 10px #ffc93c);
    }
    .intro-star.st1 { top: 20%; left: 25%; animation-delay: 0.3s; }
    .intro-star.st2 { top: 30%; right: 22%; animation-delay: 0.7s; }
    .intro-star.st3 { bottom: 28%; left: 20%; animation-delay: 1.1s; }
    .intro-star.st4 { bottom: 22%; right: 25%; animation-delay: 1.5s; }
    @keyframes starBlink {
      0%, 100% { transform: scale(0.5) rotate(0deg); opacity: 0.3; }
      50%      { transform: scale(1.2) rotate(180deg); opacity: 1; }
    }
    .intro-skip {
      position: absolute;
      bottom: 3rem; right: 3rem;
      background: rgba(255, 253, 247, 0.9);
      border: 2px dashed #1e4fa3;
      color: #1e4fa3;
      padding: 0.7rem 1.4rem;
      border-radius: 50px;
      font-family: 'Quicksand', sans-serif;
      font-weight: 700; font-size: 0.9rem;
      cursor: pointer; z-index: 10;
      transition: all 0.3s ease;
      opacity: 0;
      animation: fadeInSkip 0.5s ease 2s forwards;
      display: flex; align-items: center; gap: 0.5rem;
    }
    .intro-skip:hover {
      background: #ffe9a8;
      color: #0a1a3c;
      transform: translateY(-3px) scale(1.05);
    }
    @keyframes fadeInSkip { to { opacity: 1; } }
    @media (max-width: 480px) {
      .intro-letter { font-size: 6rem; }
      .intro-skip { bottom: 2rem; right: 1rem; padding: 0.6rem 1.1rem; font-size: 0.8rem; }
      .intro-sparkle { width: 14px; height: 14px; }
      .intro-star { font-size: 1.4rem; }
    }

    /* NAVBAR */
    nav {
      position: sticky;
      top: 0;
      z-index: 50;
      backdrop-filter: blur(14px);
      background: rgba(255, 253, 247, 0.78);
      border-bottom: 1px solid rgba(30, 79, 163, 0.08);
    }
    .nav-inner {
      display: flex; align-items: center; justify-content: space-between;
      padding: 1rem 1.5rem; max-width: 1180px; margin: 0 auto;
    }
    .logo {
      display: flex; align-items: center; gap: 0.6rem;
      font-family: 'Fraunces', serif; font-weight: 700;
      font-size: 1.35rem; color: var(--navy); text-decoration: none;
    }
    .logo-mark {
      width: 40px; height: 40px; border-radius: 12px;
      background: linear-gradient(135deg, var(--blue) 0%, var(--blue-soft) 100%);
      display: grid; place-items: center;
      color: var(--sun); font-size: 1.1rem;
      box-shadow: 0 8px 16px -6px rgba(30, 79, 163, 0.5);
      transform: rotate(-6deg); transition: transform 0.3s;
    }
    .logo:hover .logo-mark { transform: rotate(6deg) scale(1.05); }
    .nav-links { display: flex; gap: 1.6rem; align-items: center; }
    .nav-links a {
      text-decoration: none; color: var(--muted); font-weight: 600;
      font-size: 0.9rem; position: relative; transition: color 0.25s;
    }
    .nav-links a::after {
      content: ''; position: absolute; left: 0; bottom: -6px;
      width: 0; height: 3px; border-radius: 3px; background: var(--sun);
      transition: width 0.3s ease;
    }
    .nav-links a:hover { color: var(--blue); }
    .nav-links a:hover::after { width: 100%; }

    .btn {
      display: inline-flex; align-items: center; gap: 0.5rem;
      padding: 0.8rem 1.6rem; border-radius: 50px;
      font-family: 'Quicksand', sans-serif; font-weight: 700;
      font-size: 0.95rem; text-decoration: none; border: none;
      cursor: pointer; transition: all 0.28s ease; white-space: nowrap;
    }
    .btn-primary {
      background: linear-gradient(135deg, var(--blue) 0%, var(--blue-soft) 100%);
      color: #fff;
      box-shadow: 0 12px 24px -10px rgba(30, 79, 163, 0.6);
    }
    .btn-primary:hover {
      transform: translateY(-3px) scale(1.02);
      box-shadow: 0 18px 30px -10px rgba(30, 79, 163, 0.7);
    }
    .btn-sun {
      background: linear-gradient(135deg, var(--sun) 0%, var(--honey) 100%);
      color: var(--navy);
      box-shadow: 0 12px 24px -10px rgba(255, 201, 60, 0.8);
    }
    .btn-sun:hover {
      transform: translateY(-3px) scale(1.02) rotate(-1deg);
      box-shadow: 0 18px 30px -8px rgba(255, 201, 60, 0.9);
    }

    .section-head {
      text-align: center; max-width: 720px;
      margin: 0 auto 3.5rem; position: relative;
    }
    .section-head .kicker {
      display: inline-block; font-size: 0.85rem; font-weight: 700;
      letter-spacing: 0.15em; text-transform: uppercase;
      color: var(--honey); margin-bottom: 0.8rem;
    }
    .section-head .kicker::before,
    .section-head .kicker::after {
      content: '✦'; margin: 0 0.6rem; color: var(--sun); font-size: 0.7rem;
    }
    .section-head h2 { font-size: clamp(2rem, 4vw, 2.8rem); margin-bottom: 1rem; }
    .section-head p { color: var(--muted); font-size: 1.05rem; font-weight: 500; }

    /* HERO */
    .hero {
      position: relative;
      padding: 5rem 0 6rem;
      overflow: hidden;
      background-color: #ffe9a8;
      background-image:
        radial-gradient(circle, #a8c8ff 18%, transparent 20%),
        radial-gradient(circle, #b8e6d9 18%, transparent 20%);
      background-size: 36px 36px, 36px 36px;
      background-position: 0 0, 18px 18px;
    }
    .hero::before {
      content: '';
      position: absolute; inset: 0;
      background: linear-gradient(180deg,
        rgba(255, 233, 168, 0.5) 0%,
        rgba(255, 253, 247, 0.75) 35%,
        rgba(255, 253, 247, 0.95) 65%,
        #fffdf7 100%);
      z-index: 0;
      pointer-events: none;
    }
    .hero > * { position: relative; z-index: 1; }
    .hero .container { position: relative; z-index: 3; }
    .hero-grid {
      display: grid; grid-template-columns: 1.15fr 1fr;
      gap: 4rem; align-items: center; position: relative; z-index: 3;
    }
    .hero-badge {
      display: inline-flex; align-items: center; gap: 0.6rem;
      background: #fff; border: 1.5px dashed var(--sun);
      color: var(--blue); padding: 0.5rem 1.1rem; border-radius: 50px;
      font-size: 0.85rem; font-weight: 700; margin-bottom: 1.8rem;
      box-shadow: 0 8px 20px -12px rgba(30, 79, 163, 0.4);
    }
    .hero-badge i { color: var(--honey); }
    .hero h1 { font-size: clamp(2.6rem, 5.5vw, 4.5rem); margin-bottom: 1.5rem; }
    .hero h1 .highlight { position: relative; display: inline-block; color: var(--blue); }
    .hero h1 .highlight::after {
      content: ''; position: absolute; left: -4%; right: -4%; bottom: 6%;
      height: 22%; background: var(--sun-soft); z-index: -1;
      border-radius: 6px; transform: rotate(-1.5deg);
    }
    .hero p.lead {
      font-size: 1.15rem; color: var(--muted);
      max-width: 90%; margin-bottom: 2.5rem; font-weight: 500;
    }
    .hero-visual {
      position: relative; display: flex;
      justify-content: center; align-items: center; padding: 2rem;
    }
    .profile-card {
      position: relative; width: 100%; max-width: 380px;
      background: #fff; border-radius: var(--radius);
      padding: 2.5rem 2rem 2rem; box-shadow: var(--shadow-soft);
      border: 1px solid rgba(30, 79, 163, 0.08);
      text-align: center; z-index: 4;
      transform: rotate(-1.5deg); transition: transform 0.4s ease;
    }
    .profile-card:hover { transform: rotate(0deg) translateY(-6px); }
    .avatar-ring {
      width: 130px; height: 130px; margin: 0 auto 1.5rem;
      border-radius: 50%;
      background: linear-gradient(135deg, var(--sun) 0%, var(--blue-soft) 100%);
      padding: 5px; position: relative;
      box-shadow: 0 15px 30px -12px rgba(255, 201, 60, 0.7);
    }
    .avatar-ring::before {
      content: ''; position: absolute; inset: -8px; border-radius: 50%;
      border: 2px dashed var(--sun); animation: spin 18s linear infinite;
    }
    .avatar {
      width: 100%; height: 100%; border-radius: 50%;
      background: linear-gradient(160deg, var(--sky) 0%, var(--sky-soft) 60%, #fff 100%);
      display: grid; place-items: center;
      font-family: 'Fraunces', serif; font-size: 3.2rem;
      font-weight: 700; color: var(--blue); border: 4px solid #fff;
      overflow: hidden;
    }
    .avatar img { width: 100%; height: 100%; object-fit: cover; object-position: center top; }
    .profile-card h3 { font-size: 1.6rem; margin-bottom: 0.25rem; }
    .profile-card .role {
      color: var(--honey); font-weight: 700; font-size: 0.9rem;
      letter-spacing: 0.05em; text-transform: uppercase; margin-bottom: 1.2rem;
    }
    .profile-card .quote {
      font-size: 0.95rem; color: var(--muted); font-style: italic;
      line-height: 1.6; padding: 0 0.5rem; margin-bottom: 1.5rem;
    }
    .chips { display: flex; flex-wrap: wrap; gap: 0.5rem; justify-content: center; }
    .chip {
      background: var(--sky-soft); color: var(--blue);
      padding: 0.4rem 0.9rem; border-radius: 50px;
      font-size: 0.8rem; font-weight: 700;
      transition: all 0.25s ease; border: 1px solid transparent;
    }
    .chip:hover {
      background: var(--sun-soft); color: var(--navy);
      transform: translateY(-2px); border-color: var(--sun);
    }
    .chip i { margin-right: 4px; color: var(--honey); }
    .float-card {
      position: absolute; background: #fff; border-radius: var(--radius-sm);
      padding: 0.8rem 1.1rem;
      box-shadow: 0 15px 30px -12px rgba(30, 79, 163, 0.35);
      font-weight: 700; font-size: 0.85rem; color: var(--blue);
      display: flex; align-items: center; gap: 0.5rem;
      z-index: 5; border: 1px solid rgba(30, 79, 163, 0.08);
    }
    .float-card i { color: var(--honey); font-size: 1.1rem; }
    .fc-1 { top: 2%; left: -12%; animation: float 5s ease-in-out infinite; }
    .fc-2 { bottom: 8%; right: -14%; animation: float 6s ease-in-out infinite 0.5s; }
    .fc-3 { bottom: -6%; left: 4%; animation: float 7s ease-in-out infinite 1s; }

    /* BANNER POLKADOT */
    .polkadot-banner {
      position: relative;
      width: 100%;
      height: 90px;
      background-color: #ffe9a8;
      background-image:
        radial-gradient(circle, #4a7fd4 22%, transparent 24%),
        radial-gradient(circle, #a8c8ff 22%, transparent 24%);
      background-size: 40px 40px, 40px 40px;
      background-position: 0 0, 20px 20px;
      border-top: 5px dashed #4a7fd4;
      border-bottom: 5px dashed #4a7fd4;
      display: flex; align-items: center; justify-content: center;
      overflow: hidden;
      box-shadow: 0 10px 30px -15px rgba(74, 127, 212, 0.3);
      margin: 0; z-index: 5;
    }
    .polkadot-banner::before {
      content: '';
      position: absolute; inset: 0;
      background: linear-gradient(90deg,
        rgba(255, 253, 247, 0.5) 0%,
        rgba(255, 253, 247, 0) 20%,
        rgba(255, 253, 247, 0) 80%,
        rgba(255, 253, 247, 0.5) 100%);
      pointer-events: none;
    }
    .polkadot-banner-text {
      position: relative;
      font-family: 'Fraunces', serif;
      font-style: italic;
      font-weight: 700;
      font-size: 1.15rem;
      letter-spacing: 0.25em;
      color: #1e4fa3;
      text-transform: uppercase;
      padding: 0.5rem 1.5rem;
      background: rgba(255, 253, 247, 0.95);
      border-radius: 50px;
      border: 3px dashed #4a7fd4;
      box-shadow: 0 8px 20px -10px rgba(74, 127, 212, 0.4);
      animation: float 5s ease-in-out infinite;
      display: flex; align-items: center; gap: 0.8rem;
      z-index: 2;
    }
    .polkadot-banner-text i { color: #4a7fd4; font-size: 1rem; }
    .polkadot-banner-text i:last-child { color: #e8a921; }
    .polkadot-banner.thin { height: 55px; }
    .polkadot-banner.thin .polkadot-banner-text {
      font-size: 0.85rem;
      letter-spacing: 0.3em;
      padding: 0.35rem 1.2rem;
    }

    /* SPRINKLE JATUH */
    .sprinkle-layer {
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 40;
      overflow: hidden;
    }
    .sprinkle {
      position: absolute;
      top: -30px;
      width: 9px;
      height: 16px;
      border-radius: 4px;
      opacity: 0;
      animation: fall linear infinite;
      box-shadow: 0 0 6px rgba(255, 233, 168, 0.4);
    }
    .sprinkle.round { width: 11px; height: 11px; border-radius: 50%; }
    .sprinkle.square { width: 11px; height: 11px; border-radius: 3px; }
    .sprinkle.long { width: 6px; height: 15px; border-radius: 3px; }

    /* KRIM KUE */
    .cream-float {
      position: fixed;
      pointer-events: auto;
      z-index: 4;
      animation: floatCream 7s ease-in-out infinite;
      filter: drop-shadow(0 8px 12px rgba(30, 79, 163, 0.2));
      cursor: grab;
      touch-action: none;
      user-select: none;
      -webkit-user-select: none;
      transition: transform 0.15s ease;
      opacity: 0.85;
    }
    .cream-float:hover { opacity: 1; }
    .cream-float:active,
    .cream-float.dragging {
      cursor: grabbing;
      animation: none;
      transform: scale(1.1);
      z-index: 9999 !important;
      opacity: 1;
    }
    .cream-float svg { display: block; }

    /* SPRINKLE STATIS */
    .sprinkle-static {
      position: fixed;
      width: 11px;
      height: 11px;
      border-radius: 50%;
      pointer-events: auto;
      z-index: 3;
      animation: sparkle 4s ease-in-out infinite;
      cursor: grab;
      touch-action: none;
      user-select: none;
      -webkit-user-select: none;
      transition: transform 0.15s ease;
      opacity: 0.75;
    }
    .sprinkle-static:hover { opacity: 1; }
    .sprinkle-static:active,
    .sprinkle-static.dragging {
      cursor: grabbing;
      animation: none;
      transform: scale(1.3);
      z-index: 9999 !important;
      opacity: 1;
    }
    .sprinkle-static.pill { width: 6px; height: 14px; border-radius: 3px; }

    /* CONTENT PAGE */
    .content-page {
      padding: 4rem 0 5rem;
      position: relative;
      background: linear-gradient(180deg, transparent 0%, var(--sky-soft) 40%, transparent 100%);
      overflow: hidden;
    }
    .content-grid {
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      gap: 1rem;
      position: relative; z-index: 3;
      margin-top: 1rem;
    }
    .content-card {
      background: #fff;
      border-radius: var(--radius-sm);
      padding: 1.3rem 1rem;
      text-decoration: none;
      color: var(--navy);
      box-shadow: 0 15px 30px -20px rgba(30, 79, 163, 0.3);
      border: 2px solid transparent;
      transition: all 0.3s ease;
      display: flex; flex-direction: column;
      align-items: center; text-align: center;
      gap: 0.6rem;
      position: relative; overflow: hidden;
      cursor: pointer;
    }
    .content-card::before {
      content: '';
      position: absolute; top: -30px; right: -30px;
      width: 80px; height: 80px;
      border-radius: 50%;
      background: radial-gradient(circle, var(--sun-glow), transparent 70%);
      opacity: 0.7; pointer-events: none;
    }
    .content-card:hover {
      transform: translateY(-6px) rotate(-0.5deg);
      border-color: var(--sun);
      box-shadow: 0 25px 40px -20px rgba(30, 79, 163, 0.5);
    }
    .content-card:hover .content-num {
      background: var(--sun);
      color: var(--navy);
      transform: rotate(8deg) scale(1.12);
    }
    .content-num {
      width: 42px; height: 42px;
      border-radius: 14px;
      display: grid; place-items: center;
      font-family: 'Fraunces', serif;
      font-weight: 700; font-size: 1rem;
      background: var(--blue); color: var(--sun);
      transition: all 0.3s ease; flex-shrink: 0;
    }
    .content-title {
      font-family: 'Fraunces', serif;
      font-weight: 700; font-size: 0.9rem;
      color: var(--navy); line-height: 1.2;
    }
    .content-card.c-about .content-num { background: linear-gradient(135deg, var(--blue), var(--blue-soft)); }
    .content-card.c-nama .content-num { background: linear-gradient(135deg, var(--blue), var(--sky)); }
    .content-card.c-things .content-num { background: linear-gradient(135deg, var(--sun), var(--honey)); color: var(--navy); }
    .content-card.c-funfact .content-num { background: linear-gradient(135deg, var(--pink), var(--sun-soft)); color: var(--navy); }
    .content-card.c-warna .content-num {
      background: conic-gradient(#ff6b6b, #ffd93d, #4ecdc4, #4a7fd4, #a78bfa, #ffb3c6, #ff6b6b);
      color: #fff;
    }
    .content-card.c-mbti .content-num { background: linear-gradient(135deg, var(--pink), var(--mint)); color: var(--navy); }
    .content-card.c-hobi .content-num { background: linear-gradient(135deg, var(--blue), var(--sky)); color: var(--sun); }
    .content-card.c-makanan .content-num { background: linear-gradient(135deg, var(--sun-soft), var(--pink)); color: var(--navy); }
    .content-card.c-mood .content-num { background: linear-gradient(135deg, var(--mint), var(--sky)); color: var(--blue); }
    .content-card.c-comment .content-num { background: linear-gradient(135deg, var(--navy), var(--blue)); color: var(--sun); }

    /* ABOUT */
    .about { padding: 5rem 0; position: relative; overflow: hidden; }
    .about-grid {
      display: grid; grid-template-columns: 1fr 1.2fr;
      gap: 3.5rem; align-items: center;
      position: relative; z-index: 3;
    }
    .about-visual { position: relative; height: 100%; min-height: 420px; }
    .about-img-main {
      width: 78%; height: 340px; top: 8%; left: 0;
      transform: rotate(-3deg); animation: float 7s ease-in-out infinite;
      position: absolute; border-radius: 20px; overflow: hidden;
      box-shadow: 0 20px 40px -18px rgba(30, 79, 163, 0.4);
      border: 4px solid #fff;
      outline: 2px dashed var(--sun); outline-offset: 4px;
    }
    .about-img-main img { width: 100%; height: 100%; object-fit: cover; display: block; }
    .about-img-secondary {
      width: 55%; height: 200px; bottom: 0; right: 0;
      transform: rotate(5deg);
      border: 4px solid #fff;
      outline: 2px dashed var(--sun); outline-offset: 4px;
      animation: float 6s ease-in-out infinite 0.5s;
      position: absolute; border-radius: 20px; overflow: hidden;
      box-shadow: 0 20px 40px -18px rgba(30, 79, 163, 0.4);
    }
    .about-img-secondary img { width: 100%; height: 100%; object-fit: cover; display: block; }
    .about-content h2 { font-size: clamp(1.8rem, 3.5vw, 2.5rem); margin-bottom: 1.2rem; }
    .about-content .blue-philosophy {
      background: linear-gradient(135deg, var(--sky-soft) 0%, #fff 100%);
      border-left: 5px solid var(--sun);
      border-radius: 0 var(--radius-sm) var(--radius-sm) 0;
      padding: 1.3rem 1.5rem; margin: 1.5rem 0;
      font-size: 1rem; color: var(--navy); font-weight: 500;
      box-shadow: 0 10px 25px -15px rgba(30, 79, 163, 0.3);
    }
    .about-content .blue-philosophy i {
      color: var(--blue); font-size: 1.3rem; margin-right: 0.6rem;
      vertical-align: middle;
    }
    .about-content .blue-philosophy strong {
      color: var(--blue); font-family: 'Fraunces', serif; font-style: italic;
    }
    .about-text { color: var(--muted); font-weight: 500; font-size: 1.02rem; margin-bottom: 1.5rem; }

    /* BIODATA */
    .biodata {
      display: grid; grid-template-columns: 1fr 1fr;
      gap: 0.9rem; margin: 1.5rem 0;
    }
    .bio-item {
      display: flex; align-items: center; gap: 0.9rem;
      padding: 0.9rem 1.1rem;
      background: linear-gradient(135deg, var(--sky-soft) 0%, #fff 100%);
      border-radius: var(--radius-sm);
      border: 2px solid rgba(30, 79, 163, 0.08);
      transition: all 0.3s ease;
      position: relative; overflow: hidden;
    }
    .bio-item::before {
      content: '';
      position: absolute; top: -20px; right: -20px;
      width: 70px; height: 70px;
      border-radius: 50%;
      background: radial-gradient(circle, var(--sun-glow), transparent 70%);
      opacity: 0.6; pointer-events: none;
    }
    .bio-item:hover {
      transform: translateY(-3px);
      border-color: var(--sun);
      box-shadow: 0 12px 25px -15px rgba(30, 79, 163, 0.4);
    }
    .bio-icon {
      width: 44px; height: 44px;
      border-radius: 12px;
      background: linear-gradient(135deg, var(--blue), var(--blue-soft));
      color: var(--sun);
      display: grid; place-items: center;
      font-size: 1.1rem; flex-shrink: 0;
      box-shadow: 0 8px 16px -8px rgba(30, 79, 163, 0.5);
      transition: transform 0.3s ease;
      position: relative; z-index: 1;
    }
    .bio-item:hover .bio-icon { transform: rotate(-8deg) scale(1.08); }
    .bio-info {
      display: flex; flex-direction: column;
      line-height: 1.3;
      position: relative; z-index: 1;
      min-width: 0;
    }
    .bio-label {
      font-family: 'Quicksand', sans-serif;
      font-size: 0.7rem; font-weight: 700;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--honey);
      margin-bottom: 0.15rem;
    }
    .bio-value {
      font-family: 'Quicksand', sans-serif;
      font-size: 0.85rem; font-weight: 700;
      color: var(--navy);
      line-height: 1.35;
    }

    /* NAMA */
    .nama { padding: 5rem 0; position: relative; overflow: hidden; }
    .nama-grid {
      display: grid; grid-template-columns: 1fr 1.1fr;
      gap: 3.5rem; align-items: center;
      position: relative; z-index: 3;
    }
    .nama-visual {
      position: relative; min-height: 460px;
      display: flex; justify-content: center; align-items: center;
    }
    .nama-circle {
      width: 340px; height: 340px; border-radius: 50%;
      background: linear-gradient(135deg, var(--sky) 0%, var(--sky-soft) 100%);
      display: grid; place-items: center; position: relative;
      box-shadow: 0 30px 60px -25px rgba(30, 79, 163, 0.4);
      border: 3px dashed var(--sun);
      animation: float 8s ease-in-out infinite;
    }
    .nama-circle::before {
      content: ''; position: absolute; inset: -20px;
      border-radius: 50%; border: 2px dotted var(--blue-soft);
      animation: spin 30s linear infinite;
    }
    .nama-word { font-family: 'Fraunces', serif; text-align: center; line-height: 1.1; padding: 0 1rem; }
    .nama-word .nama-kecil {
      display: block; font-size: 1rem; font-weight: 600;
      color: var(--blue-soft); letter-spacing: 0.2em;
      text-transform: uppercase; margin-bottom: 0.3rem;
    }
    .nama-word .nama-besar { display: block; font-size: 3rem; font-weight: 700; color: var(--blue); }
    .nama-word small {
      display: block; font-size: 0.75rem; color: var(--honey);
      font-family: 'Quicksand', sans-serif; font-weight: 700;
      letter-spacing: 0.15em; text-transform: uppercase; margin-top: 0.7rem;
    }
    .nama-tag-float {
      position: absolute; background: #fff; border-radius: 50px;
      padding: 0.6rem 1.1rem; font-size: 0.8rem; font-weight: 700;
      color: var(--blue);
      box-shadow: 0 12px 25px -12px rgba(30, 79, 163, 0.5);
      border: 1px solid rgba(30, 79, 163, 0.08);
      display: flex; align-items: center; gap: 0.4rem;
    }
    .nama-tag-float i { color: var(--honey); }
    .nama-tag-1 { top: 6%; left: 0; animation: float 5s ease-in-out infinite; }
    .nama-tag-2 { bottom: 10%; right: 0; animation: float 6s ease-in-out infinite 0.5s; }
    .nama-tag-3 { bottom: 4%; left: 2%; animation: float 7s ease-in-out infinite 1s; }
    .nama-content h2 { font-size: clamp(1.8rem, 3.5vw, 2.5rem); margin-bottom: 1.2rem; }
    .nama-content p {
      color: var(--muted); font-weight: 500;
      font-size: 1rem; margin-bottom: 1.2rem; line-height: 1.7;
    }
    .nama-content strong { color: var(--blue); font-weight: 700; }
    .nama-content em { color: var(--honey); font-style: italic; font-weight: 600; }
    .nama-quote {
      background: linear-gradient(135deg, var(--sun-glow) 0%, #fff 100%);
      border-left: 5px solid var(--blue);
      border-radius: 0 var(--radius-sm) var(--radius-sm) 0;
      padding: 1.3rem 1.5rem; margin: 1.5rem 0;
      font-family: 'Fraunces', serif; font-style: italic;
      font-size: 1.05rem; color: var(--navy);
      box-shadow: 0 10px 25px -15px rgba(255, 201, 60, 0.4);
    }
    .nama-quote i { color: var(--honey); margin-right: 0.5rem; }
    .nama-tags { display: flex; flex-wrap: wrap; gap: 0.5rem; margin-top: 1.2rem; }
    .nama-tags span {
      background: var(--sky-soft); color: var(--blue);
      font-size: 0.8rem; font-weight: 700;
      padding: 0.4rem 0.9rem; border-radius: 50px;
      border: 1px solid rgba(30, 79, 163, 0.1);
    }

    /* SLIDER */
    .funfact {
      padding: 5rem 0; position: relative;
      background: linear-gradient(180deg, transparent 0%, var(--sky-soft) 30%, var(--sun-glow) 100%, transparent 100%);
      overflow: hidden;
    }
    .slider-hint {
      text-align: center; color: var(--honey);
      font-size: 0.9rem; font-weight: 700;
      margin-top: -2rem; margin-bottom: 2rem;
      animation: float 3s ease-in-out infinite;
    }
    .slider-hint i { margin-right: 0.4rem; }
    .slider-wrap {
      position: relative; max-width: 1180px;
      margin: 0 auto; padding: 0 1.5rem;
    }
    .slider-track {
      display: flex; gap: 1.4rem;
      overflow-x: auto; scroll-snap-type: x mandatory;
      padding: 1rem 0.5rem 2rem;
      -webkit-overflow-scrolling: touch;
      scrollbar-width: thin; scrollbar-color: var(--sun) transparent;
    }
    .slider-track::-webkit-scrollbar { height: 8px; }
    .slider-track::-webkit-scrollbar-track {
      background: var(--sky-soft); border-radius: 10px;
    }
    .slider-track::-webkit-scrollbar-thumb {
      background: linear-gradient(90deg, var(--sun), var(--honey));
      border-radius: 10px;
    }
    .slide-card {
      flex: 0 0 300px; scroll-snap-align: start;
      background: #fff; border-radius: var(--radius);
      padding: 2rem 1.6rem;
      box-shadow: 0 20px 40px -25px rgba(30, 79, 163, 0.35);
      border: 1px solid rgba(30, 79, 163, 0.06);
      transition: transform 0.35s ease, box-shadow 0.35s ease;
      position: relative; overflow: hidden;
      cursor: pointer; text-align: center;
    }
    .slide-card:hover {
      transform: translateY(-8px);
      box-shadow: 0 30px 50px -25px rgba(30, 79, 163, 0.5);
    }
    .slide-card::before {
      content: ''; position: absolute; top: -30px; right: -30px;
      width: 120px; height: 120px; border-radius: 50%;
      background: radial-gradient(circle, var(--sun-glow), transparent 70%);
      opacity: 0.6; pointer-events: none;
    }
    .slide-icon {
      width: 72px; height: 72px; border-radius: 20px;
      display: grid; place-items: center; font-size: 1.8rem;
      margin: 0 auto 1.2rem;
      transform: rotate(-5deg);
      transition: transform 0.35s ease;
    }
    .slide-card:hover .slide-icon { transform: rotate(5deg) scale(1.1); }
    .slide-card.hobby .slide-icon {
      background: var(--blue); color: var(--sun);
      box-shadow: 0 12px 24px -10px rgba(30, 79, 163, 0.6);
    }
    .slide-card.sweet .slide-icon {
      background: linear-gradient(135deg, var(--pink), var(--sun-soft));
      color: var(--navy);
      box-shadow: 0 12px 24px -10px rgba(255, 179, 198, 0.7);
    }
    .slide-card.music .slide-icon {
      background: linear-gradient(135deg, var(--blue), var(--sky));
      color: var(--sun);
      box-shadow: 0 12px 24px -10px rgba(30, 79, 163, 0.6);
    }
    .slide-card.movie .slide-icon {
      background: linear-gradient(135deg, var(--sun), var(--honey));
      color: var(--navy);
      box-shadow: 0 12px 24px -10px rgba(255, 201, 60, 0.8);
    }
    .slide-card h3 { font-size: 1.2rem; margin-bottom: 0.6rem; line-height: 1.3; }
    .slide-card p {
      color: var(--muted); font-weight: 500;
      font-size: 0.88rem; line-height: 1.6;
      margin-bottom: 1rem;
    }
    .slide-cta {
      display: inline-flex; align-items: center; gap: 0.4rem;
      background: var(--sky-soft); color: var(--blue);
      font-size: 0.75rem; font-weight: 700;
      padding: 0.4rem 0.9rem; border-radius: 50px;
      letter-spacing: 0.03em;
      transition: all 0.25s;
    }
    .slide-card:hover .slide-cta {
      background: var(--sun-soft); color: var(--navy);
      transform: scale(1.05);
    }

    /* MODAL */
    .modal-overlay {
      position: fixed; inset: 0;
      background: rgba(10, 26, 60, 0.6);
      backdrop-filter: blur(6px);
      z-index: 100;
      display: none;
      align-items: center; justify-content: center;
      padding: 1.5rem; opacity: 0;
      transition: opacity 0.3s ease;
    }
    .modal-overlay.active { display: flex; opacity: 1; }
    .modal-box {
      background: var(--cream);
      border-radius: var(--radius);
      max-width: 520px; width: 100%;
      padding: 2.5rem 2rem;
      position: relative;
      box-shadow: 0 40px 80px -30px rgba(10, 26, 60, 0.6);
      border: 3px dashed var(--sun);
      animation: slideIn 0.4s ease;
      max-height: 85vh; overflow-y: auto;
    }
    .modal-close {
      position: absolute; top: 1rem; right: 1rem;
      width: 38px; height: 38px;
      border-radius: 50%;
      background: var(--sky-soft); color: var(--blue);
      border: none; font-size: 1.2rem;
      cursor: pointer; display: grid; place-items: center;
      transition: all 0.25s; font-weight: 700;
    }
    .modal-close:hover {
      background: var(--sun); color: var(--navy);
      transform: rotate(90deg);
    }
    .modal-icon {
      width: 72px; height: 72px;
      border-radius: 20px;
      display: grid; place-items: center;
      font-size: 2rem; margin: 0 auto 1.2rem;
      transform: rotate(-5deg);
    }
    .modal-box h3 { font-size: 1.6rem; text-align: center; margin-bottom: 0.5rem; }
    .modal-sub {
      text-align: center; color: var(--muted);
      font-size: 0.9rem; font-weight: 500;
      margin-bottom: 1.5rem;
    }
    .modal-list {
      list-style: none;
      display: flex; flex-direction: column; gap: 0.6rem;
    }
    .modal-list li {
      background: #fff; border-radius: var(--radius-sm);
      padding: 0.85rem 1.1rem;
      font-weight: 600; color: var(--navy);
      display: flex; align-items: center; gap: 0.7rem;
      font-size: 0.95rem; transition: all 0.25s;
      border: 1px solid rgba(30, 79, 163, 0.06);
    }
    .modal-list li:hover {
      background: var(--sun-soft);
      transform: translateX(6px);
      border-color: var(--sun);
    }
    .modal-list li i { color: var(--honey); font-size: 0.9rem; }

    /* WARNA */
    .warna { padding: 5rem 0; position: relative; overflow: hidden; }
    .warna-grid {
      display: grid; grid-template-columns: 1fr 1.1fr;
      gap: 3.5rem; align-items: center;
      position: relative; z-index: 3;
    }
    .color-wheel-wrap {
      position: relative; display: flex;
      justify-content: center; align-items: center;
      min-height: 400px;
    }
    .color-wheel {
      width: 320px; height: 320px;
      border-radius: 50%;
      background: conic-gradient(
        #ff6b6b 0deg 40deg, #ffb347 40deg 80deg,
        #ffd93d 80deg 120deg, #b8e6d9 120deg 160deg,
        #4ecdc4 160deg 200deg, #4a7fd4 200deg 240deg,
        #1e4fa3 240deg 280deg, #a78bfa 280deg 320deg,
        #ffb3c6 320deg 360deg
      );
      box-shadow:
        0 30px 60px -25px rgba(30, 79, 163, 0.4),
        inset 0 0 0 8px #fff,
        inset 0 0 0 12px var(--sun-soft);
      position: relative;
      animation: spin 60s linear infinite;
    }
    .color-wheel::before {
      content: '';
      position: absolute; inset: 40px;
      border-radius: 50%;
      background: radial-gradient(circle, #fff 0%, var(--cream) 70%);
      box-shadow: inset 0 0 20px rgba(30, 79, 163, 0.1);
    }
    .color-wheel-center {
      position: absolute;
      width: 130px; height: 130px;
      border-radius: 50%;
      background: #fff;
      display: grid; place-items: center;
      text-align: center;
      box-shadow: 0 15px 30px -15px rgba(30, 79, 163, 0.4);
      font-family: 'Fraunces', serif;
      font-size: 1.1rem; font-weight: 700;
      color: var(--blue); line-height: 1.2;
      padding: 0.5rem;
    }
    .color-wheel-center small {
      display: block; font-size: 0.65rem;
      color: var(--honey); letter-spacing: 0.1em;
      text-transform: uppercase;
      margin-top: 0.3rem;
      font-family: 'Quicksand', sans-serif;
    }
    .color-dot-float {
      position: absolute;
      width: 44px; height: 44px;
      border-radius: 50%;
      box-shadow: 0 10px 20px -8px rgba(30, 79, 163, 0.4);
      border: 3px solid #fff;
      animation: float 5s ease-in-out infinite;
    }
    .cd-1 { top: 8%; left: 8%; background: #ff6b6b; animation-delay: 0s; }
    .cd-2 { top: 15%; right: 6%; background: #ffd93d; animation-delay: 0.5s; }
    .cd-3 { bottom: 15%; left: 4%; background: #4a7fd4; animation-delay: 1s; }
    .cd-4 { bottom: 8%; right: 10%; background: #a78bfa; animation-delay: 1.5s; }
    .warna-content h2 { font-size: clamp(1.8rem, 3.5vw, 2.5rem); margin-bottom: 1.2rem; }
    .warna-content p {
      color: var(--muted); font-weight: 500;
      font-size: 1rem; margin-bottom: 1.5rem; line-height: 1.7;
    }
    .warna-content strong { color: var(--blue); font-weight: 700; }
    .warna-palette {
      display: grid; grid-template-columns: repeat(4, 1fr);
      gap: 0.8rem; margin: 1.5rem 0;
    }
    .warna-swatch {
      aspect-ratio: 1;
      border-radius: var(--radius-sm);
      box-shadow: 0 10px 20px -10px rgba(30, 79, 163, 0.3);
      display: flex; flex-direction: column;
      justify-content: flex-end;
      padding: 0.6rem;
      color: #fff; font-size: 0.7rem; font-weight: 700;
      text-shadow: 0 1px 3px rgba(0,0,0,0.3);
      cursor: pointer;
      transition: transform 0.3s ease;
      border: 3px solid #fff;
    }
    .warna-swatch:hover { transform: translateY(-6px) scale(1.05); }
    .warna-tags { display: flex; flex-wrap: wrap; gap: 0.5rem; margin-top: 1rem; }
    .warna-tags span {
      background: var(--sky-soft); color: var(--blue);
      font-size: 0.8rem; font-weight: 700;
      padding: 0.4rem 0.9rem; border-radius: 50px;
      border: 1px solid rgba(30, 79, 163, 0.1);
    }

    /* FUNFACT AYU */
    .funfact-ayu {
      padding: 5rem 0; position: relative;
      background: linear-gradient(180deg, transparent 0%, var(--sun-glow) 50%, transparent 100%);
    }
    .funfact-ayu-grid {
      display: grid; grid-template-columns: repeat(2, 1fr);
      gap: 2rem; position: relative; z-index: 3;
      max-width: 900px; margin: 0 auto;
    }
    .funfact-ayu .fun-card {
      padding: 2.5rem 2rem;
      background: #fff; border-radius: var(--radius);
      box-shadow: 0 20px 40px -25px rgba(30, 79, 163, 0.35);
      border: 1px solid rgba(30, 79, 163, 0.06);
      position: relative; overflow: hidden;
      transition: transform 0.35s ease;
    }
    .funfact-ayu .fun-card:hover { transform: translateY(-6px); }
    .funfact-ayu .fun-card .fun-icon {
      width: 68px; height: 68px;
      font-size: 1.7rem; border-radius: 20px;
      display: grid; place-items: center;
      margin-bottom: 1.2rem;
      transform: rotate(-5deg);
    }
    .funfact-ayu .fun-card h3 { font-size: 1.3rem; margin-bottom: 0.8rem; }
    .funfact-ayu .fun-card p {
      font-size: 0.95rem; line-height: 1.7;
      color: var(--muted); font-weight: 500;
    }
    .funfact-ayu .fun-card .fun-tag {
      display: inline-block; margin-top: 1rem;
      background: var(--sky-soft); color: var(--blue);
      font-size: 0.7rem; font-weight: 700;
      padding: 0.3rem 0.7rem; border-radius: 50px;
    }
    .fun-card.cat .fun-icon {
      background: linear-gradient(135deg, var(--sun), var(--pink));
      color: var(--navy);
      box-shadow: 0 12px 24px -10px rgba(255, 201, 60, 0.8);
    }
    .fun-card.cat .fun-tag { background: var(--pink); color: var(--navy); }
    .fun-card.direction .fun-icon {
      background: linear-gradient(135deg, var(--blue), var(--sky));
      color: var(--sun);
      box-shadow: 0 12px 24px -10px rgba(30, 79, 163, 0.6);
    }
    .fun-card.direction .fun-tag { background: var(--sky-soft); color: var(--blue); }

    /* MBTI */
    .mbti-section {
      padding: 5rem 0;
      background: linear-gradient(180deg, transparent 0%, var(--sky-soft) 50%, transparent 100%);
      position: relative;
    }
    .mbti-grid {
      display: grid; grid-template-columns: 1.1fr 1fr 1fr;
      gap: 2rem; align-items: start;
      position: relative; z-index: 3;
    }
    .mbti-card {
      background: #fff; border-radius: var(--radius);
      padding: 2rem 1.8rem;
      box-shadow: 0 20px 40px -25px rgba(30, 79, 163, 0.35);
      border: 1px solid rgba(30, 79, 163, 0.06);
      transition: transform 0.35s ease;
    }
    .mbti-card:hover { transform: translateY(-6px); }
    .mbti-card.intro { background: linear-gradient(150deg, #fff 0%, var(--sky-soft) 100%); }
    .mbti-icon { font-size: 2.5rem; margin-bottom: 1rem; }
    .mbti-card h3 { font-size: 1.3rem; margin-bottom: 0.6rem; }
    .mbti-card p {
      color: var(--muted); font-weight: 500;
      font-size: 0.95rem; line-height: 1.65; margin-bottom: 1rem;
    }
    .character-img {
      width: 100%; height: 180px;
      border-radius: var(--radius-sm);
      overflow: hidden; margin-bottom: 1.2rem;
      border: 3px solid #fff;
      outline: 2px dashed var(--sun); outline-offset: 3px;
      background: linear-gradient(135deg, #4a7fd4, #ffe9a8);
      display: grid; place-items: center;
      font-size: 4rem; color: #fff;
    }
    .character-from {
      display: block; font-size: 0.75rem;
      color: var(--honey); font-weight: 700;
      letter-spacing: 0.05em;
      text-transform: uppercase;
      margin-bottom: 0.8rem;
    }
    .mbti-traits { display: flex; flex-wrap: wrap; gap: 0.5rem; }
    .mbti-traits span {
      background: var(--sun-soft); color: var(--navy);
      font-size: 0.72rem; font-weight: 700;
      padding: 0.3rem 0.75rem; border-radius: 50px;
    }
    .mbti-card.character .mbti-traits span { background: var(--sky-soft); color: var(--blue); }

    /* HOBI */
    .hobi { padding: 5rem 0; position: relative; }
    .hobi-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 2rem;
    }
    .hobi-card {
      position: relative; border-radius: var(--radius);
      padding: 2.5rem 2rem; overflow: hidden;
      transition: transform 0.35s ease, box-shadow 0.35s ease;
      border: 1px solid rgba(30, 79, 163, 0.08);
    }
    .hobi-card:hover { transform: translateY(-8px); box-shadow: var(--shadow-soft); }
    .hobi-card.drawing { background: linear-gradient(150deg, #fff 0%, var(--sky-soft) 100%); }
    .hobi-card.sleeping { background: linear-gradient(150deg, #fff 0%, var(--sun-glow) 100%); }
    .hobi-icon {
      width: 68px; height: 68px; border-radius: 20px;
      display: grid; place-items: center; font-size: 1.7rem;
      margin-bottom: 1.5rem; transform: rotate(-5deg);
      transition: transform 0.35s ease;
    }
    .hobi-card:hover .hobi-icon { transform: rotate(5deg) scale(1.08); }
    .hobi-card.drawing .hobi-icon {
      background: var(--blue); color: var(--sun);
      box-shadow: 0 12px 24px -10px rgba(30, 79, 163, 0.6);
    }
    .hobi-card.sleeping .hobi-icon {
      background: var(--sun); color: var(--navy);
      box-shadow: 0 12px 24px -10px rgba(255, 201, 60, 0.8);
    }
    .hobi-card h3 { font-size: 1.5rem; margin-bottom: 0.75rem; }
    .hobi-card p { color: var(--muted); font-weight: 500; font-size: 1rem; margin-bottom: 1.2rem; }
    .hobi-tags { display: flex; flex-wrap: wrap; gap: 0.5rem; }
    .hobi-tags span {
      background: rgba(255, 255, 255, 0.8);
      border: 1px solid rgba(30, 79, 163, 0.12);
      padding: 0.35rem 0.85rem; border-radius: 50px;
      font-size: 0.8rem; font-weight: 700; color: var(--blue);
    }
    .hobi-card.drawing .hobi-tags span i { color: var(--honey); }
    .hobi-card.sleeping .hobi-tags span i { color: var(--blue); }

    /* MAKANAN */
    .makanan {
      padding: 5rem 0;
      background: linear-gradient(180deg, transparent 0%, var(--sky-soft) 50%, transparent 100%);
      position: relative;
    }
    .food-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 2rem; margin-top: 1rem;
      position: relative; z-index: 3;
    }
    .food-card {
      background: #fff; border-radius: var(--radius);
      padding: 2.5rem 2rem; position: relative; overflow: hidden;
      box-shadow: 0 20px 40px -25px rgba(30, 79, 163, 0.3);
      border: 1px solid rgba(30, 79, 163, 0.06);
      transition: transform 0.35s ease;
    }
    .food-card:hover { transform: translateY(-6px) rotate(-0.5deg); }
    .food-emoji { font-size: 3.5rem; margin-bottom: 1rem; display: inline-block; transition: transform 0.4s ease; }
    .food-card:hover .food-emoji { transform: scale(1.15) rotate(8deg); }
    .food-card h3 { font-size: 1.6rem; margin-bottom: 0.5rem; }
    .food-card p { color: var(--muted); font-weight: 500; margin-bottom: 1.3rem; }
    .rating {
      display: flex; align-items: center; gap: 0.3rem;
      color: var(--sun); font-size: 1rem; margin-bottom: 1.2rem;
    }
    .rating span { color: var(--muted); font-weight: 700; font-size: 0.85rem; margin-left: 0.4rem; }
    .food-note {
      display: inline-block; background: var(--sun-soft);
      color: var(--navy); font-size: 0.8rem; font-weight: 700;
      padding: 0.4rem 0.9rem; border-radius: 50px;
    }
    .food-card.mie-ayam::before {
      content: '🍜'; position: absolute; font-size: 12rem;
      opacity: 0.05; right: -30px; top: -30px; transform: rotate(15deg);
    }
    .food-card.kapurung::before {
      content: '🥣'; position: absolute; font-size: 12rem;
      opacity: 0.05; right: -30px; top: -30px; transform: rotate(-10deg);
    }

    /* MOOD */
    .mood { padding: 5rem 0; }
    .mood-grid {
      display: grid; grid-template-columns: repeat(4, 1fr);
      gap: 1.2rem; position: relative; z-index: 3;
    }
    .mood-item {
      aspect-ratio: 1; border-radius: var(--radius-sm);
      display: grid; place-items: center; font-size: 2.8rem;
      transition: transform 0.35s ease, box-shadow 0.35s ease;
      cursor: pointer; position: relative; overflow: hidden;
      border: 1px solid rgba(30, 79, 163, 0.06);
    }
    .mood-item:hover {
      transform: scale(1.05) rotate(2deg);
      box-shadow: 0 20px 35px -15px rgba(30, 79, 163, 0.4);
      z-index: 2;
    }
    .mood-item span {
      position: absolute; bottom: 10px;
      font-size: 0.7rem; font-weight: 700;
      color: rgba(10, 26, 60, 0.55);
      letter-spacing: 0.05em; text-transform: uppercase;
    }

    /* COMMENT SECTION */
    .comment-section {
      padding: 5rem 0;
      position: relative;
      background: linear-gradient(180deg, transparent 0%, var(--sky-soft) 50%, transparent 100%);
      overflow: hidden;
    }
    .comment-intro {
      text-align: center; max-width: 640px;
      margin: 0 auto 3rem;
    }
    .comment-intro .kicker {
      display: inline-block; font-size: 0.85rem;
      font-weight: 700; letter-spacing: 0.15em;
      text-transform: uppercase; color: var(--honey);
      margin-bottom: 0.8rem;
    }
    .comment-intro .kicker::before,
    .comment-intro .kicker::after {
      content: '✦'; margin: 0 0.6rem;
      color: var(--sun); font-size: 0.7rem;
    }
    .comment-intro h2 { font-size: clamp(2rem, 4vw, 2.8rem); margin-bottom: 1rem; }
    .comment-intro p { color: var(--muted); font-size: 1.05rem; font-weight: 500; }
    .comment-grid {
      display: grid; grid-template-columns: 1fr 1.2fr;
      gap: 2.5rem; position: relative; z-index: 3;
      max-width: 1100px; margin: 0 auto;
    }
    .comment-form-wrap {
      background: #fff; border-radius: var(--radius);
      padding: 2rem;
      box-shadow: 0 20px 40px -25px rgba(30, 79, 163, 0.35);
      border: 2px dashed var(--sun);
      height: fit-content;
    }
    .comment-form-wrap h3 {
      font-size: 1.3rem; margin-bottom: 1.2rem;
      display: flex; align-items: center; gap: 0.6rem;
    }
    .comment-form-wrap h3 i { color: var(--honey); }
    .form-group { margin-bottom: 1rem; }
    .form-group label {
      display: block; font-size: 0.85rem;
      font-weight: 700; color: var(--navy);
      margin-bottom: 0.4rem;
    }
    .form-group input,
    .form-group textarea,
    .form-group select {
      width: 100%; padding: 0.75rem 1rem;
      border-radius: 12px;
      border: 2px solid var(--sky);
      background: var(--sky-soft);
      font-family: 'Quicksand', sans-serif;
      font-size: 0.95rem; font-weight: 500;
      color: var(--navy);
      transition: all 0.25s ease;
      outline: none;
    }
    .form-group input:focus,
    .form-group textarea:focus,
    .form-group select:focus {
      border-color: var(--sun);
      background: #fff;
      box-shadow: 0 8px 20px -12px rgba(255, 201, 60, 0.6);
    }
    .form-group textarea {
      resize: vertical; min-height: 100px;
      font-family: 'Quicksand', sans-serif;
    }
    .btn-send {
      width: 100%; margin-top: 0.5rem;
      padding: 0.9rem 1.6rem;
      border-radius: 50px;
      background: linear-gradient(135deg, var(--blue), var(--blue-soft));
      color: #fff; border: none; cursor: pointer;
      font-family: 'Quicksand', sans-serif;
      font-weight: 700; font-size: 1rem;
      transition: all 0.28s ease;
      display: flex; align-items: center; justify-content: center;
      gap: 0.6rem;
      box-shadow: 0 12px 24px -10px rgba(30, 79, 163, 0.6);
    }
    .btn-send:hover {
      transform: translateY(-3px) scale(1.01);
      box-shadow: 0 18px 30px -10px rgba(30, 79, 163, 0.7);
    }
    .comment-list-wrap {
      display: flex; flex-direction: column; gap: 1rem;
    }
    .comment-list-header {
      display: flex; align-items: center;
      justify-content: space-between; margin-bottom: 0.5rem;
    }
    .comment-list-header h3 {
      font-size: 1.3rem;
      display: flex; align-items: center; gap: 0.6rem;
    }
    .comment-list-header h3 i { color: var(--honey); }
    .comment-count {
      background: var(--sun-soft); color: var(--navy);
      font-size: 0.8rem; font-weight: 700;
      padding: 0.35rem 0.8rem; border-radius: 50px;
    }
    .comment-list {
      display: flex; flex-direction: column;
      gap: 1rem; max-height: 520px;
      overflow-y: auto; padding-right: 0.3rem;
    }
    .comment-list::-webkit-scrollbar { width: 6px; }
    .comment-list::-webkit-scrollbar-track {
      background: var(--sky-soft); border-radius: 10px;
    }
    .comment-list::-webkit-scrollbar-thumb {
      background: var(--sun); border-radius: 10px;
    }
    .comment-item {
      background: #fff; border-radius: var(--radius-sm);
      padding: 1.2rem 1.3rem;
      box-shadow: 0 15px 30px -20px rgba(30, 79, 163, 0.3);
      border: 1px solid rgba(30, 79, 163, 0.06);
      transition: transform 0.25s ease;
      animation: slideIn 0.4s ease;
    }
    .comment-item:hover {
      transform: translateY(-3px);
      box-shadow: 0 20px 35px -20px rgba(30, 79, 163, 0.4);
    }
    .comment-head {
      display: flex; align-items: center;
      gap: 0.7rem; margin-bottom: 0.6rem;
    }
    .comment-avatar {
      width: 42px; height: 42px;
      border-radius: 50%;
      display: grid; place-items: center;
      font-family: 'Fraunces', serif;
      font-weight: 700; font-size: 1rem;
      color: #fff; flex-shrink: 0;
      box-shadow: 0 6px 12px -6px rgba(30, 79, 163, 0.4);
    }
    .comment-meta { flex-grow: 1; min-width: 0; }
    .comment-name {
      font-weight: 700; font-size: 0.95rem;
      color: var(--navy);
      white-space: nowrap; overflow: hidden; text-overflow: ellipsis;
    }
    .comment-time { font-size: 0.72rem; color: var(--muted); font-weight: 500; }
    .comment-badge {
      font-size: 0.7rem; font-weight: 700;
      padding: 0.25rem 0.7rem;
      border-radius: 50px; flex-shrink: 0;
    }
    .comment-badge.critik { background: #ffe0e0; color: #c92a2a; }
    .comment-badge.saran { background: var(--sky-soft); color: var(--blue); }
    .comment-badge.pujian { background: #d4f4dd; color: #2b8a3e; }
    .comment-body {
      color: var(--muted); font-weight: 500;
      font-size: 0.92rem; line-height: 1.6;
      word-wrap: break-word;
    }
    .comment-empty {
      text-align: center; padding: 2rem 1rem;
      background: #fff; border-radius: var(--radius-sm);
      border: 2px dashed var(--sky);
      color: var(--muted); font-weight: 500;
    }
    .comment-empty i {
      font-size: 2rem; color: var(--sun);
      display: block; margin-bottom: 0.6rem;
    }

    /* QUOTE */
    .quote-section { padding: 5rem 0 6rem; }
    .quote-card {
      background: linear-gradient(135deg, var(--navy) 0%, var(--blue) 100%);
      border-radius: var(--radius); padding: 4rem 3rem;
      text-align: center; position: relative; overflow: hidden;
      color: #fff; box-shadow: 0 30px 60px -30px rgba(10, 26, 60, 0.6);
    }
    .quote-card::before {
      content: ''; position: absolute;
      top: -60px; right: -60px;
      width: 260px; height: 260px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(255, 233, 168, 0.35), transparent 70%);
    }
    .quote-card::after {
      content: ''; position: absolute;
      bottom: -80px; left: -60px;
      width: 240px; height: 240px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(74, 127, 212, 0.5), transparent 70%);
    }
    .quote-card .qmark {
      font-family: 'Fraunces', serif;
      font-size: 5rem; line-height: 0.6;
      color: var(--sun); display: block;
      margin-bottom: 0.5rem;
      position: relative; z-index: 2;
    }
    .quote-card blockquote {
      font-family: 'Fraunces', serif;
      font-size: clamp(1.4rem, 3vw, 2.1rem);
      font-weight: 600; font-style: italic;
      line-height: 1.35; max-width: 780px;
      margin: 0 auto 1.5rem;
      position: relative; z-index: 2;
    }
    .quote-card .author {
      font-weight: 700; color: var(--sun-soft);
      letter-spacing: 0.1em; text-transform: uppercase;
      font-size: 0.85rem;
      position: relative; z-index: 2;
    }
    .quote-card .btn-sun { margin-top: 2rem; position: relative; z-index: 2; }

    /* FOOTER */
    footer {
      padding: 3rem 0 2.5rem; text-align: center;
      border-top: 1px solid rgba(30, 79, 163, 0.1);
    }
    .footer-heart {
      font-size: 1.1rem; color: var(--honey);
      margin: 0 0.3rem;
      animation: beat 1.6s ease-in-out infinite;
      display: inline-block;
    }
    .footer-text { color: var(--muted); font-weight: 600; font-size: 0.9rem; margin-top: 1rem; }

    .socials {
      display: flex;
      justify-content: center;
      align-items: stretch;
      gap: 1rem;
      margin-top: 1.5rem;
      flex-wrap: wrap;
    }
    .sosial-bubble {
      display: flex;
      align-items: center;
      gap: 0.9rem;
      padding: 0.9rem 1.4rem 0.9rem 0.9rem;
      border-radius: 50px;
      background: #fff;
      text-decoration: none;
      border: 2px solid rgba(30, 79, 163, 0.1);
      box-shadow: 0 10px 25px -15px rgba(30, 79, 163, 0.4);
      transition: all 0.3s ease;
      position: relative;
      overflow: hidden;
      min-width: 200px;
    }
    .sosial-bubble:hover {
      transform: translateY(-5px);
      box-shadow: 0 20px 35px -15px rgba(30, 79, 163, 0.5);
      border-color: transparent;
    }
    .bubble-icon {
      width: 46px; height: 46px;
      border-radius: 50%;
      display: grid; place-items: center;
      color: #fff; font-size: 1.3rem;
      flex-shrink: 0;
      transition: transform 0.3s ease, background 0.3s ease;
      position: relative; z-index: 1;
    }
    .sosial-bubble:hover .bubble-icon { transform: scale(1.1) rotate(8deg); }
    .bubble-text {
      display: flex; flex-direction: column;
      text-align: left; line-height: 1.25;
      position: relative; z-index: 1;
    }
    .bubble-title {
      font-family: 'Fraunces', serif;
      font-weight: 700; font-size: 1rem;
      color: var(--navy);
      transition: color 0.3s ease;
    }
    .bubble-sub {
      font-family: 'Quicksand', sans-serif;
      font-weight: 600; font-size: 0.8rem;
      color: var(--muted);
      transition: color 0.3s ease;
    }
    .bubble-ig .bubble-icon {
      background: linear-gradient(45deg, #f09433 0%, #e6683c 25%, #dc2743 50%, #cc2366 75%, #bc1888 100%);
    }
    .bubble-ig:hover {
      background: linear-gradient(45deg, #f09433 0%, #e6683c 25%, #dc2743 50%, #cc2366 75%, #bc1888 100%);
    }
    .bubble-ig:hover .bubble-title,
    .bubble-ig:hover .bubble-sub { color: #fff; }
    .bubble-ig:hover .bubble-icon { background: rgba(255, 255, 255, 0.25); }
    .bubble-roblox .bubble-icon {
      background: linear-gradient(135deg, #e2231a, #b5190f);
    }
    .bubble-roblox:hover {
      background: linear-gradient(135deg, #e2231a, #b5190f);
    }
    .bubble-roblox:hover .bubble-title,
    .bubble-roblox:hover .bubble-sub { color: #fff; }
    .bubble-roblox:hover .bubble-icon { background: rgba(255, 255, 255, 0.25); }
    .bubble-wa .bubble-icon {
      background: linear-gradient(135deg, #25d366, #128c7e);
    }
    .bubble-wa:hover {
      background: linear-gradient(135deg, #25d366, #128c7e);
    }
    .bubble-wa:hover .bubble-title,
    .bubble-wa:hover .bubble-sub { color: #fff; }
    .bubble-wa:hover .bubble-icon { background: rgba(255, 255, 255, 0.25); }

    /* MUSIC PLAYER */
    .music-player {
      position: fixed; bottom: 1.5rem; left: 1.5rem;
      z-index: 90;
      background: rgba(255, 253, 247, 0.95);
      backdrop-filter: blur(14px);
      border-radius: 50px;
      padding: 0.5rem 0.8rem 0.5rem 0.5rem;
      display: flex; align-items: center; gap: 0.7rem;
      box-shadow: 0 20px 40px -15px rgba(30, 79, 163, 0.5);
      border: 2px dashed var(--sun);
      transition: all 0.3s ease;
      max-width: calc(100% - 3rem);
    }
    .music-player:hover {
      transform: translateY(-3px);
      box-shadow: 0 25px 50px -15px rgba(30, 79, 163, 0.6);
    }
    .music-btn {
      width: 44px; height: 44px;
      border-radius: 50%;
      background: linear-gradient(135deg, var(--blue), var(--blue-soft));
      color: var(--sun); border: none; cursor: pointer;
      display: grid; place-items: center;
      font-size: 1.1rem; transition: all 0.3s ease;
      flex-shrink: 0;
      box-shadow: 0 8px 16px -6px rgba(30, 79, 163, 0.5);
    }
    .music-btn:hover { transform: scale(1.08) rotate(8deg); }
    .music-btn.playing { animation: spin 6s linear infinite; }
    .music-info {
      display: flex; flex-direction: column;
      gap: 0.1rem; overflow: hidden;
      max-width: 160px;
    }
    .music-title {
      font-family: 'Fraunces', serif;
      font-weight: 700; font-size: 0.8rem;
      color: var(--navy);
      white-space: nowrap; overflow: hidden; text-overflow: ellipsis;
      line-height: 1.2;
    }
    .music-artist {
      font-size: 0.7rem; color: var(--muted);
      font-weight: 600;
      white-space: nowrap; overflow: hidden; text-overflow: ellipsis;
    }
    .music-eq {
      display: flex; align-items: flex-end;
      gap: 2px; height: 20px;
      padding-right: 0.4rem;
    }
    .music-eq span {
      width: 3px; background: var(--sun);
      border-radius: 3px; height: 6px;
    }
    .music-player.playing .music-eq span:nth-child(1) { animation: eq 0.6s ease-in-out infinite; }
    .music-player.playing .music-eq span:nth-child(2) { animation: eq 0.8s ease-in-out infinite 0.1s; }
    .music-player.playing .music-eq span:nth-child(3) { animation: eq 0.5s ease-in-out infinite 0.2s; }
    .music-player.playing .music-eq span:nth-child(4) { animation: eq 0.7s ease-in-out infinite 0.3s; }

    /* RESPONSIVE */
    @media (max-width: 1024px) {
      .content-grid { grid-template-columns: repeat(4, 1fr); }
      .mbti-grid { grid-template-columns: 1fr; }
      .nama-grid { grid-template-columns: 1fr; gap: 3rem; }
      .nama-visual { min-height: 400px; }
      .warna-grid { grid-template-columns: 1fr; gap: 3rem; }
      .color-wheel { width: 280px; height: 280px; }
      .comment-grid { grid-template-columns: 1fr; }
    }
    @media (max-width: 992px) {
      .hero-grid { grid-template-columns: 1fr; gap: 4rem; }
      .hero p.lead { max-width: 100%; }
      .hero-visual { order: -1; }
      .mood-grid { grid-template-columns: repeat(3, 1fr); }
      .about-grid { grid-template-columns: 1fr; gap: 2.5rem; }
      .about-visual { min-height: 380px; }
      .nav-links { gap: 1rem; }
      .content-grid { grid-template-columns: repeat(3, 1fr); }
    }
    @media (max-width: 768px) {
      .nav-links { display: none; }
      .content-grid { grid-template-columns: repeat(3, 1fr); gap: 0.8rem; }
      .content-card { padding: 1.1rem 0.8rem; }
      .content-num { width: 36px; height: 36px; font-size: 0.85rem; }
      .content-title { font-size: 0.8rem; }
      .hobi-grid, .food-grid { grid-template-columns: repeat(2, 1fr); gap: 0.8rem; }
      .hobi-card, .food-card { padding: 1.5rem 1rem; }
      .hobi-card h3, .food-card h3 { font-size: 1.1rem; }
      .hobi-card p, .food-card p { font-size: 0.82rem; }
      .mood-grid { grid-template-columns: repeat(2, 1fr); }
      .quote-card { padding: 3rem 1.5rem; }
      .fc-1, .fc-2, .fc-3 { display: none; }
      .profile-card { transform: rotate(0); }
      .funfact-ayu-grid { grid-template-columns: 1fr; }
      .nama-circle { width: 280px; height: 280px; }
      .nama-word .nama-besar { font-size: 2.4rem; }
      .slide-card { flex: 0 0 260px; }
      .warna-palette { grid-template-columns: repeat(3, 1fr); }
      .color-wheel { width: 240px; height: 240px; }
      .color-wheel-center { width: 100px; height: 100px; font-size: 0.9rem; }
      .polkadot-banner { height: 70px; }
      .polkadot-banner-text { font-size: 0.9rem; letter-spacing: 0.15em; padding: 0.4rem 1rem; }
      .star-deco.s-1 { width: 60px; height: 60px; }
      .star-deco.s-2 { width: 55px; height: 55px; }
      .star-deco.s-3 { width: 58px; height: 58px; }
      .star-deco.s-4 { width: 65px; height: 65px; }
      .star-deco.s-5 { width: 50px; height: 50px; }
      .star-deco.s-6 { width: 48px; height: 48px; }
    }
    @media (max-width: 600px) {
      .socials { flex-direction: column; align-items: stretch; }
      .sosial-bubble { min-width: auto; width: 100%; }
      .biodata { grid-template-columns: 1fr; }
    }
    @media (max-width: 480px) {
      .hero h1 { font-size: 2.2rem; }
      .content-grid { grid-template-columns: repeat(2, 1fr); }
      .mood-grid { grid-template-columns: repeat(2, 1fr); }
      .section-head .kicker::before,
      .section-head .kicker::after { display: none; }
      .nama-circle { width: 240px; height: 240px; }
      .nama-word .nama-besar { font-size: 2rem; }
      .nama-word .nama-kecil { font-size: 0.85rem; }
      .nama-tag-float { font-size: 0.7rem; padding: 0.5rem 0.8rem; }
      .slide-card { flex: 0 0 240px; padding: 1.6rem 1.2rem; }
      .modal-box { padding: 2rem 1.2rem; }
      .music-player {
        bottom: 1rem; left: 1rem; right: 1rem;
        max-width: none;
      }
      .music-info { max-width: 120px; }
      .hobi-grid, .food-grid { grid-template-columns: repeat(2, 1fr); gap: 0.6rem; }
      .hobi-card, .food-card { padding: 1.2rem 0.8rem; }
      .hobi-card h3, .food-card h3 { font-size: 1rem; }
      .hobi-card p, .food-card p { font-size: 0.75rem; line-height: 1.5; }
      .hobi-icon { width: 50px !important; height: 50px !important; font-size: 1.3rem !important; margin-bottom: 0.8rem !important; }
      .food-emoji { font-size: 2.2rem !important; margin-bottom: 0.6rem !important; }
      .rating { font-size: 0.75rem; gap: 0.15rem; }
      .rating i { font-size: 0.65rem; }
      .rating span { font-size: 0.7rem; }
      .hobi-tags span { font-size: 0.62rem; padding: 0.25rem 0.55rem; }
      .food-note { font-size: 0.62rem; padding: 0.3rem 0.7rem; }
      .polkadot-banner { height: 55px; }
      .polkadot-banner-text {
        font-size: 0.75rem;
        letter-spacing: 0.1em;
        padding: 0.3rem 0.8rem;
        gap: 0.4rem;
      }
    }
  </style>
</head>
<body>

  <!-- ============ HIASAN BINTANG POLKADOT HALFTONE (LAYER BELAKANG) ============ -->

  <div class="star-deco s-1">
    <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <pattern id="dotStar1" x="0" y="0" width="4" height="4" patternUnits="userSpaceOnUse">
          <circle cx="2" cy="2" r="1.4" fill="#4a7fd4"/>
        </pattern>
      </defs>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="url(#dotStar1)"/>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="none" stroke="#4a7fd4" stroke-width="0.8" opacity="0.4"/>
    </svg>
  </div>

  <div class="star-deco s-2">
    <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <pattern id="dotStar2" x="0" y="0" width="3.5" height="3.5" patternUnits="userSpaceOnUse">
          <circle cx="1.75" cy="1.75" r="1.2" fill="#4a7fd4"/>
        </pattern>
      </defs>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="url(#dotStar2)"/>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="none" stroke="#4a7fd4" stroke-width="0.8" opacity="0.4"/>
    </svg>
  </div>

  <div class="star-deco s-3">
    <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <pattern id="dotStar3" x="0" y="0" width="4" height="4" patternUnits="userSpaceOnUse">
          <circle cx="2" cy="2" r="1.4" fill="#5b8fdc"/>
        </pattern>
      </defs>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="url(#dotStar3)"/>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="none" stroke="#5b8fdc" stroke-width="0.8" opacity="0.4"/>
    </svg>
  </div>

  <div class="star-deco s-4">
    <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <pattern id="dotStar4" x="0" y="0" width="4.5" height="4.5" patternUnits="userSpaceOnUse">
          <circle cx="2.25" cy="2.25" r="1.6" fill="#4a7fd4"/>
        </pattern>
      </defs>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="url(#dotStar4)"/>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="none" stroke="#4a7fd4" stroke-width="0.8" opacity="0.4"/>
    </svg>
  </div>

  <div class="star-deco s-5">
    <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <pattern id="dotStar5" x="0" y="0" width="3.5" height="3.5" patternUnits="userSpaceOnUse">
          <circle cx="1.75" cy="1.75" r="1.2" fill="#4a7fd4"/>
        </pattern>
      </defs>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="url(#dotStar5)"/>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="none" stroke="#4a7fd4" stroke-width="0.8" opacity="0.4"/>
    </svg>
  </div>

  <div class="star-deco s-6">
    <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <pattern id="dotStar6" x="0" y="0" width="4" height="4" patternUnits="userSpaceOnUse">
          <circle cx="2" cy="2" r="1.4" fill="#5b8fdc"/>
        </pattern>
      </defs>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="url(#dotStar6)"/>
      <polygon points="50,8 62,38 95,40 69,62 78,94 50,75 22,94 31,62 5,40 38,38" fill="none" stroke="#5b8fdc" stroke-width="0.8" opacity="0.4"/>
    </svg>
  </div>

  <!-- ============ INTRO ANIMASI NAMA AYU ============ -->
  <div class="intro-overlay" id="introOverlay">
    <span class="intro-sparkle s1"></span>
    <span class="intro-sparkle s2"></span>
    <span class="intro-sparkle s3"></span>
    <span class="intro-sparkle s4"></span>
    <span class="intro-sparkle s5"></span>
    <span class="intro-sparkle s6"></span>
    <span class="intro-sparkle s7"></span>
    <span class="intro-sparkle s8"></span>
    <span class="intro-sparkle s9"></span>
    <span class="intro-sparkle s10"></span>

    <span class="intro-star st1">✦</span>
    <span class="intro-star st2">✦</span>
    <span class="intro-star st3">✦</span>
    <span class="intro-star st4">✦</span>

    <div class="intro-content" id="introContent">
      <span class="intro-letter letter-a">A</span>
      <span class="intro-letter letter-y">y</span>
      <span class="intro-letter letter-u">u</span>
    </div>

    <button class="intro-skip" onclick="skipIntro()">
      <i class="fas fa-forward"></i> Lewati
    </button>
  </div>

  <!-- ============ SPRINKLE JATUH ============ -->
  <div class="sprinkle-layer" aria-hidden="true">
    <div class="sprinkle round"  style="left: 8%;  background: #ffc93c; animation-duration: 22s; animation-delay: 0s;"></div>
    <div class="sprinkle long"   style="left: 28%; background: #a8c8ff; animation-duration: 26s; animation-delay: 6s;"></div>
    <div class="sprinkle square" style="left: 48%; background: #ffe9a8; animation-duration: 24s; animation-delay: 12s;"></div>
    <div class="sprinkle round"  style="left: 68%; background: #b8e6d9; animation-duration: 27s; animation-delay: 3s;"></div>
    <div class="sprinkle long"   style="left: 85%; background: #ffd93d; animation-duration: 23s; animation-delay: 15s;"></div>
    <div class="sprinkle round"  style="left: 95%; background: #c5d9ff; animation-duration: 25s; animation-delay: 9s;"></div>
  </div>

  <!-- ============ HIASAN KRIM FLOATING ============ -->

  <div class="cream-float" style="top: 12%; left: 3%; animation-delay: 0s;">
    <svg width="55" height="55" viewBox="0 0 100 100">
      <ellipse cx="50" cy="75" rx="30" ry="6" fill="#e8a921" opacity="0.4"/>
      <path d="M20 60 L30 85 L70 85 L80 60 Z" fill="#ffe9a8" stroke="#e8a921" stroke-width="2"/>
      <ellipse cx="50" cy="55" rx="30" ry="14" fill="#fff" stroke="#4a7fd4" stroke-width="2"/>
      <ellipse cx="50" cy="46" rx="22" ry="10" fill="#fff" stroke="#4a7fd4" stroke-width="2"/>
      <ellipse cx="50" cy="38" rx="14" ry="7" fill="#fff" stroke="#4a7fd4" stroke-width="2"/>
      <circle cx="50" cy="32" r="3" fill="#ffc93c"/>
    </svg>
  </div>

  <div class="cream-float" style="top: 40%; right: 3%; animation-delay: 1.5s;">
    <svg width="55" height="60" viewBox="0 0 100 100">
      <polygon points="50,95 30,55 70,55" fill="#ffe9a8" stroke="#e8a921" stroke-width="2"/>
      <circle cx="50" cy="45" r="20" fill="#fff" stroke="#4a7fd4" stroke-width="2"/>
      <circle cx="38" cy="40" r="8" fill="#a8c8ff" stroke="#4a7fd4" stroke-width="1.5"/>
      <circle cx="62" cy="42" r="8" fill="#ffe9a8" stroke="#e8a921" stroke-width="1.5"/>
      <circle cx="50" cy="32" r="8" fill="#b8e6d9" stroke="#7ac0ab" stroke-width="1.5"/>
      <circle cx="50" cy="20" r="3" fill="#ff6b6b"/>
    </svg>
  </div>

  <div class="cream-float" style="bottom: 15%; left: 5%; animation-delay: 3s;">
    <svg width="55" height="55" viewBox="0 0 100 100">
      <circle cx="50" cy="50" r="42" fill="#ffe9a8" stroke="#e8a921" stroke-width="2"/>
      <circle cx="50" cy="50" r="42" fill="none" stroke="#fff" stroke-width="3" stroke-dasharray="4,4" opacity="0.6"/>
      <circle cx="50" cy="50" r="14" fill="#fffdf7" stroke="#e8a921" stroke-width="2"/>
      <circle cx="35" cy="35" r="3" fill="#ff6b6b"/>
      <circle cx="65" cy="38" r="3" fill="#4a7fd4"/>
      <circle cx="38" cy="65" r="3" fill="#b8e6d9"/>
      <circle cx="68" cy="62" r="3" fill="#ff6b6b"/>
    </svg>
  </div>

  <div class="cream-float" style="bottom: 8%; right: 8%; animation-delay: 2s;">
    <svg width="65" height="70" viewBox="0 0 100 100">
      <ellipse cx="50" cy="92" rx="35" ry="6" fill="#e8a921" opacity="0.3"/>
      <path d="M22 62 L30 90 L70 90 L78 62 Z" fill="#a8c8ff" stroke="#4a7fd4" stroke-width="2"/>
      <line x1="30" y1="70" x2="70" y2="70" stroke="#4a7fd4" stroke-width="1.5" opacity="0.5"/>
      <line x1="28" y1="80" x2="72" y2="80" stroke="#4a7fd4" stroke-width="1.5" opacity="0.5"/>
      <ellipse cx="50" cy="60" rx="32" ry="10" fill="#fff" stroke="#1e4fa3" stroke-width="2"/>
      <ellipse cx="50" cy="50" rx="26" ry="9" fill="#fff" stroke="#1e4fa3" stroke-width="2"/>
      <ellipse cx="50" cy="41" rx="20" ry="8" fill="#fff" stroke="#1e4fa3" stroke-width="2"/>
      <ellipse cx="50" cy="33" rx="13" ry="6" fill="#fff" stroke="#1e4fa3" stroke-width="2"/>
      <circle cx="50" cy="26" r="5" fill="#ff6b6b" stroke="#c92a2a" stroke-width="1.5"/>
      <path d="M50 21 Q 53 15 58 13" fill="none" stroke="#2b8a3e" stroke-width="1.5" stroke-linecap="round"/>
      <circle cx="35" cy="58" r="1.5" fill="#ffc93c"/>
      <circle cx="65" cy="52" r="1.5" fill="#b8e6d9"/>
      <circle cx="42" cy="45" r="1.5" fill="#ff6b6b"/>
    </svg>
  </div>

  <!-- Sprinkle statis -->
  <div class="sprinkle-static"      style="top: 15%; left: 25%; background: #ffc93c; animation-delay: 0s;"></div>
  <div class="sprinkle-static pill" style="top: 22%; right: 30%; background: #a8c8ff; animation-delay: 1s;"></div>
  <div class="sprinkle-static"      style="top: 55%; left: 15%; background: #ffd93d; animation-delay: 2s;"></div>
  <div class="sprinkle-static pill" style="top: 70%; right: 20%; background: #4a7fd4; animation-delay: 0.5s;"></div>
  <div class="sprinkle-static"      style="top: 85%; left: 30%; background: #b8e6d9; animation-delay: 1.5s;"></div>

  <!-- ============ NAVBAR ============ -->
  <nav>
    <div class="nav-inner">
      <a href="#" class="logo">
        <span class="logo-mark"><i class="fas fa-feather-alt"></i></span>
        Ayu Cintya
      </a>
      <div class="nav-links">
        <a href="#about">Tentang</a>
        <a href="#nama">Nama</a>
        <a href="#funfact">Things</a>
        <a href="#warna">Warna</a>
        <a href="#comment">Komentar</a>
        <a href="#quote">Quote</a>
      </div>
      <a href="#quote" class="btn btn-primary">
        <i class="fas fa-paper-plane"></i> Sapa Ayu
      </a>
    </div>
  </nav>

  <!-- ============ HERO ============ -->
  <section class="hero">
    <span class="doodle-star" style="position:absolute; top:12%; left:6%;">✦</span>
    <span class="doodle-star" style="position:absolute; top:22%; right:8%; animation-delay:1s;">✦</span>
    <span class="doodle-star" style="position:absolute; bottom:18%; left:3%; animation-delay:2s;">✦</span>
    <span style="position:absolute; bottom:10%; right:12%; font-size:1.8rem; opacity:0.6; animation:float 5s ease-in-out infinite;">💤</span>

    <div class="container hero-grid">
      <div class="hero-text">
        <div class="hero-badge">
          <i class="fas fa-star"></i> Ruang kecil penuh warna
        </div>
        <h1>Hai, aku <span class="highlight">Ayu Cintya</span> Nirmala</h1>
        <p class="lead">
          Seorang pemburu inspirasi yang percaya bahwa hidup jadi lebih indah
          kalau ada gambar, tidur cukup, dan semangkuk mie ayam hangat. 🍜
        </p>
      </div>

      <div class="hero-visual">
        <div class="float-card fc-1"><i class="fas fa-paint-brush"></i> Suka Menggambar</div>
        <div class="float-card fc-2"><i class="fas fa-cat"></i> Pecinta Kucing</div>
        <div class="float-card fc-3"><i class="fas fa-candy-cane"></i> No Sugar No Life</div>

        <div class="profile-card">
          <div class="avatar-ring"><div class="avatar">A</div></div>
          <h3>Ayu Cintya Nirmala</h3>
          <div class="role">✦ Dreamer & Illustrator ✦</div>
          <p class="quote">
            "Gambar adalah caraku bercerita, dan tidur adalah caraku mengisi ulang cerita itu."
          </p>
          <div class="chips">
            <span class="chip"><i class="fas fa-pencil-ruler"></i> Menggambar</span>
            <span class="chip"><i class="fas fa-bed"></i> Tidur</span>
            <span class="chip"><i class="fas fa-bowl-food"></i> Mie Ayam</span>
            <span class="chip"><i class="fas fa-utensil-spoon"></i> Kapurung</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- BANNER POLKADOT #1 -->
  <div class="polkadot-banner">
    <div class="polkadot-banner-text">
      <i class="fas fa-star"></i>
      Ayu Cintya Nirmala
      <i class="fas fa-heart"></i>
    </div>
  </div>

  <!-- ============ CONTENT PAGE ============ -->
  <section class="content-page" id="content-page">
    <span class="sparkle" style="top:10%; left:6%;">✦</span>
    <span class="sparkle" style="bottom:14%; right:8%; animation-delay:1.2s;">✦</span>

    <div class="container">
      <div class="section-head">
        <span class="kicker">Daftar Isi</span>
        <h2>Mau Mulai dari Mana?</h2>
      </div>

      <div class="content-grid">
        <a href="#about" class="content-card c-about"><div class="content-num">01</div><div class="content-title">Tentang</div></a>
        <a href="#nama" class="content-card c-nama"><div class="content-num">02</div><div class="content-title">Nama</div></a>
        <a href="#funfact" class="content-card c-things"><div class="content-num">03</div><div class="content-title">Things</div></a>
        <a href="#warna" class="content-card c-warna"><div class="content-num">04</div><div class="content-title">Warna</div></a>
        <a href="#funfact-ayu" class="content-card c-funfact"><div class="content-num">05</div><div class="content-title">Funfact</div></a>
        <a href="#mbti" class="content-card c-mbti"><div class="content-num">06</div><div class="content-title">MBTI</div></a>
        <a href="#hobi" class="content-card c-hobi"><div class="content-num">07</div><div class="content-title">Hobi</div></a>
        <a href="#makanan" class="content-card c-makanan"><div class="content-num">08</div><div class="content-title">Makanan</div></a>
        <a href="#mood" class="content-card c-mood"><div class="content-num">09</div><div class="content-title">Mood</div></a>
        <a href="#comment" class="content-card c-comment"><div class="content-num">10</div><div class="content-title">Komentar</div></a>
      </div>
    </div>
  </section>

  <!-- ============ ABOUT + BIODATA ============ -->
  <section class="about" id="about">
    <span class="sparkle" style="top:10%; right:10%;">✦</span>
    <span class="sparkle" style="bottom:15%; left:8%; animation-delay:1s;">✦</span>

    <div class="container about-grid">
      <div class="about-visual">
        <div class="about-img-main">
          <img src="https://images.unsplash.com/photo-1508615039623-a25605d2b022?w=500&q=80" alt="Lukisan bunga">
        </div>
        <div class="about-img-secondary">
          <img src="https://images.unsplash.com/photo-1557682224-5b8590cd9ec5?w=500&q=80" alt="Polkadot">
        </div>
      </div>

      <div class="about-content">
        <span class="kicker" style="display:block; font-size:0.8rem; font-weight:700; letter-spacing:0.15em; text-transform:uppercase; color:var(--honey); margin-bottom:0.8rem;">✦ Tentang Ayu ✦</span>
        <h2>Ayu Cintya Nirmala</h2>

        <div class="biodata">
          <div class="bio-item">
            <div class="bio-icon"><i class="fas fa-birthday-cake"></i></div>
            <div class="bio-info">
              <span class="bio-label">Umur</span>
              <span class="bio-value">18 tahun</span>
            </div>
          </div>

          <div class="bio-item">
            <div class="bio-icon"><i class="fas fa-graduation-cap"></i></div>
            <div class="bio-info">
              <span class="bio-label">Alumni</span>
              <span class="bio-value">SMA Negeri 3 Kota Palopo, Sulawesi Selatan</span>
            </div>
          </div>

          <div class="bio-item">
            <div class="bio-icon"><i class="fas fa-university"></i></div>
            <div class="bio-info">
              <span class="bio-label">Kuliah</span>
              <span class="bio-value">UIN Palopo — S1 Perbankan Syariah</span>
            </div>
          </div>

          <div class="bio-item">
            <div class="bio-icon"><i class="fas fa-landmark"></i></div>
            <div class="bio-info">
              <span class="bio-label">Fakultas</span>
              <span class="bio-value">FEBI (Fakultas Ekonomi & Bisnis Islam)</span>
            </div>
          </div>
        </div>

        <p class="about-text">
          Aku suka biru — bukan cuma karena indah dipandang, tapi karena biru
          adalah elemen kehidupan yang melambangkan <strong>ketenangan, hati
          yang jernih, dan kemurnian</strong>. Seperti langit yang luas dan laut
          yang dalam, biru mengingatkanku untuk tetap tenang, jernih, dan murni
          dalam menjalani hari.
        </p>
        <div class="blue-philosophy">
          <i class="fas fa-water"></i>
          <strong>Biru</strong> mengajarkanku bahwa kedalaman tidak harus berisik.
          Kadang, ketenangan justru yang paling kuat.
        </div>
        <p class="about-text">
          Di balik semua itu, aku juga manusia biasa yang hobinya menggambar,
          tidur, dan jatuh cinta pada mie ayam & kapurung. Selamat menjelajahi
          ruang kecilku ini. 💙
        </p>
      </div>
    </div>
  </section>

  <!-- BANNER POLKADOT #2 -->
  <div class="polkadot-banner">
    <div class="polkadot-banner-text">
      <i class="fas fa-star"></i>
      Ruang Kecil Penuh Warna
      <i class="fas fa-heart"></i>
    </div>
  </div>

  <!-- ============ NAMA ============ -->
  <section class="nama" id="nama">
    <span class="sparkle" style="top:12%; left:8%;">✦</span>
    <span class="sparkle" style="bottom:18%; right:10%; animation-delay:1.2s;">✦</span>

    <div class="container">
      <div class="section-head">
        <span class="kicker">Nama & Makna</span>
        <h2>Ayu Cintya Nirmala — Satu Nama, Tiga Cerita</h2>
        <p>Di balik setiap kata dalam namaku, ada makna yang indah — tapi satu yang paling bersinar.</p>
      </div>

      <div class="nama-grid">
        <div class="nama-visual">
          <div class="nama-circle">
            <div class="nama-word">
              <span class="nama-kecil">✦ Ayu Cintya ✦</span>
              <span class="nama-besar">Nirmala</span>
              <small>✦ Murni & Tanpa Noda ✦</small>
            </div>
          </div>
          <div class="nama-tag-float nama-tag-1"><i class="fas fa-feather-alt"></i> Sanskerta</div>
          <div class="nama-tag-float nama-tag-2"><i class="fas fa-palette"></i> Nirmana</div>
          <div class="nama-tag-float nama-tag-3"><i class="fas fa-heart"></i> Favoritku</div>
        </div>

        <div class="nama-content">
          <p>
            Namaku terdiri dari tiga kata, dan masing-masing punya makna yang
            indah. <strong>Ayu</strong> berasal dari bahasa Jawa Kuno yang
            berarti "cantik" atau "indah". <strong>Cintya</strong> berasal dari
            bahasa Sanskerta yang berarti "pikiran" atau "kesadaran".
          </p>
          <p>
            Tapi dari ketiganya, <strong>aku paling menyukai nama akhirku:
            Nirmala</strong>. Kata ini berasal dari bahasa Sanskerta:
            <em>nir</em> artinya "tanpa", dan <em>mala</em> artinya "noda".
            Jadi, <strong>Nirmala berarti "yang murni", "tanpa cela", atau
            "bersih sepenuhnya"</strong>.
          </p>
          <p>
            Dan kalau dipelesetkan sedikit, <strong>Nirmala → Nirmana</strong>.
            <strong>Nirmana adalah dasar dari seni rupa dan desain</strong> —
            ilmu menyusun elemen visual menjadi kesatuan yang harmonis.
          </p>
          <div class="nama-quote">
            <i class="fas fa-quote-left"></i>
            Jadi mungkin… aku memang sudah ditakdirkan untuk menyukai seni.
            Namaku murni, dan pelesetannya adalah fondasi tempat para seniman
            belajar berkarya. 💙
          </div>
          <div class="nama-tags">
            <span>✦ Ayu = Cantik</span>
            <span>✦ Cintya = Pikiran</span>
            <span>✦ Nirmala = Murni</span>
            <span>✦ Nirmana = Dasar Seni Rupa</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ============ THINGS THAT MAKE ME ME (SLIDER) ============ -->
  <section class="funfact" id="funfact">
    <span class="sparkle" style="top:8%; left:6%;">✦</span>
    <span class="sparkle" style="top:20%; right:12%; animation-delay:0.8s;">✦</span>
    <span class="sparkle" style="bottom:10%; left:15%; animation-delay:1.5s;">✦</span>

    <div class="container">
      <div class="section-head">
        <span class="kicker">Things That Make Me Me</span>
        <h2>Empat Hal yang Membuatku Jadi Aku</h2>
        <p>Geser kartunya, lalu ketuk untuk lihat daftar lengkapnya. 💙💛</p>
      </div>
    </div>

    <div class="slider-hint">
      <i class="fas fa-arrow-left"></i> Geser & Ketuk Kartunya <i class="fas fa-arrow-right"></i>
    </div>

    <div class="slider-wrap">
      <div class="slider-track">
        <div class="slide-card hobby" onclick="openModal('modal-hobi')">
          <div class="slide-icon"><i class="fas fa-paint-brush"></i></div>
          <h3>Tidur & Menggambar</h3>
          <p>Menggambar adalah caraku bercerita, dan tidur adalah caraku mengisi ulang cerita itu.</p>
          <span class="slide-cta"><i class="fas fa-hand-pointer"></i> Ketuk untuk lihat</span>
        </div>
        <div class="slide-card sweet" onclick="openModal('modal-makanan')">
          <div class="slide-icon"><i class="fas fa-candy-cane"></i></div>
          <h3>Makanan Favorit</h3>
          <p>No sugar no life! Ditambah kapurung dan mie ayam.</p>
          <span class="slide-cta"><i class="fas fa-hand-pointer"></i> Ketuk untuk lihat</span>
        </div>
        <div class="slide-card music" onclick="openModal('modal-musik')">
          <div class="slide-icon"><i class="fas fa-music"></i></div>
          <h3>Band/Artist Favorit</h3>
          <p>Delapan nama yang selalu menemani hari-hariku.</p>
          <span class="slide-cta"><i class="fas fa-hand-pointer"></i> Ketuk untuk lihat</span>
        </div>
        <div class="slide-card movie" onclick="openModal('modal-film')">
          <div class="slide-icon"><i class="fas fa-film"></i></div>
          <h3>My Comfort Movies</h3>
          <p>Enam film yang selalu menemani waktu santai.</p>
          <span class="slide-cta"><i class="fas fa-hand-pointer"></i> Ketuk untuk lihat</span>
        </div>
      </div>
    </div>
  </section>

  <!-- MODALS -->
  <div class="modal-overlay" id="modal-hobi" onclick="closeModal(event)">
    <div class="modal-box">
      <button class="modal-close" onclick="closeModal(event)">×</button>
      <div class="modal-icon" style="background: var(--blue); color: var(--sun);"><i class="fas fa-paint-brush"></i></div>
      <h3>Tidur & Menggambar</h3>
      <p class="modal-sub">Dua dunia yang bikin hidupku seimbang</p>
      <ul class="modal-list">
        <li><i class="fas fa-paint-brush"></i> Menggambar sketsa & doodle</li>
        <li><i class="fas fa-palette"></i> Digital art & ilustrasi</li>
        <li><i class="fas fa-bed"></i> Power nap & tidur panjang</li>
        <li><i class="fas fa-cloud"></i> Deep sleep untuk isi ulang energi</li>
        <li><i class="fas fa-star"></i> Bangun dengan inspirasi segar</li>
      </ul>
    </div>
  </div>

  <div class="modal-overlay" id="modal-makanan" onclick="closeModal(event)">
    <div class="modal-box">
      <button class="modal-close" onclick="closeModal(event)">×</button>
      <div class="modal-icon" style="background: linear-gradient(135deg, var(--pink), var(--sun-soft)); color: var(--navy);"><i class="fas fa-candy-cane"></i></div>
      <h3>Makanan Favorit</h3>
      <p class="modal-sub">No sugar, no life 🍰</p>
      <ul class="modal-list">
        <li><i class="fas fa-cake-candles"></i> Kue & dessert manis</li>
        <li><i class="fas fa-candy-cane"></i> Permen & jajanan manis</li>
        <li><i class="fas fa-ice-cream"></i> Minuman manis & es krim</li>
        <li><i class="fas fa-bowl-food"></i> Mie ayam hangat</li>
        <li><i class="fas fa-utensil-spoon"></i> Kapurung khas Sulawesi</li>
      </ul>
    </div>
  </div>

  <div class="modal-overlay" id="modal-musik" onclick="closeModal(event)">
    <div class="modal-box">
      <button class="modal-close" onclick="closeModal(event)">×</button>
      <div class="modal-icon" style="background: linear-gradient(135deg, var(--blue), var(--sky)); color: var(--sun);"><i class="fas fa-music"></i></div>
      <h3>Band/Artist Favorit</h3>
      <p class="modal-sub">Delapan nama di hati 🎧</p>
      <ul class="modal-list">
        <li><i class="fas fa-star"></i> The Marías</li>
        <li><i class="fas fa-star"></i> Olivia Rodrigo</li>
        <li><i class="fas fa-star"></i> MARINA</li>
        <li><i class="fas fa-star"></i> TV Girl</li>
        <li><i class="fas fa-star"></i> NewJeans</li>
        <li><i class="fas fa-star"></i> NIKI</li>
        <li><i class="fas fa-star"></i> PinkPantheress</li>
        <li><i class="fas fa-star"></i> Bruno Mars</li>
      </ul>
    </div>
  </div>

  <div class="modal-overlay" id="modal-film" onclick="closeModal(event)">
    <div class="modal-box">
      <button class="modal-close" onclick="closeModal(event)">×</button>
      <div class="modal-icon" style="background: linear-gradient(135deg, var(--sun), var(--honey)); color: var(--navy);"><i class="fas fa-film"></i></div>
      <h3>My Comfort Movies</h3>
      <p class="modal-sub">Enam film yang menemani waktu santai 🎬</p>
      <ul class="modal-list">
        <li><i class="fas fa-hat-wizard"></i> Harry Potter</li>
        <li><i class="fas fa-watermelon"></i> Twinkling Watermelon</li>
        <li><i class="fas fa-running"></i> The Maze Runner</li>
        <li><i class="fas fa-lion"></i> Narnia</li>
        <li><i class="fas fa-graduation-cap"></i> 3 Idiots</li>
        <li><i class="fas fa-dragon"></i> How to Train Your Dragon</li>
      </ul>
    </div>
  </div>

  <!-- ============ WARNA ============ -->
  <section class="warna" id="warna">
    <span class="sparkle" style="top:12%; left:8%;">✦</span>
    <span class="sparkle" style="bottom:18%; right:10%; animation-delay:1.2s;">✦</span>

    <div class="container">
      <div class="section-head">
        <span class="kicker">Warna Favorit</span>
        <h2>Palet Warna Kehidupanku</h2>
        <p>Setiap warna punya cerita, dan ini warna-warna yang paling mewakiliku. 🎨</p>
      </div>

      <div class="warna-grid">
        <div class="color-wheel-wrap">
          <span class="color-dot-float cd-1"></span>
          <span class="color-dot-float cd-2"></span>
          <span class="color-dot-float cd-3"></span>
          <span class="color-dot-float cd-4"></span>
          <div class="color-wheel"></div>
          <div class="color-wheel-center">
            Warna<br>Favorit
            <small>✦ Color Wheel ✦</small>
          </div>
        </div>

        <div class="warna-content">
          <h2>Warna yang Menemaniku</h2>
          <p>
            Aku percaya setiap warna punya arti — dan warna-warna ini yang
            paling mewakili diriku. <strong>Biru</strong> sebagai warna utama,
            melambangkan ketenangan dan kemurnian hati. <strong>Kuning</strong>
            sebagai aksen, membawa kehangatan dan keceriaan.
          </p>
          <div class="warna-palette">
            <div class="warna-swatch" style="background: #1e4fa3;">Biru</div>
            <div class="warna-swatch" style="background: #4a7fd4;">Blue Soft</div>
            <div class="warna-swatch" style="background: #ffd93d; color: var(--navy);">Kuning</div>
            <div class="warna-swatch" style="background: #ffe9a8; color: var(--navy);">Pastel</div>
            <div class="warna-swatch" style="background: #ff6b6b;">Merah</div>
            <div class="warna-swatch" style="background: #ffb3c6; color: var(--navy);">Pink</div>
            <div class="warna-swatch" style="background: #b8e6d9; color: var(--navy);">Mint</div>
            <div class="warna-swatch" style="background: #a78bfa;">Ungu</div>
          </div>
          <div class="warna-tags">
            <span>💙 Biru = Ketenangan</span>
            <span>💛 Kuning Pastel = Kelembutan</span>
            <span>💗 Pink = Lembut</span>
            <span>💜 Ungu = Mimpi</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- BANNER POLKADOT #3 (tipis) -->
  <div class="polkadot-banner thin">
    <div class="polkadot-banner-text">
      <i class="fas fa-star"></i>
      Dreamer & Illustrator
      <i class="fas fa-heart"></i>
    </div>
  </div>

  <!-- ============ FUNFACT AYU ============ -->
  <section class="funfact-ayu" id="funfact-ayu">
    <span class="sparkle" style="top:12%; left:8%;">✦</span>
    <span class="sparkle" style="bottom:18%; right:10%; animation-delay:1.2s;">✦</span>

    <div class="container">
      <div class="section-head">
        <span class="kicker">Funfact Ayu</span>
        <h2>Dua Fakta Random Tentangku</h2>
        <p>Hal-hal kecil yang mungkin bikin kamu senyum (atau ketawa). 💙</p>
      </div>

      <div class="funfact-ayu-grid">
        <div class="fun-card cat">
          <div class="fun-icon"><i class="fas fa-cat"></i></div>
          <h3>Suka Kucing, Tapi Tidak Pelihara</h3>
          <p>
            Setiap berkunjung ke rumah teman, hal pertama yang kucari bukan
            temannya — melainkan kucing imut gemasnya. Tapi sesuka-sukanya
            aku sama kucing, aku tidak pelihara karena dilarang. 🐱
          </p>
          <span class="fun-tag">🐱 Magnet Pertama</span>
        </div>

        <div class="fun-card direction">
          <div class="fun-icon"><i class="fas fa-compass"></i></div>
          <h3>Kalau Soal Jalan, Jangan Tanya Aku</h3>
          <p>
            Serius, jangan tanya aku soal arah jalan kalau tidak mau kita
            tersesat. Aku tidak pandai mengingat arah — kadang jalan yang
            sama pun bisa bikin aku bingung. 🧭
          </p>
          <span class="fun-tag">🧭 Tersesat Ahli</span>
        </div>
      </div>
    </div>
  </section>

  <!-- ============ MBTI ============ -->
  <section class="mbti-section" id="mbti">
    <div class="container">
      <div class="section-head">
        <span class="kicker">Me If I Was a Character</span>
        <h2>INTJ & Dua Karakter Fiksi yang Mirip Aku</h2>
        <p>Architect yang strategis, dengan hati yang penuh perasaan.</p>
      </div>

      <div class="mbti-grid">
        <div class="mbti-card intro">
          <div class="mbti-icon">🧠</div>
          <h3>INTJ — The Architect</h3>
          <p>
            INTJ adalah tipe kepribadian yang strategis, analitis, dan mandiri.
            Punya visi jangka panjang, suka merencanakan dengan matang, dan
            tidak takut berbeda. Di balik sikap rasional, INTJ sangat peduli
            dan punya dunia batin yang kaya.
          </p>
          <div class="mbti-traits">
            <span>Strategis</span>
            <span>Analitis</span>
            <span>Mandiri</span>
            <span>Visioner</span>
          </div>
        </div>

        <div class="mbti-card character">
          <div class="character-img">🐰</div>
          <h3>Anais Watterson</h3>
          <span class="character-from">The Amazing World of Gumball</span>
          <p>
            Adik kecil yang jauh lebih pintar dari keluarganya. Membantu PR
            kakak-kakaknya, bikin sarapan, dan selalu punya rencana. Tapi di
            balik kecerdasannya, Anais masih punya sisi childish dan social
            awkward — persis seperti INTJ yang kompleks.
          </p>
          <div class="mbti-traits">
            <span>Cerdas</span>
            <span>Mature</span>
            <span>Socially Awkward</span>
          </div>
        </div>

        <div class="mbti-card character">
          <div class="character-img">🌙</div>
          <h3>Princess Luna</h3>
          <span class="character-from">My Little Pony</span>
          <p>
            Penguasa malam yang pernah menjadi Nightmare Moon karena
            kecemburuan. Setelah dikembalikan, Luna kesulitan beradaptasi dan
            sering tidak dipahami. Tapi di balik itu, dia melindungi alam mimpi
            dan membantu poni lain — INTJ yang misunderstood tapi penuh empati.
          </p>
          <div class="mbti-traits">
            <span>Introvert</span>
            <span>Deep Thinker</span>
            <span>Misunderstood</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ============ HOBI ============ -->
  <section class="hobi" id="hobi">
    <div class="container">
      <div class="section-head">
        <span class="kicker">Hal yang kucintai</span>
        <h2>Dua Hobi, Dua Dunia</h2>
        <p>Ada saatnya aku jadi seniman, ada saatnya aku jadi ratu kasur. Dua-duanya bikin hidup seimbang.</p>
      </div>

      <div class="hobi-grid">
        <div class="hobi-card drawing">
          <div class="hobi-icon"><i class="fas fa-paint-brush"></i></div>
          <h3>Menggambar</h3>
          <p>
            Menumpahkan imajinasi ke atas kertas adalah terapi terbaikku.
            Dari sketsa kecil sampai ilustrasi penuh warna, setiap goresan
            punya ceritanya sendiri.
          </p>
          <div class="hobi-tags">
            <span><i class="fas fa-star"></i> Sketsa</span>
            <span><i class="fas fa-star"></i> Digital Art</span>
            <span><i class="fas fa-star"></i> Doodle</span>
          </div>
        </div>

        <div class="hobi-card sleeping">
          <div class="hobi-icon"><i class="fas fa-bed"></i></div>
          <h3>Tidur</h3>
          <p>
            Bukan sekadar hobi, tapi seni. Tidur yang cukup bikin pikiran
            jernih, mood bagus, dan inspirasi gambar datang lebih cepat.
            Serius, ini produktif!
          </p>
          <div class="hobi-tags">
            <span><i class="fas fa-moon"></i> Power Nap</span>
            <span><i class="fas fa-cloud"></i> Deep Sleep</span>
            <span><i class="fas fa-sun"></i> Bangun Fresh</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ============ MAKANAN ============ -->
  <section class="makanan" id="makanan">
    <div class="container">
      <div class="section-head">
        <span class="kicker">Makanan Favorit</span>
        <h2>Dua Makanan, Satu Cinta</h2>
        <p>Kalau ditanya mau makan apa, jawabannya selalu dua ini. Gak pernah bosan.</p>
      </div>

      <div class="food-grid">
        <div class="food-card mie-ayam">
          <div class="food-emoji">🍜</div>
          <h3>Mie Ayam</h3>
          <p>
            Kuah hangat, mie kenyal, topping ayam kecap yang manis-gurih.
            Ditambah sedikit sambal dan acar — sempurna untuk kapan saja.
          </p>
          <div class="rating">
            <i class="fas fa-star"></i><i class="fas fa-star"></i>
            <i class="fas fa-star"></i><i class="fas fa-star"></i>
            <i class="fas fa-star"></i>
            <span>Rating 5.0</span>
          </div>
          <span class="food-note">🍜 Comfort food sejati</span>
        </div>

        <div class="food-card kapurung">
          <div class="food-emoji">🥣</div>
          <h3>Kapurung</h3>
          <p>
            Makanan khas Sulawesi Selatan yang bikin kangen. Perpaduan sagu,
            sayur, dan kuah ikan yang segar — selalu berhasil bikin hati hangat.
          </p>
          <div class="rating">
            <i class="fas fa-star"></i><i class="fas fa-star"></i>
            <i class="fas fa-star"></i><i class="fas fa-star"></i>
            <i class="fas fa-star"></i>
            <span>Rating 5.0</span>
          </div>
          <span class="food-note">🥣 Rasa kampung halaman</span>
        </div>
      </div>
    </div>
  </section>

  <!-- ============ MOOD ============ -->
  <section class="mood" id="mood">
    <div class="container">
      <div class="section-head">
        <span class="kicker">Moodboard</span>
        <h2>Warna-Warni Hari Ayu</h2>
        <p>Sedikit cuplikan suasana hati yang sering muncul dalam keseharian.</p>
      </div>

      <div class="mood-grid">
        <div class="mood-item" style="background: var(--sky-soft);">🎨 <span>Kreatif</span></div>
        <div class="mood-item" style="background: var(--sun-glow);">😴 <span>Ngantuk</span></div>
        <div class="mood-item" style="background: var(--sky);">✨ <span>Bersinar</span></div>
        <div class="mood-item" style="background: var(--sun-soft);">🍜 <span>Laper</span></div>
        <div class="mood-item" style="background: var(--sky-soft);">☁️ <span>Tenang</span></div>
        <div class="mood-item" style="background: var(--sun-glow);">🐱 <span>Kucing</span></div>
        <div class="mood-item" style="background: var(--sky);">🖌️ <span>Produktif</span></div>
        <div class="mood-item" style="background: var(--sun-soft);">🍰 <span>Manis</span></div>
      </div>
    </div>
  </section>

  <!-- ============ COMMENT SECTION ============ -->
  <section class="comment-section" id="comment">
    <span class="sparkle" style="top:10%; left:6%;">✦</span>
    <span class="sparkle" style="bottom:14%; right:8%; animation-delay:1.2s;">✦</span>

    <div class="container">
      <div class="comment-intro">
        <span class="kicker">About Me — Kritik & Saran</span>
        <h2>Ceritakan Pendapatmu Tentangku</h2>
        <p>Silakan tinggalkan kritik, saran, atau pesan untukku. Semua akan kubaca dengan hati terbuka. 💙</p>
      </div>

      <div class="comment-grid">
        <div class="comment-form-wrap">
          <h3><i class="fas fa-pen-fancy"></i> Tulis Pesanmu</h3>
          <form id="commentForm" onsubmit="submitComment(event)">
            <div class="form-group">
              <label for="nama">Nama Kamu</label>
              <input type="text" id="nama" placeholder="Contoh: Budi" maxlength="30" required>
            </div>
            <div class="form-group">
              <label for="jenis">Jenis Pesan</label>
              <select id="jenis" required>
                <option value="pujian">💙 Pujian</option>
                <option value="saran">💡 Saran</option>
                <option value="kritik">📝 Kritik</option>
              </select>
            </div>
            <div class="form-group">
              <label for="pesan">Pesanmu</label>
              <textarea id="pesan" placeholder="Tulis pesanmu di sini..." maxlength="500" required></textarea>
            </div>
            <button type="submit" class="btn-send" id="btnKirim">
              <i class="fas fa-paper-plane"></i> Kirim Pesan
            </button>
          </form>
        </div>

        <div class="comment-list-wrap">
          <div class="comment-list-header">
            <h3><i class="fas fa-comments"></i> Pesan Masuk</h3>
            <span class="comment-count" id="commentCount">0 pesan</span>
          </div>
          <div class="comment-list" id="commentList">
            <div class="comment-empty">
              <i class="fas fa-inbox"></i>
              Belum ada pesan. Jadilah yang pertama! ✨
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ============ QUOTE ============ -->
  <section class="quote-section" id="quote">
    <div class="container">
      <div class="quote-card">
        <span class="qmark">"</span>
        <blockquote>
          Hidup itu seperti kanvas kosong — kita bebas memilih warna,
          kapan harus istirahat, dan makanan apa yang menemani.
        </blockquote>
        <div class="author">— Ayu Cintya Nirmala</div>
        <a href="#" class="btn btn-sun">
          <i class="fas fa-heart"></i> Terima Kasih Sudah Mampir
        </a>
      </div>
    </div>
  </section>

  <!-- BANNER POLKADOT #4 -->
  <div class="polkadot-banner">
    <div class="polkadot-banner-text">
      <i class="fas fa-star"></i>
      Let's Be Friend
      <i class="fas fa-heart"></i>
    </div>
  </div>

  <!-- ============ FOOTER ============ -->
  <footer>
    <div class="container">
      <div class="socials">
        <a href="https://www.instagram.com/ayl_0jjh?stkn=ejhsM3pvYTR3anJ1"
           target="_blank" rel="noopener" class="sosial-bubble bubble-ig">
          <div class="bubble-icon"><i class="fab fa-instagram"></i></div>
          <div class="bubble-text">
            <span class="bubble-title">Let's be friend</span>
            <span class="bubble-sub">@ayl_0jjh</span>
          </div>
        </a>

        <a href="https://www.roblox.com/share?code=7b0d205e21606c4dbf4b12f5af6d54ad&type=Profile&source=ProfileShare&stamp=1790380900748"
           target="_blank" rel="noopener" class="sosial-bubble bubble-roblox">
          <div class="bubble-icon"><i class="fas fa-gamepad"></i></div>
          <div class="bubble-text">
            <span class="bubble-title">Add me</span>
            <span class="bubble-sub">nirluvmaa</span>
          </div>
        </a>

        <a href="https://wa.me/qr/F42XHFVSSRIAO1"
           target="_blank" rel="noopener" class="sosial-bubble bubble-wa">
          <div class="bubble-icon"><i class="fab fa-whatsapp"></i></div>
          <div class="bubble-text">
            <span class="bubble-title">Contact person</span>
            <span class="bubble-sub">+62 878-6769-6714</span>
          </div>
        </a>
      </div>
      <p class="footer-text">
        Dibuat dengan <span class="footer-heart">♥</span> oleh Ayu Cintya Nirmala &copy; 2025
      </p>
    </div>
  </footer>

  <!-- ============ MUSIC PLAYER — LO-FI DREAMY ============ -->
  <div class="music-player" id="musicPlayer">
    <button class="music-btn" id="musicBtn" onclick="toggleMusic()" aria-label="Play music">
      <i class="fas fa-play" id="musicIcon"></i>
    </button>
    <div class="music-info">
      <div class="music-title" id="musicTitle">Dreamy Lofi</div>
      <div class="music-artist" id="musicArtist">Ayu Cintya Nirmala</div>
    </div>
    <div class="music-eq">
      <span></span><span></span><span></span><span></span>
    </div>
    <audio id="myAudio" loop preload="auto" crossorigin="anonymous">
      <source src="https://cdn.pixabay.com/download/audio/2022/05/27/audio_1808fbf07a.mp3?filename=lofi-study-112191.mp3" type="audio/mpeg">
      <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
    </audio>
  </div>

  <script>
    /* ============ INTRO ANIMASI + JELLY + AUTOPLAY MUSIC ============ */
    function skipIntro() {
      var overlay = document.getElementById('introOverlay');
      if (overlay) {
        overlay.classList.add('hide');
        setTimeout(function() {
          overlay.style.display = 'none';
        }, 800);
      }
      tryAutoplayMusic();
    }

    function tryAutoplayMusic() {
      var audioEl = document.getElementById('myAudio');
      var iconEl = document.getElementById('musicIcon');
      var playerEl = document.getElementById('musicPlayer');
      if (!audioEl) return;
      audioEl.volume = 0.45;
      var playPromise = audioEl.play();
      if (playPromise !== undefined) {
        playPromise.then(function() {
          if (iconEl) iconEl.className = 'fas fa-pause';
          if (playerEl) playerEl.classList.add('playing');
        }).catch(function() {
          console.log('Autoplay diblokir browser. User harus ketuk tombol ▶️ manual.');
        });
      }
    }

    document.addEventListener('DOMContentLoaded', function() {
      var overlay = document.getElementById('introOverlay');
      var introContent = document.getElementById('introContent');

      if (introContent) {
        setTimeout(function() {
          introContent.classList.add('jelly');
        }, 3700);
      }

      if (overlay) {
        setTimeout(function() {
          overlay.classList.add('hide');
          setTimeout(function() {
            overlay.style.display = 'none';
          }, 800);
          tryAutoplayMusic();
        }, 5500);

        overlay.addEventListener('click', function(e) {
          if (e.target.classList.contains('intro-overlay')) {
            skipIntro();
          }
        });
      }

      // Fallback: coba autoplay saat interaksi pertama (klik/scroll/touch)
      var interactionDone = false;
      function onFirstInteraction() {
        if (interactionDone) return;
        interactionDone = true;
        var audioEl = document.getElementById('myAudio');
        if (audioEl && audioEl.paused) {
          tryAutoplayMusic();
        }
      }
      document.addEventListener('click', onFirstInteraction, { once: true });
      document.addEventListener('touchstart', onFirstInteraction, { once: true });
      document.addEventListener('scroll', onFirstInteraction, { once: true });
    });

    /* ============ MODAL ============ */
    function openModal(id) {
      var modal = document.getElementById(id);
      if (modal) {
        modal.classList.add('active');
        document.body.style.overflow = 'hidden';
      }
    }
    function closeModal(event) {
      if (event.target.classList.contains('modal-overlay') ||
          event.target.classList.contains('modal-close')) {
        var modals = document.querySelectorAll('.modal-overlay');
        modals.forEach(function(m) { m.classList.remove('active'); });
        document.body.style.overflow = '';
      }
    }
    document.addEventListener('keydown', function(e) {
      if (e.key === 'Escape') {
        var modals = document.querySelectorAll('.modal-overlay');
        modals.forEach(function(m) { m.classList.remove('active'); });
        document.body.style.overflow = '';
      }
    });

    /* ============ COMMENT SECTION ============ */
    var STORAGE_KEY = 'ayu_comments_v1';
    var AVATAR_COLORS = [
      'linear-gradient(135deg, #1e4fa3, #4a7fd4)',
      'linear-gradient(135deg, #ffc93c, #e8a921)',
      'linear-gradient(135deg, #ffb3c6, #ff8fab)',
      'linear-gradient(135deg, #b8e6d9, #7ac0ab)',
      'linear-gradient(135deg, #a78bfa, #7c5cd6)',
      'linear-gradient(135deg, #4a7fd4, #ffc93c)',
      'linear-gradient(135deg, #ff6b6b, #ff8e53)',
      'linear-gradient(135deg, #0a1a3c, #1e4fa3)'
    ];

    function loadComments() {
      try {
        var raw = localStorage.getItem(STORAGE_KEY);
        return raw ? JSON.parse(raw) : [];
      } catch (e) { return []; }
    }
    function saveComments(list) {
      try { localStorage.setItem(STORAGE_KEY, JSON.stringify(list)); }
      catch (e) { console.warn('Gagal simpan komentar:', e); }
    }
    function escapeHTML(str) {
      return String(str)
        .replace(/&/g, '&amp;').replace(/</g, '&lt;')
        .replace(/>/g, '&gt;').replace(/"/g, '&quot;')
        .replace(/'/g, '&#39;');
    }
    function timeAgo(ts) {
      var diff = Math.floor((Date.now() - ts) / 1000);
      if (diff < 60) return 'baru saja';
      if (diff < 3600) return Math.floor(diff / 60) + ' menit lalu';
      if (diff < 86400) return Math.floor(diff / 3600) + ' jam lalu';
      if (diff < 604800) return Math.floor(diff / 86400) + ' hari lalu';
      var d = new Date(ts);
      return d.getDate() + '/' + (d.getMonth() + 1) + '/' + d.getFullYear();
    }
    function getBadgeLabel(type) {
      if (type === 'kritik') return '📝 Kritik';
      if (type === 'saran') return '💡 Saran';
      return '💙 Pujian';
    }
    function renderComments() {
      var list = loadComments().slice().reverse();
      var wrap = document.getElementById('commentList');
      var count = document.getElementById('commentCount');
      if (!wrap) return;
      count.textContent = list.length + ' pesan';
      if (list.length === 0) {
        wrap.innerHTML = '<div class="comment-empty"><i class="fas fa-inbox"></i>Belum ada pesan. Jadilah yang pertama! ✨</div>';
        return;
      }
      var html = '';
      list.forEach(function(c) {
        var colorIdx = (c.name || '').length % AVATAR_COLORS.length;
        var initial = (c.name || '?').trim().charAt(0).toUpperCase();
        html +=
          '<div class="comment-item">' +
            '<div class="comment-head">' +
              '<div class="comment-avatar" style="background:' + AVATAR_COLORS[colorIdx] + ';">' + escapeHTML(initial) + '</div>' +
              '<div class="comment-meta">' +
                '<div class="comment-name">' + escapeHTML(c.name) + '</div>' +
                '<div class="comment-time">' + timeAgo(c.time) + '</div>' +
              '</div>' +
              '<span class="comment-badge ' + (c.type || 'pujian') + '">' + getBadgeLabel(c.type) + '</span>' +
            '</div>' +
            '<div class="comment-body">' + escapeHTML(c.message).replace(/\n/g, '<br>') + '</div>' +
          '</div>';
      });
      wrap.innerHTML = html;
    }
    function submitComment(e) {
      e.preventDefault();
      var name = document.getElementById('nama').value.trim();
      var jenis = document.getElementById('jenis').value;
      var pesan = document.getElementById('pesan').value.trim();
      if (!name || !pesan) return;
      if (name.length > 30) return;
      if (pesan.length > 500) return;
      var list = loadComments();
      list.push({ name: name, type: jenis, message: pesan, time: Date.now() });
      saveComments(list);
      document.getElementById('commentForm').reset();
      renderComments();
    }
    document.addEventListener('DOMContentLoaded', renderComments);

    /* ============ MUSIC PLAYER TOGGLE ============ */
    var audio = document.getElementById('myAudio');
    var icon = document.getElementById('musicIcon');
    var player = document.getElementById('musicPlayer');
    audio.volume = 0.45;

    function toggleMusic() {
      if (audio.paused) {
        audio.play();
        icon.className = 'fas fa-pause';
        player.classList.add('playing');
      } else {
        audio.pause();
        icon.className = 'fas fa-play';
        player.classList.remove('playing');
      }
    }

    /* ============ DRAG & DROP HIASAN ============ */
    document.addEventListener('DOMContentLoaded', function() {
      var draggables = document.querySelectorAll('.sprinkle-static, .cream-float');

      draggables.forEach(function(el) {
        var isDragging = false;
        var startX = 0, startY = 0;
        var offsetX = 0, offsetY = 0;

        function onDown(e) {
          e.preventDefault();
          e.stopPropagation();
          isDragging = true;
          el.classList.add('dragging');
          var point = e.touches ? e.touches[0] : e;
          startX = point.clientX;
          startY = point.clientY;
          var rect = el.getBoundingClientRect();
          offsetX = startX - rect.left;
          offsetY = startY - rect.top;
          el.style.left = rect.left + 'px';
          el.style.top = rect.top + 'px';
          el.style.right = 'auto';
          el.style.bottom = 'auto';
          el.style.position = 'fixed';
          document.addEventListener('mousemove', onMove, { passive: false });
          document.addEventListener('mouseup', onUp);
          document.addEventListener('touchmove', onMove, { passive: false });
          document.addEventListener('touchend', onUp);
        }

        function onMove(e) {
          if (!isDragging) return;
          e.preventDefault();
          var point = e.touches ? e.touches[0] : e;
          var newLeft = point.clientX - offsetX;
          var newTop = point.clientY - offsetY;
          var maxLeft = window.innerWidth - el.offsetWidth;
          var maxTop = window.innerHeight - el.offsetHeight;
          newLeft = Math.max(0, Math.min(newLeft, maxLeft));
          newTop = Math.max(0, Math.min(newTop, maxTop));
          el.style.left = newLeft + 'px';
          el.style.top = newTop + 'px';
        }

        function onUp() {
          if (!isDragging) return;
          isDragging = false;
          el.classList.remove('dragging');
          document.removeEventListener('mousemove', onMove);
          document.removeEventListener('mouseup', onUp);
          document.removeEventListener('touchmove', onMove);
          document.removeEventListener('touchend', onUp);
        }

        el.addEventListener('mousedown', onDown);
        el.addEventListener('touchstart', onDown, { passive: false });
      });
    });
  </script>

</body>
</html>
<!-- ═══════════════════════════════════════════════════════════════
     BAGIAN 3 — CLOSING SECTION (GAME + PUISI FILSUF) FINAL
     
     📍 CARA PASTE:
     1) Blok <style> di bawah → paste SEBELUM </style> di <head>
     2) Blok <section> di bawah → paste SEBELUM </footer>
     3) Blok <script> di bawah → paste SEBELUM </script> terakhir
     ═══════════════════════════════════════════════════════════════ -->


<!-- ╔═══════════════════════════════════════════════════════════╗
     ║  BLOK 1 — CSS  (paste sebelum </style> di <head>)        ║
     ╚═══════════════════════════════════════════════════════════╝ -->
<style>
  /* ============ CLOSING SECTION (GAME + PUISI FILSUF) ============ */
  .closing-section {
    padding: 5rem 0 6rem;
    position: relative;
    background: linear-gradient(180deg, transparent 0%, var(--sun-glow) 30%, var(--sky-soft) 70%, transparent 100%);
    overflow: hidden;
  }

  /* Header */
  .closing-head {
    text-align: center;
    max-width: 720px;
    margin: 0 auto 3rem;
  }
  .closing-head .kicker {
    display: inline-block;
    font-size: 0.85rem;
    font-weight: 700;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: var(--honey);
    margin-bottom: 0.8rem;
  }
  .closing-head .kicker::before,
  .closing-head .kicker::after {
    content: '✦'; margin: 0 0.6rem; color: var(--sun); font-size: 0.7rem;
  }
  .closing-head h2 {
    font-size: clamp(2rem, 4vw, 2.8rem);
    margin-bottom: 1rem;
  }
  .closing-head p { color: var(--muted); font-size: 1.05rem; font-weight: 500; }

  /* ============ GAME: TANGKAP SPRINKLE ============ */
  .game-wrap {
    max-width: 640px;
    margin: 0 auto 4rem;
    background: #fff;
    border-radius: var(--radius);
    padding: 2rem 1.5rem;
    box-shadow: 0 30px 60px -30px rgba(30, 79, 163, 0.4);
    border: 2px dashed var(--sun);
    position: relative;
    z-index: 3;
  }
  .game-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 1rem;
    margin-bottom: 1.2rem;
    padding-bottom: 1rem;
    border-bottom: 2px dashed var(--sky);
  }
  .game-title {
    display: flex;
    align-items: center;
    gap: 0.6rem;
    font-family: 'Fraunces', serif;
    font-weight: 700;
    font-size: 1.2rem;
    color: var(--navy);
  }
  .game-title i { color: var(--honey); font-size: 1.3rem; }
  .game-stats {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
  }
  .game-stat {
    background: var(--sky-soft);
    padding: 0.4rem 0.9rem;
    border-radius: 50px;
    font-size: 0.85rem;
    font-weight: 700;
    color: var(--blue);
    display: flex;
    align-items: center;
    gap: 0.4rem;
  }
  .game-stat i { color: var(--honey); }
  .game-stat .stat-value {
    font-family: 'Fraunces', serif;
    color: var(--navy);
    font-size: 1rem;
    min-width: 1.5rem;
    text-align: center;
  }

  #gameArea {
    position: relative;
    width: 100%;
    height: 320px;
    background: linear-gradient(180deg, #eef4ff 0%, #fffdf7 100%);
    border-radius: var(--radius-sm);
    overflow: hidden;
    cursor: crosshair;
    user-select: none;
    -webkit-user-select: none;
    touch-action: none;
    border: 1px solid rgba(30, 79, 163, 0.1);
  }

  .game-sprinkle {
    position: absolute;
    width: 38px;
    height: 38px;
    border-radius: 50%;
    display: grid;
    place-items: center;
    font-size: 1.3rem;
    cursor: pointer;
    pointer-events: auto;
    transition: transform 0.15s ease;
    box-shadow: 0 6px 15px -5px rgba(30, 79, 163, 0.4);
    border: 3px solid #fff;
    animation: gameFall linear forwards;
    z-index: 5;
  }
  .game-sprinkle:hover { transform: scale(1.1); }
  .game-sprinkle.popped {
    animation: popAway 0.35s ease-out forwards !important;
    pointer-events: none;
  }
  @keyframes gameFall {
    from { top: -50px; transform: rotate(0deg); }
    to   { top: 100%;  transform: rotate(360deg); }
  }
  @keyframes popAway {
    0%   { transform: scale(1); opacity: 1; }
    50%  { transform: scale(1.6); opacity: 0.9; }
    100% { transform: scale(0); opacity: 0; }
  }

  .score-pop {
    position: absolute;
    font-family: 'Fraunces', serif;
    font-weight: 700;
    color: var(--honey);
    font-size: 1.1rem;
    pointer-events: none;
    animation: scorePop 0.7s ease-out forwards;
    z-index: 10;
  }
  @keyframes scorePop {
    0%   { transform: translateY(0) scale(0.8); opacity: 1; }
    100% { transform: translateY(-40px) scale(1.3); opacity: 0; }
  }

  .game-overlay {
    position: absolute;
    inset: 0;
    background: rgba(255, 253, 247, 0.92);
    backdrop-filter: blur(4px);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 1rem;
    padding: 1.5rem;
    text-align: center;
    z-index: 20;
    transition: opacity 0.3s ease;
  }
  .game-overlay.hidden { display: none; }
  .game-overlay h3 {
    font-size: 1.5rem;
    color: var(--navy);
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }
  .game-overlay h3 i { color: var(--honey); }
  .game-overlay p {
    color: var(--muted);
    font-weight: 500;
    font-size: 0.95rem;
    max-width: 380px;
    line-height: 1.6;
  }
  .game-btn {
    background: linear-gradient(135deg, var(--blue), var(--blue-soft));
    color: #fff;
    border: none;
    padding: 0.8rem 1.8rem;
    border-radius: 50px;
    font-family: 'Quicksand', sans-serif;
    font-weight: 700;
    font-size: 1rem;
    cursor: pointer;
    transition: all 0.28s ease;
    box-shadow: 0 12px 24px -10px rgba(30, 79, 163, 0.6);
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
  }
  .game-btn:hover {
    transform: translateY(-3px) scale(1.03);
    box-shadow: 0 18px 30px -10px rgba(30, 79, 163, 0.7);
  }
  .game-btn.sun {
    background: linear-gradient(135deg, var(--sun), var(--honey));
    color: var(--navy);
    box-shadow: 0 12px 24px -10px rgba(255, 201, 60, 0.8);
  }

  .game-reset {
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
    background: transparent;
    border: 2px solid var(--sky);
    color: var(--muted);
    padding: 0.4rem 0.9rem;
    border-radius: 50px;
    font-family: 'Quicksand', sans-serif;
    font-weight: 700;
    font-size: 0.75rem;
    cursor: pointer;
    transition: all 0.25s ease;
    margin-top: 1rem;
  }
  .game-reset:hover {
    border-color: var(--honey);
    color: var(--honey);
    transform: translateY(-2px);
  }

  /* ============ PUISI FILSUF ============ */
  .poem-section {
    max-width: 720px;
    margin: 0 auto;
    text-align: center;
    position: relative;
    z-index: 3;
  }
  .poem-card {
    background: linear-gradient(180deg, #fff 0%, var(--sun-glow) 100%);
    border-radius: var(--radius);
    padding: 3.5rem 2.5rem;
    box-shadow: 0 30px 60px -30px rgba(30, 79, 163, 0.35);
    border: 3px dashed var(--sun);
    position: relative;
    overflow: hidden;
  }
  .poem-card::before {
    content: '"';
    position: absolute;
    top: -20px;
    left: 20px;
    font-family: 'Fraunces', serif;
    font-size: 8rem;
    color: var(--sun-soft);
    opacity: 0.5;
    line-height: 1;
    pointer-events: none;
  }
  .poem-card::after {
    content: '"';
    position: absolute;
    bottom: -60px;
    right: 20px;
    font-family: 'Fraunces', serif;
    font-size: 8rem;
    color: var(--sun-soft);
    opacity: 0.5;
    line-height: 1;
    pointer-events: none;
  }
  .poem-title {
    font-family: 'Fraunces', serif;
    font-size: clamp(1.5rem, 3vw, 2rem);
    font-weight: 700;
    color: var(--blue);
    margin-bottom: 2rem;
    position: relative;
    z-index: 2;
  }
  .poem-title::after {
    content: '';
    display: block;
    width: 60px;
    height: 3px;
    background: var(--sun);
    border-radius: 3px;
    margin: 1rem auto 0;
  }
  .poem-line {
    font-family: 'Fraunces', serif;
    font-style: italic;
    font-size: 1.1rem;
    line-height: 1.9;
    color: var(--navy);
    opacity: 0;
    transform: translateY(15px);
    transition: opacity 0.8s ease, transform 0.8s ease;
    position: relative;
    z-index: 2;
    margin-bottom: 0.4rem;
  }
  .poem-line.visible {
    opacity: 1;
    transform: translateY(0);
  }
  .poem-line.highlight {
    color: var(--honey);
    font-weight: 700;
    font-size: 0.95rem;
    letter-spacing: 0.05em;
    margin-bottom: 1.6rem;
  }
  .poem-signature {
    margin-top: 2.5rem;
    font-family: 'Fraunces', serif;
    font-size: 1rem;
    color: var(--muted);
    font-style: italic;
    opacity: 0;
    transform: translateY(15px);
    transition: opacity 0.8s ease 0.5s, transform 0.8s ease 0.5s;
  }
  .poem-signature.visible {
    opacity: 1;
    transform: translateY(0);
  }
  .poem-signature::before {
    content: '— ';
  }

  /* Responsive */
  @media (max-width: 768px) {
    #gameArea { height: 260px; }
    .game-sprinkle { width: 34px; height: 34px; font-size: 1.15rem; }
    .poem-card { padding: 2.5rem 1.5rem; }
    .poem-line { font-size: 1rem; line-height: 1.8; }
    .poem-line.highlight { font-size: 0.9rem; }
    .game-wrap { padding: 1.5rem 1rem; }
  }
  @media (max-width: 480px) {
    #gameArea { height: 240px; }
    .game-sprinkle { width: 30px; height: 30px; font-size: 1rem; border-width: 2px; }
    .game-header { flex-direction: column; align-items: flex-start; }
    .poem-card { padding: 2rem 1.2rem; }
    .poem-line { font-size: 0.92rem; }
  }
</style>


<!-- ╔═══════════════════════════════════════════════════════════╗
     ║  BLOK 2 — HTML  (paste SEBELUM </footer>)                ║
     ╚═══════════════════════════════════════════════════════════╝ -->
<section class="closing-section" id="closing">
  <span class="sparkle" style="top:8%; left:6%;">✦</span>
  <span class="sparkle" style="top:18%; right:10%; animation-delay:1s;">✦</span>
  <span class="sparkle" style="bottom:10%; left:12%; animation-delay:2s;">✦</span>

  <div class="container">

    <!-- HEADER -->
    <div class="closing-head">
      <span class="kicker">Sebelum Pulang</span>
      <h2>Main Dulu, Renung Sejenak, Baru Pulang 💙</h2>
      <p>Terima kasih sudah mampir ke ruang kecilku. Sebelum pergi, coba main game mini ini dan baca kutipan para filsuf tentang ketenangan.</p>
    </div>

    <!-- GAME: TANGKAP SPRINKLE -->
    <div class="game-wrap">
      <div class="game-header">
        <div class="game-title">
          <i class="fas fa-cookie-bite"></i>
          Tangkap Sprinkle!
        </div>
        <div class="game-stats">
          <div class="game-stat">
            <i class="fas fa-star"></i> Skor: <span class="stat-value" id="gameScore">0</span>
          </div>
          <div class="game-stat">
            <i class="fas fa-clock"></i> Waktu: <span class="stat-value" id="gameTime">30</span>s
          </div>
          <div class="game-stat">
            <i class="fas fa-trophy"></i> Best: <span class="stat-value" id="gameBest">0</span>
          </div>
        </div>
      </div>

      <div id="gameArea">
        <!-- Overlay start -->
        <div class="game-overlay" id="gameStartOverlay">
          <h3><i class="fas fa-gamepad"></i> Cara Main</h3>
          <p>Ketuk sprinkle warna-warni yang jatuh dari atas selama 30 detik. Tiap sprinkle yang kena = +1 poin. Ayo kumpulkan sebanyak mungkin!</p>
          <button class="game-btn" onclick="startGame()">
            <i class="fas fa-play"></i> Mulai Main
          </button>
          <button class="game-reset" onclick="resetHighScore()">
            <i class="fas fa-redo"></i> Reset High Score
          </button>
        </div>

        <!-- Overlay game over -->
        <div class="game-overlay hidden" id="gameOverOverlay">
          <h3><i class="fas fa-star"></i> Selesai!</h3>
          <p id="gameOverText">Skor kamu: 0</p>
          <button class="game-btn sun" onclick="startGame()">
            <i class="fas fa-redo"></i> Main Lagi
          </button>
        </div>
      </div>
    </div>

    <!-- PUISI FILSUF -->
    <div class="poem-section">
      <div class="poem-card">
        <h3 class="poem-title">Ketenangan di Tengah Riuh Negeri</h3>

        <p class="poem-line">"Keheningan membawa kebenaran."</p>
        <p class="poem-line highlight">— Mahatma Gandhi</p>

        <p class="poem-line">Di negeri yang ramai oleh kabar dan gosip,</p>
        <p class="poem-line">hening jadi barang mahal yang jarang dibeli.</p>
        <p class="poem-line">Padahal di dalam diam, ada jawaban</p>
        <p class="poem-line">yang tak pernah bisa diucap oleh berita.</p>

        <p class="poem-line">"Jika kamu tenang, kamu hidup di masa sekarang."</p>
        <p class="poem-line highlight">— Lao Tzu</p>

        <p class="poem-line">Sementara layar terus menuntut kita</p>
        <p class="poem-line">tentang esok yang belum tentu datang,</p>
        <p class="poem-line">tentang harga yang naik dan janji yang turun —</p>
        <p class="poem-line">ketenangan hanya ada bagi yang berani berhenti.</p>

        <p class="poem-line">"Kedamaian adalah kemerdekaan dalam ketenangan."</p>
        <p class="poem-line highlight">— Marcus Tullius Cicero</p>

        <p class="poem-line">Merdeka bukan hanya soal bendera dan tanggal,</p>
        <p class="poem-line">tapi soal hati yang tak lagi gelisah</p>
        <p class="poem-line">saat melihat dunia berputar terlalu cepat —</p>
        <p class="poem-line">dan tetap bisa memilih untuk bernapas.</p>

        <p class="poem-line">"Tidak ada yang bisa memberimu kedamaian selain dirimu sendiri."</p>
        <p class="poem-line highlight">— Ralph Waldo Emerson</p>

        <p class="poem-line">Di tengah hiruk-pikuk kota yang tak pernah tidur,</p>
        <p class="poem-line">di antara dering notifikasi dan sorak berita,</p>
        <p class="poem-line">tak ada yang bisa menenangkan kita</p>
        <p class="poem-line">selain kita sendiri.</p>

        <p class="poem-signature">Ayu Cintya Nirmala</p>
      </div>
    </div>

  </div>
</section>


<!-- ╔═══════════════════════════════════════════════════════════╗
     ║  BLOK 3 — JAVASCRIPT  (paste SEBELUM </script> terakhir) ║
     ╚═══════════════════════════════════════════════════════════╝ -->
<script>
  /* ============ GAME: TANGKAP SPRINKLE ============ */
  var gameState = {
    running: false,
    score: 0,
    time: 30,
    timer: null,
    spawnInterval: null,
    spawnSpeed: 900
  };

  var GAME_BEST_KEY = 'ayu_game_best_v1';
  var sprinkleEmojis = ['🍩', '🧁', '🍰', '🍪', '🍬', '🍭', '🎨', '⭐', '✦', '🍜', '🐱', '💙'];
  var sprinkleColors = [
    'linear-gradient(135deg, #ffc93c, #ffe9a8)',
    'linear-gradient(135deg, #4a7fd4, #a8c8ff)',
    'linear-gradient(135deg, #ffb3c6, #ffd1dd)',
    'linear-gradient(135deg, #b8e6d9, #d5f2eb)',
    'linear-gradient(135deg, #a78bfa, #c4b5fd)'
  ];

  function updateGameBest() {
    var best = parseInt(localStorage.getItem(GAME_BEST_KEY) || '0', 10);
    var el = document.getElementById('gameBest');
    if (el) el.textContent = best;
    return best;
  }

  function saveGameBest(score) {
    var best = parseInt(localStorage.getItem(GAME_BEST_KEY) || '0', 10);
    if (score > best) {
      localStorage.setItem(GAME_BEST_KEY, String(score));
      return true;
    }
    return false;
  }

  function resetHighScore() {
    if (confirm('Yakin mau reset high score?')) {
      localStorage.removeItem(GAME_BEST_KEY);
      updateGameBest();
      var el = document.getElementById('gameBest');
      if (el) el.textContent = '0';
    }
  }

  function startGame() {
    var area = document.getElementById('gameArea');
    var startOverlay = document.getElementById('gameStartOverlay');
    var overOverlay = document.getElementById('gameOverOverlay');
    if (!area) return;

    var old = area.querySelectorAll('.game-sprinkle, .score-pop');
    old.forEach(function(s) { s.remove(); });

    gameState.running = true;
    gameState.score = 0;
    gameState.time = 30;
    gameState.spawnSpeed = 900;

    document.getElementById('gameScore').textContent = '0';
    document.getElementById('gameTime').textContent = '30';

    if (startOverlay) startOverlay.classList.add('hidden');
    if (overOverlay) overOverlay.classList.add('hidden');

    gameState.timer = setInterval(function() {
      gameState.time--;
      var timeEl = document.getElementById('gameTime');
      if (timeEl) timeEl.textContent = gameState.time;

      if (gameState.time === 22 || gameState.time === 14 || gameState.time === 6) {
        gameState.spawnSpeed = Math.max(400, gameState.spawnSpeed - 180);
        clearInterval(gameState.spawnInterval);
        gameState.spawnInterval = setInterval(spawnGameSprinkle, gameState.spawnSpeed);
      }

      if (gameState.time <= 0) {
        endGame();
      }
    }, 1000);

    gameState.spawnInterval = setInterval(spawnGameSprinkle, gameState.spawnSpeed);
    spawnGameSprinkle();
  }

  function spawnGameSprinkle() {
    if (!gameState.running) return;
    var area = document.getElementById('gameArea');
    if (!area) return;

    var sprink = document.createElement('div');
    sprink.className = 'game-sprinkle';
    var emoji = sprinkleEmojis[Math.floor(Math.random() * sprinkleEmojis.length)];
    var color = sprinkleColors[Math.floor(Math.random() * sprinkleColors.length)];
    sprink.textContent = emoji;
    sprink.style.background = color;
    sprink.style.left = (Math.random() * 85 + 2) + '%';

    var fallDuration = 2.2 + Math.random() * 1.3;
    sprink.style.animationDuration = fallDuration + 's';

    sprink.addEventListener('click', function(e) {
      e.stopPropagation();
      popSprinkle(sprink);
    });
    sprink.addEventListener('touchstart', function(e) {
      e.preventDefault();
      e.stopPropagation();
      popSprinkle(sprink);
    }, { passive: false });

    area.appendChild(sprink);

    setTimeout(function() {
      if (sprink.parentNode) sprink.remove();
    }, fallDuration * 1000 + 100);
  }

  function popSprinkle(el) {
    if (!gameState.running || el.classList.contains('popped')) return;
    el.classList.add('popped');
    gameState.score++;
    document.getElementById('gameScore').textContent = gameState.score;

    var rect = el.getBoundingClientRect();
    var area = document.getElementById('gameArea');
    var areaRect = area.getBoundingClientRect();
    var pop = document.createElement('div');
    pop.className = 'score-pop';
    pop.textContent = '+1';
    pop.style.left = (rect.left - areaRect.left) + 'px';
    pop.style.top = (rect.top - areaRect.top) + 'px';
    area.appendChild(pop);
    setTimeout(function() { if (pop.parentNode) pop.remove(); }, 700);

    setTimeout(function() { if (el.parentNode) el.remove(); }, 350);
  }

  function endGame() {
    gameState.running = false;
    clearInterval(gameState.timer);
    clearInterval(gameState.spawnInterval);

    var isNewBest = saveGameBest(gameState.score);
    updateGameBest();

    var overOverlay = document.getElementById('gameOverOverlay');
    var overText = document.getElementById('gameOverText');
    if (overText) {
      overText.innerHTML = 'Skor kamu: <strong>' + gameState.score + '</strong>' +
                           (isNewBest ? '<br><span style="color: var(--honey); font-weight: 700;">🎉 High Score Baru!</span>' : '');
    }
    if (overOverlay) overOverlay.classList.remove('hidden');

    var area = document.getElementById('gameArea');
    if (area) {
      var remaining = area.querySelectorAll('.game-sprinkle');
      remaining.forEach(function(s) { s.remove(); });
    }
  }

  /* ============ PUISI — FADE-IN SAAT SCROLL ============ */
  function setupPoemReveal() {
    var lines = document.querySelectorAll('.poem-line, .poem-signature');
    if (!lines.length) return;

    if (!('IntersectionObserver' in window)) {
      lines.forEach(function(l) { l.classList.add('visible'); });
      return;
    }

    var observer = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) {
          var el = entry.target;
          var allLines = Array.prototype.slice.call(document.querySelectorAll('.poem-line, .poem-signature'));
          var idx = allLines.indexOf(el);
          var delay = Math.max(0, idx * 120);
          setTimeout(function() {
            el.classList.add('visible');
          }, delay);
          observer.unobserve(el);
        }
      });
    }, { threshold: 0.2, rootMargin: '0px 0px -50px 0px' });

    lines.forEach(function(l) { observer.observe(l); });
  }

  document.addEventListener('DOMContentLoaded', function() {
    updateGameBest();
    setupPoemReveal();
  });
</script>
