<svg width="1000" height="300" viewBox="0 0 1000 300" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0d0d1a"/>
      <stop offset="55%" stop-color="#1a0b2e"/>
      <stop offset="100%" stop-color="#2a0a3d"/>
    </linearGradient>
    <linearGradient id="neon" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#7c3aed"/>
      <stop offset="100%" stop-color="#ec4899"/>
    </linearGradient>
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <pattern id="scanlines" width="4" height="4" patternUnits="userSpaceOnUse">
      <rect width="4" height="2" fill="black" opacity="0.15"/>
    </pattern>
  </defs>

  <!-- background -->
  <rect width="1000" height="300" fill="url(#bg)"/>

  <!-- floating pixel stars -->
  <g fill="#ec4899">
    <rect x="60" y="40" width="4" height="4">
      <animate attributeName="opacity" values="0.2;1;0.2" dur="2.4s" repeatCount="indefinite"/>
    </rect>
    <rect x="920" y="60" width="4" height="4">
      <animate attributeName="opacity" values="1;0.2;1" dur="1.8s" repeatCount="indefinite"/>
    </rect>
    <rect x="150" y="230" width="4" height="4" fill="#7c3aed">
      <animate attributeName="opacity" values="0.2;1;0.2" dur="3s" repeatCount="indefinite"/>
    </rect>
    <rect x="850" y="220" width="4" height="4" fill="#7c3aed">
      <animate attributeName="opacity" values="1;0.3;1" dur="2.2s" repeatCount="indefinite"/>
    </rect>
    <rect x="500" y="30" width="3" height="3">
      <animate attributeName="opacity" values="0.3;1;0.3" dur="1.6s" repeatCount="indefinite"/>
    </rect>
  </g>

  <!-- title -->
  <text x="500" y="95" font-family="'Courier New', monospace" font-size="42" font-weight="bold"
        text-anchor="middle" fill="url(#neon)" filter="url(#glow)">SHREYA.EXE</text>
  <text x="500" y="130" font-family="'Courier New', monospace" font-size="16"
        text-anchor="middle" fill="#c9b6ea" letter-spacing="2">DATA ENGINEER &#8226; FINAL YEAR &#8226; LVL 4</text>

  <!-- blinking press start -->
  <text x="500" y="165" font-family="'Courier New', monospace" font-size="15"
        text-anchor="middle" fill="#ec4899" letter-spacing="3">
    PRESS START TO CONTINUE
    <animate attributeName="opacity" values="1;0;1" dur="1.2s" repeatCount="indefinite"/>
  </text>

  <!-- XP bar -->
  <rect x="300" y="185" width="400" height="18" rx="4" fill="#1e1e2e" stroke="#7c3aed" stroke-width="2"/>
  <rect x="303" y="188" width="0" height="12" rx="2" fill="url(#neon)">
    <animate attributeName="width" values="0;394" dur="3s" fill="freeze" begin="0.3s"/>
  </rect>
  <text x="500" y="222" font-family="'Courier New', monospace" font-size="12" text-anchor="middle" fill="#8a7ba8">
    XP: LOADING SKILLS... [PYTHON] [SQL] [AIRFLOW] [AWS]
  </text>

  <!-- pixel character walking -->
  <g transform="translate(100,240)">
    <g>
      <animateTransform attributeName="transform" type="translate"
        values="0,0; 780,0; 780,0; 0,0" keyTimes="0;0.45;0.55;1" dur="9s" repeatCount="indefinite"/>
      <!-- body -->
      <rect x="0" y="0" width="16" height="16" fill="#ec4899"/>
      <rect x="4" y="16" width="8" height="10" fill="#7c3aed"/>
      <!-- legs animation -->
      <rect x="2" y="26" width="4" height="6" fill="#c9b6ea">
        <animate attributeName="height" values="6;2;6" dur="0.4s" repeatCount="indefinite"/>
      </rect>
      <rect x="10" y="26" width="4" height="6" fill="#c9b6ea">
        <animate attributeName="height" values="2;6;2" dur="0.4s" repeatCount="indefinite"/>
      </rect>
    </g>
  </g>

  <!-- ground line -->
  <line x1="0" y1="272" x2="1000" y2="272" stroke="#7c3aed" stroke-width="2" opacity="0.5"/>

  <!-- scanline overlay -->
  <rect width="1000" height="300" fill="url(#scanlines)"/>

  <!-- border frame -->
  <rect x="4" y="4" width="992" height="292" fill="none" stroke="#7c3aed" stroke-width="2" opacity="0.6"/>
</svg>
