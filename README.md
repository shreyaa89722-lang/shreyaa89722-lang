<svg width="1000" height="280" viewBox="0 0 1000 280" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0a0a0f"/>
      <stop offset="100%" stop-color="#150a2e"/>
    </linearGradient>
    <linearGradient id="neonGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#7c3aed"/>
      <stop offset="100%" stop-color="#ec4899"/>
    </linearGradient>
    <filter id="glow" x="-60%" y="-60%" width="220%" height="220%">
      <feGaussianBlur stdDeviation="3.5" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <pattern id="grid" width="30" height="30" patternUnits="userSpaceOnUse">
      <path d="M 30 0 L 0 0 0 30" fill="none" stroke="#7c3aed" stroke-width="0.4" opacity="0.25"/>
    </pattern>
  </defs>

  <!-- background -->
  <rect width="1000" height="280" fill="url(#bgGrad)"/>
  <rect width="1000" height="280" fill="url(#grid)"/>

  <!-- HUD corner brackets -->
  <g stroke="#ec4899" stroke-width="3" fill="none" opacity="0.9">
    <path d="M20,20 L20,55 M20,20 L55,20"/>
    <path d="M980,20 L980,55 M980,20 L945,20"/>
    <path d="M20,260 L20,225 M20,260 L55,260"/>
    <path d="M980,260 L980,225 M980,260 L945,260"/>
  </g>

  <!-- ONLINE status -->
  <circle cx="45" cy="42" r="5" fill="#22ff88">
    <animate attributeName="opacity" values="1;0.3;1" dur="1.4s" repeatCount="indefinite"/>
  </circle>
  <text x="58" y="46" font-family="'Courier New', monospace" font-size="12" fill="#22ff88" letter-spacing="1">ONLINE</text>

  <!-- controller icon (top right) -->
  <g transform="translate(910,28)" fill="none" stroke="url(#neonGrad)" stroke-width="2.5" filter="url(#glow)">
    <path d="M5,15 Q5,2 20,2 L45,2 Q60,2 60,15 L60,20 Q60,30 50,30 Q45,30 42,25 L38,20 L27,20 L23,25 Q20,30 15,30 Q5,30 5,20 Z"/>
    <line x1="16" y1="10" x2="16" y2="18"/>
    <line x1="12" y1="14" x2="20" y2="14"/>
    <circle cx="48" cy="10" r="1.8" fill="#ec4899" stroke="none"/>
    <circle cx="53" cy="15" r="1.8" fill="#ec4899" stroke="none"/>
  </g>

  <!-- title -->
  <text x="500" y="90" font-family="'Courier New', monospace" font-size="46" font-weight="bold"
        text-anchor="middle" fill="url(#neonGrad)" filter="url(#glow)" letter-spacing="4">SHREYA</text>
  <text x="500" y="118" font-family="'Courier New', monospace" font-size="15"
        text-anchor="middle" fill="#c9b6ea" letter-spacing="3">DATA ENGINEER // FINAL YEAR // MALNAD COLLEGE</text>

  <!-- divider -->
  <line x1="250" y1="135" x2="750" y2="135" stroke="#7c3aed" stroke-width="1" opacity="0.5"/>

  <!-- stat bars -->
  <g font-family="'Courier New', monospace" font-size="13" fill="#c9b6ea">
    <!-- PYTHON -->
    <text x="250" y="160">PYTHON</text>
    <rect x="350" y="149" width="330" height="14" rx="3" fill="#1e1e2e" stroke="#7c3aed" stroke-width="1.5"/>
    <rect x="353" y="152" width="0" height="8" rx="2" fill="url(#neonGrad)">
      <animate attributeName="width" values="0;300" dur="2s" fill="freeze" begin="0.2s"/>
    </rect>
    <text x="695" y="160" fill="#ec4899">90%</text>

    <!-- SQL -->
    <text x="250" y="185">SQL</text>
    <rect x="350" y="174" width="330" height="14" rx="3" fill="#1e1e2e" stroke="#7c3aed" stroke-width="1.5"/>
    <rect x="353" y="177" width="0" height="8" rx="2" fill="url(#neonGrad)">
      <animate attributeName="width" values="0;230" dur="2s" fill="freeze" begin="0.4s"/>
    </rect>
    <text x="695" y="185" fill="#ec4899">70%</text>

    <!-- AIRFLOW -->
    <text x="250" y="210">AIRFLOW</text>
    <rect x="350" y="199" width="330" height="14" rx="3" fill="#1e1e2e" stroke="#7c3aed" stroke-width="1.5"/>
    <rect x="353" y="202" width="0" height="8" rx="2" fill="url(#neonGrad)">
      <animate attributeName="width" values="0;165" dur="2s" fill="freeze" begin="0.6s"/>
    </rect>
    <text x="695" y="210" fill="#ec4899">50%</text>

    <!-- AWS -->
    <text x="250" y="235">AWS</text>
    <rect x="350" y="224" width="330" height="14" rx="3" fill="#1e1e2e" stroke="#7c3aed" stroke-width="1.5"/>
    <rect x="353" y="227" width="0" height="8" rx="2" fill="url(#neonGrad)">
      <animate attributeName="width" values="0;100" dur="2s" fill="freeze" begin="0.8s"/>
    </rect>
    <text x="695" y="235" fill="#ec4899">30%</text>
  </g>

  <!-- scanning sweep line -->
  <rect x="0" y="0" width="4" height="280" fill="#ec4899" opacity="0.5">
    <animate attributeName="x" values="0;996;0" dur="6s" repeatCount="indefinite"/>
  </rect>
</svg>
