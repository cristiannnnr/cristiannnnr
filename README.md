<div align="center">

# 宇智波 オビト

<br/>

<svg viewBox="0 0 300 300" width="260" height="260" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <radialGradient id="irisGrad" cx="45%" cy="45%" r="55%">
      <stop offset="0%" stop-color="#ff4444"/>
      <stop offset="60%" stop-color="#cc0000"/>
      <stop offset="100%" stop-color="#7a0000"/>
    </radialGradient>
    <radialGradient id="bgGrad" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#1a0505"/>
      <stop offset="100%" stop-color="#050000"/>
    </radialGradient>
    <radialGradient id="pupilGrad" cx="40%" cy="35%" r="60%">
      <stop offset="0%" stop-color="#1a0000"/>
      <stop offset="100%" stop-color="#000000"/>
    </radialGradient>
    <filter id="glow" x="-40%" y="-40%" width="180%" height="180%">
      <feGaussianBlur in="SourceGraphic" stdDeviation="5" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <filter id="softGlow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur in="SourceGraphic" stdDeviation="2.5" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- Dark background -->
  <rect width="300" height="300" fill="url(#bgGrad)"/>

  <!-- Outer aura pulse (slow) -->
  <circle cx="150" cy="150" r="130" fill="none" stroke="#880000" stroke-width="1.5">
    <animate attributeName="opacity" values="0.05;0.45;0.05" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="r" values="124;134;124" dur="3s" repeatCount="indefinite"/>
  </circle>

  <!-- Second aura ring (offset) -->
  <circle cx="150" cy="150" r="116" fill="none" stroke="#cc0000" stroke-width="1">
    <animate attributeName="opacity" values="0.35;0.05;0.35" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="r" values="111;120;111" dur="3s" repeatCount="indefinite"/>
  </circle>

  <!-- Counter-rotating outer decoration ring -->
  <g>
    <animateTransform attributeName="transform" type="rotate"
      from="0 150 150" to="-360 150 150"
      dur="12s" repeatCount="indefinite"/>
    <circle cx="150" cy="150" r="101" fill="none" stroke="#550000" stroke-width="1" stroke-dasharray="8 14"/>
  </g>

  <!-- Sclera (white of eye) -->
  <circle cx="150" cy="150" r="93" fill="#ececec" filter="url(#softGlow)"/>

  <!-- Red iris -->
  <circle cx="150" cy="150" r="73" fill="url(#irisGrad)"/>

  <!-- SPINNING GROUP: ring + 3 tomoe -->
  <g>
    <animateTransform attributeName="transform" type="rotate"
      from="0 150 150" to="360 150 150"
      dur="5s" repeatCount="indefinite"/>

    <!-- Inner ring at radius 47 -->
    <circle cx="150" cy="150" r="47" fill="none" stroke="#5a0000" stroke-width="2.5"/>

    <!-- Tomoe 1: head at top (150, 103) -->
    <circle cx="150" cy="103" r="11" fill="#0d0000" filter="url(#glow)"/>
    <path d="M150,103 Q180,118 164,143" stroke="#0d0000" stroke-width="9" fill="none" stroke-linecap="round"/>

    <!-- Tomoe 2: head at bottom-right (191, 173) -->
    <!-- 150 + 47*cos(30°)=191, 150 + 47*sin(30°)=173.5 -->
    <circle cx="191" cy="174" r="11" fill="#0d0000" filter="url(#glow)"/>
    <path d="M191,174 Q177,201 152,196" stroke="#0d0000" stroke-width="9" fill="none" stroke-linecap="round"/>

    <!-- Tomoe 3: head at bottom-left (109, 173) -->
    <!-- 150 + 47*cos(150°)=109, 150 + 47*sin(150°)=173.5 -->
    <circle cx="109" cy="174" r="11" fill="#0d0000" filter="url(#glow)"/>
    <path d="M109,174 Q123,201 148,196" stroke="#0d0000" stroke-width="9" fill="none" stroke-linecap="round"/>
  </g>

  <!-- Pupil -->
  <circle cx="150" cy="150" r="25" fill="url(#pupilGrad)"/>

  <!-- Pupil glow core -->
  <circle cx="150" cy="150" r="18" fill="#080000">
    <animate attributeName="opacity" values="0.7;1;0.7" dur="3s" repeatCount="indefinite"/>
  </circle>

  <!-- Subtle corneal highlight -->
  <ellipse cx="158" cy="141" rx="9" ry="5.5" fill="rgba(255,255,255,0.13)" transform="rotate(-30 158 141)"/>
</svg>

<br/>

---

*El mundo del genjutsu siempre estuvo en sus ojos.*

</div>
