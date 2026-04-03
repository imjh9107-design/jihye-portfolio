[index.html](https://github.com/user-attachments/files/26461542/index.html)
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>임지혜 | HR Data Analyst 포트폴리오</title>
  <meta name="description" content="데이터로 HR을 분석하고 발전시키고 싶은 임지혜의 포트폴리오입니다." />
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard/dist/web/static/pretendard.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  
  <style>
    :root {
      --bg-main: #f4f7fb;
      --text-main: #1e293b;
      --text-muted: #64748b;
      --primary: #4f46e5;
      --primary-light: #e0e7ff;
      --card-bg: rgba(255, 255, 255, 0.7);
      --card-border: rgba(255, 255, 255, 0.8);
      --shadow-sm: 0 4px 6px -1px rgba(0, 0, 0, 0.05), 0 2px 4px -1px rgba(0, 0, 0, 0.03);
      --shadow-lg: 0 20px 40px -10px rgba(0, 0, 0, 0.05);
      --border-radius: 24px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Pretendard', sans-serif;
      background-color: var(--bg-main);
      color: var(--text-main);
      line-height: 1.6;
      min-height: 100vh;
      position: relative;
      overflow-x: hidden;
    }

    /* Elegant Background Float Elements */
    .bg-shape {
      position: absolute;
      border-radius: 50%;
      filter: blur(80px);
      z-index: -1;
      opacity: 0.6;
      animation: float 20s infinite alternate cubic-bezier(0.4, 0, 0.2, 1);
    }

    .shape-1 {
      width: 500px; height: 500px;
      background: #c7d2fe;
      top: -100px; left: -200px;
    }

    .shape-2 {
      width: 400px; height: 400px;
      background: #e0e7ff;
      bottom: 20%; right: -100px;
      animation-delay: -5s;
    }

    .shape-3 {
      width: 300px; height: 300px;
      background: #fbcfe8;
      top: 40%; left: 30%;
      animation-delay: -10s;
    }

    @keyframes float {
      0% { transform: translate(0, 0) scale(1); }
      100% { transform: translate(70px, 70px) scale(1.1); }
    }

    main {
      max-width: 900px;
      margin: 0 auto;
      padding: 60px 20px;
      display: flex;
      flex-direction: column;
      gap: 24px;
      position: relative;
      z-index: 1;
    }

    /* Glassmorphism Card Style */
    .card {
      background: var(--card-bg);
      backdrop-filter: blur(20px);
      -webkit-backdrop-filter: blur(20px);
      border: 1px solid var(--card-border);
      border-radius: var(--border-radius);
      padding: 40px;
      box-shadow: var(--shadow-lg);
      transition: transform 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275), box-shadow 0.4s ease;
    }

    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 30px 60px -15px rgba(0, 0, 0, 0.1);
    }

    .section-header {
      display: flex;
      align-items: center;
      gap: 14px;
      margin-bottom: 20px;
    }

    .icon-wrapper {
      width: 44px; height: 44px;
      background: var(--primary-light);
      color: var(--primary);
      border-radius: 12px;
      display: flex; justify-content: center; align-items: center;
      font-size: 20px;
    }

    .highlight-icon {
      background: linear-gradient(135deg, #4f46e5, #ec4899);
      color: white;
    }

    h1 {
      font-size: 48px; font-weight: 800; margin: 0 0 16px 0;
      letter-spacing: -1px; color: #0f172a;
    }

    h2 {
      font-size: 26px; font-weight: 700; margin: 0;
      color: #1e293b; letter-spacing: -0.5px;
    }

    p {
      color: var(--text-muted); font-size: 16.5px; margin-bottom: 14px;
      word-break: keep-all;
    }

    p:last-child { margin-bottom: 0; }
    strong { color: var(--text-main); font-weight: 600; }

    /* Hero Section */
    .hero {
      padding: 50px 40px;
      background: linear-gradient(135deg, rgba(255,255,255,0.9) 0%, rgba(255,255,255,0.4) 100%);
      position: relative; overflow: hidden;
    }

    .badge {
      display: inline-block; padding: 8px 18px;
      background: var(--primary); color: white;
      border-radius: 999px; font-size: 14px; font-weight: 600;
      margin-bottom: 20px; box-shadow: 0 4px 14px rgba(79, 70, 229, 0.4);
    }

    .subtitle {
      color: var(--text-muted); font-size: 20px; font-weight: 400; line-height: 1.5; margin-bottom: 0;
    }

    /* Grid layout for Strength */
    .grid {
      display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 20px; margin-top: 24px;
    }

    .grid-card {
      background: rgba(255, 255, 255, 0.85); padding: 24px; border-radius: 16px;
      border: 1px solid rgba(255, 255, 255, 1); box-shadow: var(--shadow-sm);
      transition: all 0.3s ease; display: flex; flex-direction: column;
    }

    .grid-card:hover {
      background: #ffffff; transform: translateY(-4px); box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.05);
    }

    .grid-icon { font-size: 24px; color: var(--primary); margin-bottom: 16px; }
    .grid-card h3 { font-size: 18px; font-weight: 700; margin-bottom: 8px; color: #1e293b; }
    .grid-card p { font-size: 14.5px; line-height: 1.5; margin: 0; }

    /* Split Layout for dual sections */
    .split-layout { display: flex; gap: 24px; }
    .split-item { flex: 1; margin-bottom: 0; }

    /* Personality text */
    .mbti-badge {
      display: inline-block; font-size: 36px; font-weight: 800; color: transparent;
      background: linear-gradient(135deg, #4f46e5, #0ea5e9);
      -webkit-background-clip: text; margin-bottom: 16px; letter-spacing: 1px;
    }

    /* Lists */
    .interest-list { list-style: none; display: flex; flex-direction: column; gap: 16px; }
    .interest-list li {
      display: flex; align-items: flex-start; gap: 16px; padding: 16px;
      background: rgba(255,255,255,0.7); border-radius: 12px; transition: background 0.2s ease;
    }
    .interest-list li:hover { background: rgba(255,255,255,1); }
    .interest-list i {
      font-size: 20px; color: var(--primary); background: var(--primary-light);
      width: 44px; height: 44px; display: flex; justify-content: center; align-items: center;
      border-radius: 50%; flex-shrink: 0;
    }
    .interest-list div { display: flex; flex-direction: column; gap: 2px; }
    .interest-list strong { font-size: 16px; }
    .interest-list span { font-size: 14px; color: var(--text-muted); }

    /* Goal section custom */
    .goal-section {
      background: linear-gradient(135deg, #ffffff 0%, rgba(248, 250, 252, 0.8) 100%);
    }
    .goal-text { font-size: 18px; line-height: 1.7; color: #334155; }
    .goal-text strong {
      color: var(--primary); background: linear-gradient(120deg, rgba(79, 70, 229, 0.15) 0%, rgba(79, 70, 229, 0.15) 100%);
      background-repeat: no-repeat; background-size: 100% 30%; background-position: 0 92%;
    }

    /* Animations */
    .slide-up {
      opacity: 0; transform: translateY(40px);
      transition: opacity 0.8s cubic-bezier(0.165, 0.84, 0.44, 1), transform 0.8s cubic-bezier(0.165, 0.84, 0.44, 1);
    }
    .slide-up.visible { opacity: 1; transform: translateY(0); }
    .delay-1 { transition-delay: 0.1s; }
    .delay-2 { transition-delay: 0.2s; }
    .delay-3 { transition-delay: 0.3s; }
    .delay-4 { transition-delay: 0.4s; }
    .delay-5 { transition-delay: 0.5s; }

    /* Mobile logic */
    @media (max-width: 768px) {
      main { padding: 30px 16px; gap: 16px; }
      .split-layout { flex-direction: column; gap: 16px; }
      .card { padding: 24px; }
      h1 { font-size: 36px; }
      h2 { font-size: 22px; }
      .subtitle { font-size: 17px; }
    }
  </style>
</head>
<body>
  <!-- Ambient Background Elements -->
  <div class="bg-shape shape-1"></div>
  <div class="bg-shape shape-2"></div>
  <div class="bg-shape shape-3"></div>

  <main>
    <!-- Hero Section -->
    <section class="card hero slide-up">
      <span class="badge">HR Data Analyst</span>
      <h1>임지혜</h1>
      <p class="subtitle">데이터로 사람과 조직을 이해하고,<br>더 나은 방향을 고민합니다.</p>
    </section>

    <!-- About Me Section -->
    <section class="card slide-up delay-1">
      <div class="section-header">
        <div class="icon-wrapper"><i class="fa-solid fa-user"></i></div>
        <h2>About Me</h2>
      </div>
      <p>안녕하세요. <strong>데이터로 HR을 분석하고 발전시키고 싶은 임지혜</strong>입니다.</p>
      <p>급여, 4대보험, 퇴직연금 등 HR 실무를 경험하며 숫자와 기준, 그리고 프로세스의 중요성을 꾸준히 배워왔습니다.</p>
      <p>이제는 단순 운영을 넘어 데이터를 통해 문제를 더 정확하게 보고, 더 나은 방향을 제안할 수 있는 사람이 되고 싶습니다.</p>
    </section>

    <!-- Strength Section -->
    <section class="card slide-up delay-2">
      <div class="section-header">
        <div class="icon-wrapper"><i class="fa-solid fa-bolt"></i></div>
        <h2>Strength</h2>
      </div>
      <div class="grid">
        <div class="grid-card">
          <div class="grid-icon"><i class="fa-solid fa-briefcase"></i></div>
          <h3>실무 경험</h3>
          <p>급여, 4대보험, 퇴직연금 등 HR 전반 업무 경험</p>
        </div>
        <div class="grid-card">
          <div class="grid-icon"><i class="fa-solid fa-magnifying-glass-chart"></i></div>
          <h3>문제 해결</h3>
          <p>오류를 줄이고 업무 흐름을 정리하는 데 강점</p>
        </div>
        <div class="grid-card">
          <div class="grid-icon"><i class="fa-solid fa-chart-line"></i></div>
          <h3>데이터 관심</h3>
          <p>숫자 기반으로 원인을 찾고 개선 방향을 고민</p>
        </div>
      </div>
    </section>

    <!-- Split Layout for Personality & Interests -->
    <div class="split-layout">
      <!-- Personality -->
      <section class="card split-item slide-up delay-3">
        <div class="section-header">
          <div class="icon-wrapper"><i class="fa-solid fa-brain"></i></div>
          <h2>Personality</h2>
        </div>
        <div class="mbti-badge">ISTP</div>
        <p>차분하고 현실적인 시각으로 문제를 바라보고, 복잡한 상황도 하나씩 정리하며 해결해가는 편입니다.</p>
      </section>

      <!-- Interests -->
      <section class="card split-item slide-up delay-4">
        <div class="section-header">
          <div class="icon-wrapper"><i class="fa-solid fa-heart"></i></div>
          <h2>Interests</h2>
        </div>
        <ul class="interest-list">
          <li>
            <i class="fa-solid fa-dumbbell"></i>
            <div>
              <strong>운동</strong>
              <span>꾸준함과 균형을 만드는 시간</span>
            </div>
          </li>
          <li>
            <i class="fa-solid fa-chart-pie"></i>
            <div>
              <strong>데이터분석</strong>
              <span>숫자로 흐름을 읽고 의미를 찾는 일</span>
            </div>
          </li>
          <li>
            <i class="fa-solid fa-baby"></i>
            <div>
              <strong>육아</strong>
              <span>일상 속에서 배우는 가장 현실적인 성장</span>
            </div>
          </li>
        </ul>
      </section>
    </div>

    <!-- Goal Section -->
    <section class="card slide-up delay-5 goal-section">
      <div class="section-header">
        <div class="icon-wrapper highlight-icon"><i class="fa-solid fa-flag-checkered"></i></div>
        <h2>Goal</h2>
      </div>
      <p class="goal-text">단순한 HR 운영을 넘어, <strong>데이터를 기반으로 조직과 사람을 이해하고 개선 방향을 제시</strong>할 수 있는 HR Data Analyst로 성장하는 것이 목표입니다.</p>
    </section>
  </main>
  
  <script>
    document.addEventListener("DOMContentLoaded", () => {
        // Elegant fade-in scrolling effect for all sections
        const observerOptions = {
            root: null,
            rootMargin: "0px",
            threshold: 0.15
        };

        const observer = new IntersectionObserver((entries, observer) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                    // Stop observing once animated
                    observer.unobserve(entry.target);
                }
            });
        }, observerOptions);

        const hiddenElements = document.querySelectorAll('.slide-up');
        hiddenElements.forEach((el) => observer.observe(el));
    });
  </script>
</body>
</html>
