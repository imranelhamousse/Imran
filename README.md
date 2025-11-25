<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>بيرجر الغرب • تصميم بديل</title>
  <link href="https://fonts.googleapis.com/css2?family=Almarai:wght@300;400;700&display=swap" rel="stylesheet">
  <style>
    :root{--bg:#fff2eb;--card:#ffffff;--accent:#ff3b30;--muted:#6b6b6b}
    *{box-sizing:border-box}
    body{margin:0;font-family:'Almarai',sans-serif;background:linear-gradient(180deg,#fff2eb 0%, #ffe8de 100%);color:#222}
    a{color:inherit}
    header{position:sticky;top:0;background:rgba(255,255,255,0.85);backdrop-filter:blur(6px);z-index:50;border-bottom:1px solid rgba(0,0,0,0.06)}
    .container{max-width:1100px;margin:0 auto;padding:18px}
    .nav{display:flex;align-items:center;justify-content:space-between}
    .logo{display:flex;align-items:center;gap:12px}
    .logo .ico{width:48px;height:48px;border-radius:12px;background:linear-gradient(135deg,#ffd1c1,#ff3b30);display:flex;align-items:center;justify-content:center;font-size:22px;color:#fff}
    .cta{background:var(--accent);color:#fff;padding:10px 14px;border-radius:10px;font-weight:700}

    /* Hero with split diagonal */
    .hero{display:grid;grid-template-columns:1fr 420px;gap:24px;align-items:center;padding:40px 18px}
    .hero-card{background:var(--card);border-radius:16px;padding:22px;box-shadow:0 10px 30px rgba(0,0,0,0.06)}
    h1{margin:0;font-size:36px}
    p.lead{color:var(--muted);margin-top:8px}

    /* Animated SVG burger */
    .svg-wrap{display:flex;align-items:center;justify-content:center;height:320px}
    .burger-svg{width:260px;height:260px}
    .bun-top{transform-origin:50% 40%;animation:bounce 3s ease-in-out infinite}
    @keyframes bounce{0%{transform:translateY(0)}50%{transform:translateY(-14px) rotate(-2deg)}100%{transform:translateY(0)}}

    /* Long page sections */
    section{padding:40px 18px}
    .grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .menu-card{background:linear-gradient(180deg,#fff,#fff8f6);padding:14px;border-radius:12px;border:1px solid rgba(0,0,0,0.04)}
    .price{font-weight:800;color:var(--accent)}

    /* Order modal */
    .order-modal{position:fixed;right:18px;bottom:18px;background:var(--accent);color:#fff;padding:12px 16px;border-radius:12px;box-shadow:0 12px 30px rgba(0,0,0,0.18);cursor:pointer}

    /* Testimonials slider (css scroll snap) */
    .snap{display:flex;gap:12px;overflow:auto;padding-bottom:8px;scroll-snap-type:x mandatory}
    .snap > div{min-width:280px;flex:0 0 auto;scroll-snap-align:center;background:#fff;border-radius:12px;padding:14px;border:1px solid rgba(0,0,0,0.04)}

    footer{padding:28px 18px;text-align:center;color:var(--muted)}

    @media(max-width:900px){.hero{grid-template-columns:1fr}.grid-3{grid-template-columns:repeat(2,1fr)} }
    @media(max-width:560px){.grid-3{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="logo"><div class="ico">🍔</div><div><strong>بيرجر الغرب</strong><div style="font-size:12px;color:var(--muted)">نكهات لا تُقاوم</div></div></div>
      <div style="display:flex;gap:12px;align-items:center"><a class="cta" href="#menu">اطلب الآن</a><a href="#contact" style="font-size:14px;color:var(--muted)">تواصل</a></div>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="hero-card">
        <h1>تعرف على بيرجر الغرب — طابع غربي مع لمسة محلية</h1>
        <p class="lead">برغر محضر من مكونات مُنتقاة، خبز مخبوز يومياً، وصوصات منزلية سرية — جرب تشكيلاتنا الخاصة أو صمّم البرغر بنفسك.</p>

        <div style="display:flex;gap:12px;margin-top:18px;flex-wrap:wrap">
          <div style="background:#fff8f2;padding:10px;border-radius:10px;border:1px solid rgba(0,0,0,0.03)">توصيل سريع</div>
          <div style="background:#fff8f2;padding:10px;border-radius:10px;border:1px solid rgba(0,0,0,0.03)">مكونات طازجة</div>
          <div style="background:#fff8f2;padding:10px;border-radius:10px;border:1px solid rgba(0,0,0,0.03)">خيارات نباتية</div>
        </div>

        <div style="margin-top:22px;display:flex;gap:12px">
          <a class="cta" href="#menu">اطلب من القائم</a>
          <a style="padding:10px 14px;border-radius:10px;background:transparent;border:1px solid rgba(0,0,0,0.06)">القائمة الكاملة</a>
        </div>
      </div>

      <div class="svg-wrap">
        <!-- playful SVG burger with animated top bun -->
        <svg class="burger-svg" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
          <defs>
            <linearGradient id="g1" x1="0" x2="1"><stop offset="0" stop-color="#ffd1c1"/><stop offset="1" stop-color="#ff7a5a"/></linearGradient>
          </defs>
          <g transform="translate(100,100)">
            <g class="bun-top">
              <ellipse rx="68" ry="30" fill="url(#g1)"></ellipse>
              <g fill="#fff" opacity="0.9">
                <circle cx="-30" cy="-8" r="3"/>
                <circle cx="10" cy="-12" r="2.5"/>
                <circle cx="36" cy="-6" r="2"/>
              </g>
            </g>
            <ellipse cy="18" rx="72" ry="14" fill="#6a3b1a"></ellipse>
            <rect x="-68" y="4" width="136" height="30" rx="6" fill="#d4a23b"></rect>
            <ellipse cy="36" rx="70" ry="10" fill="#f6f0e4"></ellipse>
          </g>
        </svg>
      </div>
    </section>

    <section id="menu">
      <div class="container">
        <h2 style="margin:0 0 12px;text-align:right">قائمة مُختارة</h2>
        <div class="grid-3">
          <div class="menu-card">
            <h4 style="margin:0">الملك الغربي</h4>
            <p style="color:var(--muted);margin:6px 0">لحم بقري ممتاز، جبنة شيدر، بصل مكرمل</p>
            <div style="display:flex;justify-content:space-between;align-items:center"><div class="price">95 درهم</div><button style="padding:8px 12px;border-radius:10px;background:linear-gradient(90deg,#ff6b50,#ff3b30);color:#fff;border:none">أضف</button></div>
          </div>
          <div class="menu-card">
            <h4 style="margin:0">تشيكن سبايسي</h4>
            <p style="color:var(--muted);margin:6px 0">فيليه دجاج متبل ومقرمش</p>
            <div style="display:flex;justify-content:space-between;align-items:center"><div class="price">78 درهم</div><button style="padding:8px 12px;border-radius:10px;background:linear-gradient(90deg,#ff6b50,#ff3b30);color:#fff;border:none">أضف</button></div>
          </div>
          <div class="menu-card">
            <h4 style="margin:0">برغر نباتي بالحمص</h4>
            <p style="color:var(--muted);margin:6px 0">خيار صحي ونكهة رائعة</p>
            <div style="display:flex;justify-content:space-between;align-items:center"><div class="price">62 درهم</div><button style="padding:8px 12px;border-radius:10px;background:linear-gradient(90deg,#ff6b50,#ff3b30);color:#fff;border:none">أضف</button></div>
          </div>
        </div>
      </div>
    </section>

    <section style="background:linear-gradient(180deg,transparent,#fff8f6);">
      <div class="container">
        <h3 style="text-align:right;margin-bottom:12px">آراء العملاء</h3>
        <div class="snap">
          <div><strong>ليلى</strong><p style="color:var(--muted);margin:6px 0">أفضل برغر في المدينة، والخبز طازج كل صباح.</p></div>
          <div><strong>يوسف</strong><p style="color:var(--muted);margin:6px 0">الصلصات لديهم فريدة — لا أستطيع التوقف!</p></div>
          <div><strong>عائشة</strong><p style="color:var(--muted);margin:6px 0">خدمة سريعة ونظافة ممتازة.</p></div>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container">
        <h3 style="text-align:right">حجز و تواصل</h3>
        <form onsubmit="event.preventDefault();alert('شكراً! تم إرسال الرسالة (نموذج تجريبي)');" style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-top:12px">
          <input placeholder="الاسم" required style="padding:10px;border-radius:10px;border:1px solid rgba(0,0,0,0.06)" />
          <input placeholder="هاتف" required style="padding:10px;border-radius:10px;border:1px solid rgba(0,0,0,0.06)" />
          <textarea placeholder="رسالة" rows="4" style="grid-column:1/-1;padding:10px;border-radius:10px;border:1px solid rgba(0,0,0,0.06)"></textarea>
          <div style="grid-column:1/-1;text-align:left"><button class="cta">أرسل</button></div>
        </form>
      </div>
    </section>

  </main>

  <div class="order-modal" onclick="alert('نموذج الطلب: هذه واجهة تجريبية');">🛒 افتح الطلب</div>

  <footer>
    <div class="container">
      <small>© 2025 بيرجر الغرب — جميع الحقوق محفوظة</small>
    </div>
  </footer>
</body>
</html>

