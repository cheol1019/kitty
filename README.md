<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <title>🎀 시험 화이팅팅팅팅! 💯 헬로키티 특급 응원 🌟</title>
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Canvas Confetti -->
  <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <!-- Google Fonts: Jua & Gaegu -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Gaegu:wght@700&family=Jua&family=Noto+Sans+KR:wght@700;900&display=swap" rel="stylesheet">

  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            jua: ['"Jua"', 'sans-serif'],
            gaegu: ['"Gaegu"', 'cursive'],
            sans: ['"Noto Sans KR"', 'sans-serif'],
          },
          colors: {
            sanrio: {
              red: '#e6002b',
              crimson: '#c40024',
              softPink: '#ffe8f0',
              pinkGingham: '#ffccd9',
              pastelPink: '#ff7597',
              yellowNose: '#ffcc00',
              blueOveralls: '#1a6fba',
              darkLine: '#1e1b18'
            }
          },
          animation: {
            'text-bounce': 'titleBounce 1s cubic-bezier(0.28, 0.84, 0.42, 1) infinite alternate',
            'kitty-wiggle': 'kittyFloat 1.8s ease-in-out infinite alternate',
            'kitty-jump': 'kittyJump 0.45s ease-in-out 2',
            'float-item': 'floatingItem 2.2s ease-in-out infinite alternate',
            'spin-sparkle': 'spin 10s linear infinite',
            'pulse-glow': 'pulseGlow 1.4s ease-in-out infinite alternate',
          },
          keyframes: {
            titleBounce: {
              '0%': { transform: 'scale(0.97) translateY(0)' },
              '100%': { transform: 'scale(1.05) translateY(-8px)' },
            },
            kittyFloat: {
              '0%': { transform: 'translateY(0px) rotate(-1deg)' },
              '100%': { transform: 'translateY(-12px) rotate(1.5deg)' },
            },
            kittyJump: {
              '0%, 100%': { transform: 'translateY(0) scale(1)' },
              '45%': { transform: 'translateY(-32px) scale(1.12) rotate(3deg)' },
            },
            floatingItem: {
              '0%': { transform: 'translateY(0) rotate(0deg) scale(0.95)', opacity: '0.85' },
              '100%': { transform: 'translateY(-14px) rotate(15deg) scale(1.1)', opacity: '1' },
            },
            pulseGlow: {
              '0%': { transform: 'scale(1)', opacity: '0.5' },
              '100%': { transform: 'scale(1.15)', opacity: '0.9' },
            }
          }
        }
      }
    }
  </script>

  <style>
    /* 정통 산리오 딸기우유 깅엄 체크 배경 */
    body {
      background-color: #fff2f6;
      background-image: 
        linear-gradient(45deg, rgba(255, 175, 195, 0.28) 25%, transparent 25%), 
        linear-gradient(-45deg, rgba(255, 175, 195, 0.28) 25%, transparent 25%), 
        linear-gradient(45deg, transparent 75%, rgba(255, 175, 195, 0.28) 75%), 
        linear-gradient(-45deg, transparent 75%, rgba(255, 175, 195, 0.28) 75%);
      background-size: 28px 28px;
      touch-action: manipulation;
      user-select: none;
      -webkit-user-select: none;
      overflow: hidden;
      height: 100vh;
      height: 100dvh;
    }

    /* 거대 볼드 응원 타이포그래피 (3중 입체 섀도우) */
    .sanrio-title {
      color: #e6002b;
      text-shadow: 
        4px 4px 0 #ffffff,
        -4px -4px 0 #ffffff,
        4px -4px 0 #ffffff,
        -4px 4px 0 #ffffff,
        0 8px 0 #ff7597,
        0 14px 20px rgba(230, 0, 43, 0.35);
      letter-spacing: -0.01em;
    }

    /* 탭할 때 폭발하듯 솟아오르는 이모지 파티클 */
    .tap-pop-particle {
      position: absolute;
      pointer-events: none;
      font-size: 2.2rem;
      font-weight: 900;
      animation: popFly 0.9s cubic-bezier(0.18, 0.89, 0.32, 1.28) forwards;
      z-index: 999;
      filter: drop-shadow(0 4px 8px rgba(0,0,0,0.18));
      white-space: nowrap;
    }
    @keyframes popFly {
      0% {
        opacity: 1;
        transform: translate(-50%, -50%) scale(0.3) rotate(0deg);
      }
      50% {
        transform: translate(-50%, -90px) scale(1.4) rotate(15deg);
      }
      100% {
        opacity: 0;
        transform: translate(-50%, -170px) scale(1.8) rotate(-20deg);
      }
    }

    /* 말풍선 디테일 */
    .kitty-bubble {
      filter: drop-shadow(0 8px 18px rgba(255, 80, 120, 0.22));
    }
    .kitty-bubble::after {
      content: '';
      position: absolute;
      bottom: -11px;
      left: 50%;
      transform: translateX(-50%);
      border-width: 11px 11px 0 11px;
      border-style: solid;
      border-color: #ffffff transparent transparent transparent;
    }
    .kitty-bubble::before {
      content: '';
      position: absolute;
      bottom: -14px;
      left: 50%;
      transform: translateX(-50%);
      border-width: 14px 14px 0 14px;
      border-style: solid;
      border-color: #ff99b3 transparent transparent transparent;
    }

    /* 부드러운 썬샤인 원형 그라데이션 */
    .halo-shine {
      background: radial-gradient(circle, rgba(255, 255, 255, 0.95) 0%, rgba(255, 218, 230, 0.6) 45%, transparent 70%);
    }
  </style>
</head>
<body class="w-full h-full relative flex flex-col justify-between items-center p-3 sm:p-5 overflow-hidden">

  <!-- 후광 글로우 레이어 -->
  <div class="halo-shine absolute inset-0 pointer-events-none z-0"></div>

  <!-- 떠다니는 귀여운 시험 합격 데코레이션 아이콘들 -->
  <div class="absolute inset-0 pointer-events-none overflow-hidden z-0">
    <span class="absolute top-[8%] left-[7%] text-3xl sm:text-4xl animate-float-item">✨</span>
    <span class="absolute top-[14%] right-[8%] text-3xl sm:text-4xl animate-float-item" style="animation-delay: 0.7s;">🌟</span>
    <span class="absolute bottom-[20%] left-[8%] text-4xl sm:text-5xl animate-float-item" style="animation-delay: 1.2s;">💯</span>
    <span class="absolute bottom-[22%] right-[7%] text-4xl sm:text-5xl animate-float-item" style="animation-delay: 0.5s;">🅰️➕</span>
    <span class="absolute top-[38%] left-[3%] text-3xl animate-float-item" style="animation-delay: 1.6s;">✏️</span>
    <span class="absolute top-[42%] right-[4%] text-3xl animate-float-item" style="animation-delay: 0.9s;">🍀</span>
    <span class="absolute top-[72%] left-[12%] text-2xl animate-float-item" style="animation-delay: 0.3s;">🎯</span>
    <span class="absolute top-[68%] right-[12%] text-2xl animate-float-item" style="animation-delay: 1.4s;">🎀</span>
  </div>

  <!-- [상단 헤더]: BGM 제어 및 키티 의상/모드 토글 -->
  <header class="w-full max-w-md mx-auto flex justify-between items-center z-30 pt-1">
    <!-- 옷 색상 토글 (클래식 블루 멜빵 ↔ 핑크 큐티 드레스) -->
    <button id="outfitBtn" class="px-3.5 py-1.5 rounded-full bg-white/95 border-2 border-pink-300 text-sanrio-crimson shadow-sm active:scale-95 transition flex items-center gap-1.5 backdrop-blur-sm font-jua text-xs sm:text-sm cursor-pointer">
      <span class="text-base">👗</span>
      <span id="outfitLabel">클래식 멜빵</span>
    </button>

    <!-- 배경 멜로디 On/Off -->
    <button id="bgmToggleBtn" class="px-3.5 py-1.5 rounded-full bg-white/95 border-2 border-pink-300 text-sanrio-crimson shadow-sm active:scale-95 transition flex items-center gap-1.5 backdrop-blur-sm font-jua text-xs sm:text-sm cursor-pointer">
      <i id="bgmIcon" class="fa-solid fa-volume-high text-sanrio-red animate-pulse"></i>
      <span id="bgmLabel">키티 응원곡 ON</span>
    </button>
  </header>


  <!-- [중앙 메인 영역]: 큰 시험 화이팅 문구 + 정통 산리오 비율 헬로키티 -->
  <main class="w-full max-w-lg my-auto flex flex-col items-center justify-center text-center z-20 relative select-none">
    
    <!-- 1. 키티 머리 위 거대 화이팅 타이틀 구역 -->
    <div class="mb-2 sm:mb-3 animate-text-bounce cursor-pointer" onclick="triggerMegaConfetti(event)">
      <!-- 상단 리본 뱃지 -->
      <div class="inline-flex items-center gap-1.5 px-4 py-1 rounded-full bg-white border-2 border-pink-300 text-sanrio-crimson font-jua text-xs sm:text-sm shadow-md mb-2">
        <span class="text-sanrio-red text-base">🎀</span>
        <span>정답만 쏙쏙! 백점 만점의 기운</span>
        <span class="text-sanrio-red text-base">🎀</span>
      </div>

      <!-- 메인 메가 텍스트 -->
      <h1 class="sanrio-title font-jua text-5xl sm:text-6xl md:text-7xl font-black leading-none drop-shadow-sm">
        시험 화이팅! 💯✨
      </h1>

      <!-- 서브 슬로건 -->
      <p class="font-jua text-sanrio-crimson text-base sm:text-xl mt-2 tracking-wide">
        "너는 무조건 잘 볼 거야! A+ 가자! 💖"
      </p>
    </div>

    <!-- 2. 동적 응원 말풍선 (터치 시 산리오 명언 및 특급 격려문구 롤링) -->
    <div id="speechBubble" class="kitty-bubble relative bg-white border-2 border-pink-300 px-5 py-2.5 rounded-2xl shadow-lg mb-2 max-w-xs transition-all duration-300">
      <p class="font-jua text-sanrio-crimson text-xs sm:text-sm flex items-center justify-center gap-1.5">
        <span class="text-base">🌸</span>
        <span id="bubbleText">너의 노력을 믿어! 넌 반드시 해내!</span>
        <span class="text-base">💖</span>
      </p>
    </div>

    <!-- 3. 산리오 공식 정품 비율을 완벽 구현한 헬로키티 캐릭터 -->
    <div id="kittyContainer" class="relative cursor-pointer group py-1" onclick="onKittyClick(event)">
      
      <!-- 키티 뒤 은은한 핑크 펄스 링 -->
      <div class="absolute -inset-5 bg-gradient-to-tr from-pink-300 via-rose-200 to-amber-100 rounded-full blur-xl opacity-70 group-hover:opacity-100 transition duration-500 animate-pulse-glow"></div>

      <!-- 정통 Sanrio 헬로키티 공식 벡터 그래픽 -->
      <!-- 
        공식 비율 체크포인트 준수:
        1. 가로로 둥글넙적한 얼굴 타원형 (가로:세로 약 1.3:1 비율)
        2. 입 절대 없음 (No mouth)
        3. 눈: 낮고 멀리 떨어진 짙은 타원형 2개
        4. 코: 두 눈 사이 하단과 동일 수평선에 위치한 밝은 샛노란 타원형
        5. 수염: 양 볼에 자연스러운 각도의 단정한 3줄씩
        6. 리본: 왼쪽 귀 앞쪽에 둥근 중앙 매듭과 빵빵한 두 날개의 선명한 레드 리본
        7. 클래식 오버롤 & 치어리딩 황금 응원봉 + 100점 시험지
      -->
      <svg id="kittySvg" viewBox="0 0 340 330" class="w-64 h-64 sm:w-76 sm:h-76 md:w-84 md:h-84 drop-shadow-2xl relative z-10 transition-transform animate-kitty-wiggle">
        
        <!-- 바닥 그림자 -->
        <ellipse cx="170" cy="316" rx="90" ry="12" fill="rgba(230, 0, 43, 0.22)" />

        <!-- [몸통 & 클래식 옷] -->
        <g id="kitty-outfit">
          <!-- 빨간 티셔츠 팔뚝 / 어깨 베이스 -->
          <path d="M 120 220 L 220 220 L 210 260 L 130 260 Z" fill="#e6002b" stroke="#1e1b18" stroke-width="6.5" stroke-linejoin="round"/>
          
          <!-- 오버롤 바지/멜빵 몸체 (클래식 블루 / 핑크 전환 가능) -->
          <path id="overallsBase" d="M 125 230 C 115 280, 110 300, 135 305 C 150 307, 160 300, 170 300 C 180 300, 190 307, 205 305 C 230 300, 225 280, 215 230 Z" 
                fill="#1a6fba" stroke="#1e1b18" stroke-width="7" stroke-linejoin="round"/>

          <!-- 멜빵 어깨 끈 (좌 / 우) -->
          <path id="strapLeft" d="M 132 225 L 142 270" stroke="#1a6fba" stroke-width="15" stroke-linecap="round"/>
          <path d="M 132 225 L 142 270" stroke="#1e1b18" stroke-width="3" stroke-linecap="round" fill="none" class="opacity-30"/>
          <path id="strapRight" d="M 208 225 L 198 270" stroke="#1a6fba" stroke-width="15" stroke-linecap="round"/>
          <path d="M 208 225 L 198 270" stroke="#1e1b18" stroke-width="3" stroke-linecap="round" fill="none" class="opacity-30"/>

          <!-- 멜빵 단추 (노란색) -->
          <circle cx="142" cy="265" r="5" fill="#ffcc00" stroke="#1e1b18" stroke-width="3"/>
          <circle cx="198" cy="265" r="5" fill="#ffcc00" stroke="#1e1b18" stroke-width="3"/>

          <!-- 앙증맞은 두 발 (흰색 타원) -->
          <ellipse cx="145" cy="308" rx="19" ry="12" fill="#ffffff" stroke="#1e1b18" stroke-width="6.5"/>
          <ellipse cx="195" cy="308" rx="19" ry="12" fill="#ffffff" stroke="#1e1b18" stroke-width="6.5"/>
        </g>

        <!-- [왼손: 100점 대박 시험지를 꼭 쥐고 있는 손] -->
        <g id="left-hand-exam" transform="translate(70, 210)">
          <!-- 시험지 종이 -->
          <g transform="rotate(-18) translate(-10, 0)">
            <rect x="0" y="0" width="48" height="60" rx="4" fill="#ffffff" stroke="#1e1b18" stroke-width="4.5" />
            <!-- 시험지 위 100점 동그라미 표시 -->
            <text x="24" y="28" font-family="'Jua', sans-serif" font-size="22" font-weight="900" fill="#e6002b" text-anchor="middle" dominant-baseline="middle">100</text>
            <circle cx="24" cy="27" r="18" fill="none" stroke="#e6002b" stroke-width="3.5" stroke-dasharray="85 10"/>
            <!-- 밑줄 줄글 -->
            <line x1="8" y1="44" x2="40" y2="44" stroke="#ffccd9" stroke-width="3" stroke-linecap="round"/>
            <line x1="8" y1="51" x2="32" y2="51" stroke="#ffccd9" stroke-width="3" stroke-linecap="round"/>
          </g>
          <!-- 왼손 발 (흰색 타원) -->
          <ellipse cx="38" cy="30" rx="16" ry="14" fill="#ffffff" stroke="#1e1b18" stroke-width="6.5"/>
        </g>

        <!-- [오른손: 황금빛 행운의 응원 폼폼 / 별봉을 들고 파이팅!] -->
        <g id="right-hand-cheer" transform="translate(230, 200)">
          <!-- 위로 번쩍 든 오른손 팔 -->
          <path d="M 0 35 C 16 20, 28 5, 34 -15 C 38 -5, 20 45, 5 45 Z" fill="#ffffff" stroke="#1e1b18" stroke-width="6.5" stroke-linejoin="round"/>
          <ellipse cx="32" cy="-14" rx="15" ry="14" fill="#ffffff" stroke="#1e1b18" stroke-width="6.5"/>
          
          <!-- 손에 든 황금빛 응원 별봉 (합격 요술봉) -->
          <g transform="translate(36, -20) rotate(15)">
            <line x1="0" y1="0" x2="16" y2="-38" stroke="#ffaa00" stroke-width="6" stroke-linecap="round"/>
            <!-- 반짝이는 황금 별 -->
            <polygon points="16,-52 21,-38 36,-38 24,-28 28,-14 16,-22 4,-14 8,-28 -4,-38 11,-38" 
                     fill="#ffcc00" stroke="#d97706" stroke-width="3.5" stroke-linejoin="round"/>
            <circle cx="16" cy="-33" r="3.5" fill="#ffffff"/>
          </g>
        </g>

        <!-- [정통 산리오 헬로키티 얼굴 (황금 타원형 비율 + 귀)] -->
        <g id="kitty-face-group">
          <!-- 
            얼굴 윤곽:
            산리오 고유의 넓적하고 낮은 타원형 귀와 볼 라인
            폭 240, 높이 180의 완벽한 1.33:1 가로 타원 비율
          -->
          <path d="M 98 75 
                   C 80 40, 56 46, 68 96 
                   C 36 130, 42 195, 108 222 
                   C 138 232, 202 232, 232 222 
                   C 298 195, 304 130, 272 96 
                   C 284 46, 260 40, 242 75 
                   C 205 63, 135 63, 98 75 Z" 
                fill="#ffffff" stroke="#1e1b18" stroke-width="8" stroke-linejoin="round"/>

          <!-- [콧수염: 양 볼에 3줄씩, 단정하고 정확한 산리오 앵글] -->
          <!-- 왼쪽 볼 수염 (3개) -->
          <line x1="42" y1="138" x2="94" y2="142" stroke="#1e1b18" stroke-width="6.5" stroke-linecap="round"/>
          <line x1="38" y1="158" x2="92" y2="158" stroke="#1e1b18" stroke-width="6.5" stroke-linecap="round"/>
          <line x1="45" y1="178" x2="95" y2="173" stroke="#1e1b18" stroke-width="6.5" stroke-linecap="round"/>

          <!-- 오른쪽 볼 수염 (3개) -->
          <line x1="298" y1="138" x2="246" y2="142" stroke="#1e1b18" stroke-width="6.5" stroke-linecap="round"/>
          <line x1="302" y1="158" x2="248" y2="158" stroke="#1e1b18" stroke-width="6.5" stroke-linecap="round"/>
          <line x1="295" y1="178" x2="245" y2="173" stroke="#1e1b18" stroke-width="6.5" stroke-linecap="round"/>

          <!-- [두 눈: 낮고 넓게 위치한 세로 타원형 순수 블랙] -->
          <!-- 왼쪽 눈 (x: 122, y: 158) -->
          <ellipse cx="122" cy="158" rx="8" ry="11.5" fill="#1e1b18"/>
          <!-- 오른쪽 눈 (x: 218, y: 158) -->
          <ellipse cx="218" cy="158" rx="8" ry="11.5" fill="#1e1b18"/>

          <!-- [코: 두 눈 사이의 하단 수평 라인에 정중앙 위치한 샛노란 타원형] -->
          <ellipse cx="170" cy="173" rx="11" ry="8.5" fill="#ffcc00" stroke="#1e1b18" stroke-width="4.5"/>

          <!-- 산리오 헬로키티 공식 철칙: 입은 그리지 않음 (NO MOUTH) -->

          <!-- 은은하고 사랑스러운 딸기 볼터치 (생기 업) -->
          <ellipse cx="94" cy="170" rx="15" ry="9" fill="#ff7597" opacity="0.45"/>
          <ellipse cx="246" cy="170" rx="15" ry="9" fill="#ff7597" opacity="0.45"/>

          <!-- [산리오 시그니처 레드 리본 (키티 기준 오른쪽 귀, 보는 이 기준 왼쪽 앞 귀)] -->
          <g transform="translate(100, 75) rotate(-22)">
            <!-- 리본 왼쪽 날개 -->
            <ellipse cx="-28" cy="0" rx="25" ry="18" fill="#e6002b" stroke="#1e1b18" stroke-width="6"/>
            <!-- 리본 오른쪽 날개 -->
            <ellipse cx="28" cy="0" rx="25" ry="18" fill="#e6002b" stroke="#1e1b18" stroke-width="6"/>
            <!-- 리본 중앙 둥근 매듭 매듭구 -->
            <circle cx="0" cy="0" r="16" fill="#e6002b" stroke="#1e1b18" stroke-width="6"/>
            <!-- 입체 하이라이트 -->
            <ellipse cx="-4" cy="-4" rx="5" ry="3" fill="#ffffff" opacity="0.6"/>
          </g>
        </g>
      </svg>
      
      <!-- 인터랙티브 터치 안내 뱃지 -->
      <div class="inline-flex items-center gap-1.5 mt-2 px-3.5 py-1 bg-white/95 rounded-full border-2 border-pink-200 text-xs font-jua text-sanrio-crimson shadow-sm">
        <span class="animate-bounce">👉</span>
        <span>키티나 화면 아무 데나 터치해봐! 축포가 펑펑! 💥</span>
      </div>
    </div>

  </main>


  <!-- [하단 컨트롤 구역]: 원터치 응원 에너지 전송 & 카운터 -->
  <footer class="w-full max-w-sm mx-auto z-30 pb-2 sm:pb-3 flex flex-col items-center gap-2">
    
    <!-- 슈퍼 응원 에너지 팍팍 보내기 버튼 -->
    <button id="cheerPowerBtn" class="w-full py-3.5 sm:py-4 px-6 rounded-3xl bg-gradient-to-r from-sanrio-red via-pink-500 to-rose-500 text-white font-jua text-lg sm:text-xl shadow-xl shadow-pink-400/50 hover:brightness-105 active:scale-95 transition-all flex items-center justify-center gap-2.5 border-2 border-white cursor-pointer">
      <span class="text-2xl animate-spin-sparkle">💖</span>
      <span>응원 에너지 팍팍 보내기!</span>
      <span class="text-xl">🔥</span>
    </button>

    <!-- 실시간 응원 상태 -->
    <div class="w-full flex items-center justify-between px-3 text-xs font-jua text-neutral-600">
      <span>보낸 에너지: <strong id="energyValue" class="text-sanrio-red text-sm">100</strong>% 파워업!</span>
      <span class="text-sanrio-pastelPink">무조건 만점 합격 🎓💯</span>
    </div>
  </footer>


  <!-- 자바스크립트 로직: 무한 축포 파티클, 고해상도 Web Audio BGM 및 터치 반응 -->
  <script>
    // --- 1. Web Audio API 사운드 시스템 (통통 튀는 산리오 멜로디 & 차임) ---
    let audioCtx = null;
    let isBgmOn = true;
    let bgmInterval = null;
    let noteStep = 0;

    function getAudio() {
      if (!audioCtx) {
        audioCtx = new (window.AudioContext || window.webkitAudioContext)();
      }
      if (audioCtx.state === 'suspended') {
        audioCtx.resume();
      }
      return audioCtx;
    }

    // 맑고 뽀송한 차임 벨소리
    function playTone(freq, duration = 0.3, gainVal = 0.1, type = 'sine') {
      try {
        const ctx = getAudio();
        const osc = ctx.createOscillator();
        const gain = ctx.createGain();

        osc.type = type;
        osc.frequency.setValueAtTime(freq, ctx.currentTime);

        gain.gain.setValueAtTime(gainVal, ctx.currentTime);
        gain.gain.exponentialRampToValueAtTime(0.0001, ctx.currentTime + duration);

        osc.connect(gain);
        gain.connect(ctx.destination);

        osc.start();
        osc.stop(ctx.currentTime + duration);
      } catch (err) {}
    }

    // 화면 탭 시 경쾌한 팝 차임 사운드
    function playTapSound() {
      const scale = [523.25, 659.25, 783.99, 987.77, 1046.50, 1318.51];
      const note = scale[Math.floor(Math.random() * scale.length)];
      playTone(note, 0.28, 0.13, 'triangle');
    }

    // 축포 팡팡 메가 팡파레 화음
    function playFanfareSound() {
      const chord = [523.25, 659.25, 783.99, 1046.50, 1318.51]; // C major
      chord.forEach((freq, idx) => {
        setTimeout(() => playTone(freq, 0.55, 0.1, 'sine'), idx * 55);
      });
    }

    // 귀여운 키티 오르골 BGM 루프 (도-미-솔-라-시-도 펜타토닉 행진곡 풍)
    const bgmNotes = [
      523.25, 659.25, 783.99, 1046.50, 
      880.00, 1046.50, 783.99, 659.25, 
      698.46, 880.00, 1046.50, 880.00,
      783.99, 659.25, 587.33, 523.25
    ];

    function startMusic() {
      if (bgmInterval) clearInterval(bgmInterval);
      isBgmOn = true;
      document.getElementById('bgmIcon').className = 'fa-solid fa-volume-high text-sanrio-red animate-pulse';
      document.getElementById('bgmLabel').textContent = '키티 응원곡 ON';

      bgmInterval = setInterval(() => {
        if (!isBgmOn) return;
        const freq = bgmNotes[noteStep % bgmNotes.length];
        playTone(freq, 0.35, 0.045, 'sine');
        noteStep++;
      }, 330);
    }

    function stopMusic() {
      isBgmOn = false;
      if (bgmInterval) clearInterval(bgmInterval);
      document.getElementById('bgmIcon').className = 'fa-solid fa-volume-xmark text-neutral-400';
      document.getElementById('bgmLabel').textContent = '키티 응원곡 OFF';
    }

    document.getElementById('bgmToggleBtn').addEventListener('click', (e) => {
      e.stopPropagation();
      getAudio();
      if (isBgmOn) {
        stopMusic();
      } else {
        startMusic();
      }
    });


    // --- 2. 넌스톱 폭죽 & 연속 파티클 엔진 ---
    const partyColors = ['#e6002b', '#ff7597', '#ffcc00', '#ffffff', '#1a6fba', '#a855f7'];

    // 좌우 하단에서 끊임없이 솟아오르는 축제 폭죽
    function runAmbientFireworks() {
      if (typeof confetti !== 'function') return;

      confetti({
        particleCount: 5,
        angle: 60,
        spread: 60,
        origin: { x: 0, y: 0.85 },
        colors: partyColors,
        ticks: 200,
        gravity: 0.85,
        scalar: 1.15
      });

      confetti({
        particleCount: 5,
        angle: 120,
        spread: 60,
        origin: { x: 1, y: 0.85 },
        colors: partyColors,
        ticks: 200,
        gravity: 0.85,
        scalar: 1.15
      });
    }

    setInterval(runAmbientFireworks, 420);

    // 대형 축포 발사 (클릭 지점 또는 센터)
    function triggerMegaConfetti(e) {
      if (e) e.stopPropagation();
      getAudio();
      playFanfareSound();

      const x = e ? (e.clientX / window.innerWidth) : 0.5;
      const y = e ? (e.clientY / window.innerHeight) : 0.45;

      if (typeof confetti === 'function') {
        confetti({
          particleCount: 80,
          spread: 100,
          origin: { x, y },
          colors: partyColors,
          scalar: 1.3,
          ticks: 250
        });

        setTimeout(() => {
          confetti({
            particleCount: 60,
            angle: 90,
            spread: 120,
            origin: { x, y: Math.max(0.15, y - 0.1) },
            colors: ['#ffcc00', '#e6002b', '#ffffff', '#ff7597'],
            scalar: 1.2
          });
        }, 180);
      }
    }


    // --- 3. 인터랙티브 키티 반응 & 말풍선 격려 메시지 ---
    const kittySvg = document.getElementById('kittySvg');
    const bubbleText = document.getElementById('bubbleText');
    const speechBubble = document.getElementById('speechBubble');
    const energyValue = document.getElementById('energyValue');
    let totalEnergy = 100;

    const cheerMessages = [
      "너의 노력을 믿어! 넌 반드시 해내! 💖",
      "아는 문제는 술술, 찍은 건 전부 정답! 🎯",
      "키티가 온 우주의 합격 기운을 모아줄게! 🌟",
      "절대 떨지 마! 넌 진짜 준비된 천재야! 💯",
      "A+ 성적표 받고 맛있는 거 왕창 먹자! 🍰",
      "시험지 다 찢고 당당하게 나오자! 파이팅! 🔥",
      "내가 뒤에서 제일 크게 응원하고 있어! 🍀"
    ];

    function onKittyClick(e) {
      if (e) e.stopPropagation();
      getAudio();
      playFanfareSound();

      // 키티 신나게 점프
      kittySvg.classList.remove('animate-kitty-wiggle');
      kittySvg.classList.add('animate-kitty-jump');
      setTimeout(() => {
        kittySvg.classList.remove('animate-kitty-jump');
        kittySvg.classList.add('animate-kitty-wiggle');
      }, 950);

      // 말풍선 대사 변경 & 팝 효과
      const randomMsg = cheerMessages[Math.floor(Math.random() * cheerMessages.length)];
      bubbleText.textContent = randomMsg;
      speechBubble.classList.add('scale-110');
      setTimeout(() => speechBubble.classList.remove('scale-110'), 250);

      // 폭죽 & 파티클 스폰
      triggerMegaConfetti(e);
      spawnPopEmoji(e ? e.clientX : window.innerWidth / 2, e ? e.clientY : window.innerHeight / 2);
    }


    // --- 4. 화면 아무 곳이나 탭했을 때 반응하는 행운 이모지 파티클 ---
    const examLuckyEmojis = ['💯', '🅰️➕', '🍀', '🎯', '⭐', '💖', '🎀', '🎉'];

    function spawnPopEmoji(clientX, clientY) {
      const el = document.createElement('div');
      el.className = 'tap-pop-particle';
      el.style.left = `${clientX}px`;
      el.style.top = `${clientY}px`;
      el.textContent = examLuckyEmojis[Math.floor(Math.random() * examLuckyEmojis.length)];
      document.body.appendChild(el);

      setTimeout(() => {
        el.remove();
      }, 900);
    }

    window.addEventListener('pointerdown', (e) => {
      // 상단/하단 제어 버튼 클릭 제외
      if (e.target.closest('#bgmToggleBtn') || e.target.closest('#outfitBtn') || e.target.closest('#cheerPowerBtn')) {
        return;
      }

      getAudio();
      playTapSound();
      spawnPopEmoji(e.clientX, e.clientY);

      // 터치한 위치에서 미니 폭죽 팡!
      if (typeof confetti === 'function') {
        confetti({
          particleCount: 18,
          spread: 50,
          origin: { x: e.clientX / window.innerWidth, y: e.clientY / window.innerHeight },
          colors: partyColors,
          ticks: 120
        });
      }

      // 첫 상호작용 시 음악 자동 시작 보조
      if (isBgmOn && !bgmInterval) {
        startMusic();
      }
    });


    // --- 5. "응원 에너지 팍팍 보내기" 슈퍼 버튼 액션 ---
    document.getElementById('cheerPowerBtn').addEventListener('click', (e) => {
      e.stopPropagation();
      totalEnergy += 100;
      energyValue.textContent = totalEnergy;

      onKittyClick(e);

      // 화면 전역 슈퍼 축포
      if (typeof confetti === 'function') {
        confetti({
          particleCount: 120,
          spread: 160,
          origin: { y: 0.6 },
          colors: ['#e6002b', '#ffcc00', '#ffffff', '#ff7597', '#38bdf8']
        });
      }
    });


    // --- 6. 키티 오버롤 의상 토글 (클래식 블루 멜빵 ↔ 핑크 큐티 드레스) ---
    let isPinkOutfit = false;
    const outfitBtn = document.getElementById('outfitBtn');
    const outfitLabel = document.getElementById('outfitLabel');
    const overallsBase = document.getElementById('overallsBase');
    const strapLeft = document.getElementById('strapLeft');
    const strapRight = document.getElementById('strapRight');

    outfitBtn.addEventListener('click', (e) => {
      e.stopPropagation();
      getAudio();
      playTapSound();

      isPinkOutfit = !isPinkOutfit;
      if (isPinkOutfit) {
        overallsBase.setAttribute('fill', '#ff527b');
        strapLeft.setAttribute('stroke', '#ff527b');
        strapRight.setAttribute('stroke', '#ff527b');
        outfitLabel.textContent = '핑크 멜빵';
      } else {
        overallsBase.setAttribute('fill', '#1a6fba');
        strapLeft.setAttribute('stroke', '#1a6fba');
        strapRight.setAttribute('stroke', '#1a6fba');
        outfitLabel.textContent = '클래식 멜빵';
      }

      triggerMegaConfetti(e);
    });


    // 최초 로드 시 축포 발사 및 오디오 리스너 준비
    window.addEventListener('load', () => {
      setTimeout(() => {
        triggerMegaConfetti();
      }, 350);

      const unlockAudio = () => {
        getAudio();
        if (isBgmOn && !bgmInterval) {
          startMusic();
        }
        window.removeEventListener('click', unlockAudio);
        window.removeEventListener('touchstart', unlockAudio);
      };
      window.addEventListener('click', unlockAudio);
      window.addEventListener('touchstart', unlockAudio);
    });
  </script>
</body>
</html>
