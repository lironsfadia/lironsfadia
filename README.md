<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 400 200">
  <defs>
    <linearGradient id="bg-gradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#120c6e;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#5e2d79;stop-opacity:1" />
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3.5" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  
  <rect width="100%" height="100%" fill="url(#bg-gradient)"/>
  
  <g transform="translate(200 100)">
    <path d="M-150 70 L-120 70 L-90 40 L-60 70 L150 70" stroke="#ff00ff" stroke-width="2" fill="none">
      <animate attributeName="d" dur="5s" repeatCount="indefinite"
        values="
          M-150 70 L-120 70 L-90 40 L-60 70 L150 70;
          M-150 65 L-120 65 L-90 35 L-60 65 L150 65;
          M-150 70 L-120 70 L-90 40 L-60 70 L150 70"
      />
    </path>
  </g>

  <text x="50%" y="50%" text-anchor="middle" font-family="Arial Black, sans-serif" font-size="40" fill="#00ffff" filter="url(#glow)">
    It's my GitHub
    <animate attributeName="opacity" values="1;0.7;1" dur="2s" repeatCount="indefinite"/>
  </text>

  <g id="stars">
    <circle cx="30" cy="30" r="2" fill="#ffffff">
      <animate attributeName="opacity" values="0;1;0" dur="3s" repeatCount="indefinite"/>
    </circle>
    <circle cx="350" cy="50" r="1" fill="#ffffff">
      <animate attributeName="opacity" values="0;1;0" dur="4s" repeatCount="indefinite"/>
    </circle>
    <circle cx="280" cy="120" r="1.5" fill="#ffffff">
      <animate attributeName="opacity" values="0;1;0" dur="2.5s" repeatCount="indefinite"/>
    </circle>
  </g>
</svg>
