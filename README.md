# Imran
<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>بيرجر الغرب • الصفحة الرئيسية</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --accent:#ff6b35; --muted:#9aa4b2; --glass: rgba(255,255,255,0.04);
      --glass-2: rgba(255,255,255,0.02);
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:'Cairo',system-ui,Arial; background:linear-gradient(180deg,#071026 0%, #072033 60%); color:#e6eef8}
    a{color:inherit;text-decoration:none}
    /* NAV */
    .nav{position:fixed;inset:auto 0 0 auto;top:0;right:0;left:0;padding:14px 28px;display:flex;align-items:center;justify-content:space-between;backdrop-filter: blur(6px);background:linear-gradient(0deg, rgba(0,0,0,0.28), rgba(0,0,0,0.12));z-index:100}
    .brand{display:flex;align-items:center;gap:12px;font-weight:800;font-size:20px}
    .brand .logo{width:44px;height:44px;border-radius:10px;background:linear-gradient(135deg,#ffd89b,#ff6b35);display:flex;align-items:center;justify-content:center;font-size:22px;box-shadow:0 6px 18px rgba(0,0,0,0.5)}
    .nav-links{display:flex;gap:18px;align-items:center}
    .btn{background:var(--accent);color:#fff;padding:10px 16px;border-radius:10px;font-weight:600;box-shadow:0 8px 18px rgba(255,107,53,0.12);}

    /* HERO */
    .hero{min-height:92vh;display:grid;grid-template-columns:1fr 480px;gap:36px;padding:90px 6vw 60px;align-items:center}
    .hero-left{max-width:820px}
    .eyebrow{display:inline-block;padding:6px 10px;border-radius:999px;background:var(--glass);color:var(--accent);font-weight:700;margin-bottom:18px}
    h1{font-size:48px;line-height:1.02;margin:0 0 14px}
    p.lead{color:var(--muted);font-size:18px;margin:0 0 20px}
    .actions{display:flex;gap:12px;margin-top:18px}
    .hero-cta{display:inline-flex;align-items:center;gap:10px}

    /* floating burger */
    .hero-right{position:relative}
    .burger-card{background:linear-gradient(180deg, rgba(255,255,255,0.04), rgba(255,255,255,0.02));border-radius:18px;padding:22px;backdrop-filter: blur(6px);}
    .floating-burger{position:absolute;top:-40px;left:40px;font-size:48px;transform:rotate(-15deg);animation:float 4s ease-in-out infinite}
    @keyframes float{0%{transform:translateY(0) rotate(-12deg)}50%{transform:translateY(-16px) rotate(2deg)}100%{transform:translateY(0) rotate(-12deg)}}

    /* Menu grid */
    .menu{padding:60px 6vw;background:linear-gradient(180deg, rgba(7,16,38,0.0), rgba(7,16,38,0.25));}
    .menu-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:20px}
    .card{background:var(--card);padding:16px;border-radius:14px;box-shadow:0 6px 18px rgba(2,6,23,0.6);transition:transform .32s, box-shadow .32s}
    .card:hover{transform:translateY(-8px);box-shadow:0 20px 40px rgba(2,6,23,0.6)}
    .price{font-weight:800;color:var(--accent);font-size:18px}

    /* gallery */
    .gallery{display:grid;grid-template-columns:1fr 320px;gap:20px;align-items:center;padding:60px 6vw}
    .gallery .slider{overflow:hidden;border-radius:14px}
    .slides{display:flex;gap:6px;transform:translateX(0);transition:transform .6s cubic-bezier(.2,.9,.2,1)}
    .slide{min-width:70%;height:320px;background-size:cover;background-position:center;border-radius:12px}

    /* features, counters */
    .features{padding:60px 6vw;display:flex;gap:24px;align-items:stretch}
    .feat{flex:1;background:var(--glass);padding:20px;border-radius:12px;text-align:center}
    .count{font-size:28px;font-weight:800;color:var(--accent)}

    /* testimonials */
    .testimonials{padding:60px 6vw;background:linear-gradient(180deg, rgba(255,255,255,0.01), transparent)}
    .test-cards{display:flex;gap:18px;overflow:auto;padding-bottom:8px}
    .test{min-width:280px;background:var(--card);padding:16px;border-radius:12px}

    /* contact */
    .contact{padding:60px 6vw 120px}
    form{display:grid;grid-template-columns:1fr 240px;gap:12px}
    input,textarea{padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit}

    footer{padding:24px 6vw;text-align:center;color:var(--muted)}

    /* reveal animations */
    .reveal{opacity:0;transform:translateY(18px);transition:all .7s cubic-bezier(.2,.9,.2,1)}
    .reveal.show{opacity:1;transform:translateY(0)}

    /* responsive */
    @media(max-width:900px){.hero{grid-template-columns:1fr;padding-top:120px}.hero-right{order:2}.burger-card{margin-top:14px}.gallery{grid-template-columns:1fr}}
    @media(max-width:520px){h1{font-size:34px}.nav-links{display:none}.hero{padding:100px 4vw}}
  </style>
</head>
<body>
  <nav class="nav">
    <div class="brand"><div class="logo">🍔</div><div>بيرجر الغرب</div></div>
    <div class="nav-links"><a class="btn" href="#menu">اطلب الآن</a></div>
  </nav>

  <header class="hero">
    <div class="hero-left">
      <div class="eyebrow">طعم أصيل — توصيل سريع</div>
      <h1 class="reveal">أشهى <span style="color:var(--accent)">بيرجر</span> في المنطقة — بلمسة منزلية</h1>
      <p class="lead reveal">نطبخ من مكونات طازجة، ونقدم بيرجر مُعدّ بحب. قوائم متنوعة، خيارات نباتية، وبرجر خاص بالمطعم — جربه اليوم!</p>
      <div class="actions reveal">
        <a class="btn hero-cta" href="#menu">قائمة الطعام</a>
        <a class="hero-cta" href="#contact" style="padding:10px 14px;border-radius:10px;background:transparent;border:1px solid rgba(255,255,255,0.06)">اتصل بنا</a>
      </div>

      <div style="margin-top:28px;display:flex;gap:14px;flex-wrap:wrap">
        <div class="card reveal" style="display:flex;gap:12px;align-items:center;"> <div style="font-size:28px">🚚</div><div><div style="font-weight:700">توصيل سريع</div><div style="color:var(--muted);font-size:13px">في غضون 30-45 دقيقة</div></div></div>
        <div class="card reveal" style="display:flex;gap:12px;align-items:center;"> <div style="font-size:28px">🌿</div><div><div style="font-weight:700">خيارات نباتية</div><div style="color:var(--muted);font-size:13px">نباتي؟ لدينا بدائل لذيذة</div></div></div>
      </div>

    </div>

    <div class="hero-right">
      <div class="floating-burger">🍔</div>
      <div class="burger-card reveal">
        <h3 style="margin:0 0 10px">برغر الأسبوع: الغربي الملكي</h3>
        <p style="margin:0 0 12px;color:var(--muted)">لحم فاخر، جبنة ذائبة، صوص سري، وخبز محمص طازج.</p>
        <div style="display:flex;gap:10px;align-items:center;justify-content:space-between">
          <div style="font-weight:800;font-size:18px">120 درهم</div>
          <div style="display:flex;gap:8px"><button class="btn">اطلب الآن</button><button style="padding:10px 12px;border-radius:10px;background:transparent;border:1px solid rgba(255,255,255,0.04)">شاهد القائمة</button></div>
        </div>
      </div>
    </div>
  </header>

  <section id="menu" class="menu">
    <h2 style="text-align:right;margin:0 0 18px">قائمة الطعام</h2>
    <div class="menu-grid">
      <div class="card reveal">
        <h4 style="margin:0 0 8px">الغربي الكلاسيكي</h4>
        <div style="color:var(--muted);font-size:14px;margin-bottom:10px">لحم بقر، خس، طماطم، صوص خاص</div>
        <div style="display:flex;justify-content:space-between;align-items:center"><div class="price">85 درهم</div><button class="btn">أضف للسلة</button></div>
      </div>
      <div class="card reveal">
        <h4 style="margin:0 0 8px">تشيكن كرنشي</h4>
        <div style="color:var(--muted);font-size:14px;margin-bottom:10px">فيليه دجاج مقرمش، جبنة، صوص باربيكيو</div>
        <div style="display:flex;justify-content:space-between;align-items:center"><div class="price">74 درهم</div><button class="btn">أضف للسلة</button></div>
      </div>
      <div class="card reveal">
        <h4 style="margin:0 0 8px">بيرجر نباتي</h4>
        <div style="color:var(--muted);font-size:14px;margin-bottom:10px">برجر نباتي محضر من الحمص والبقول</div>
        <div style="display:flex;justify-content:space-between;align-items:center"><div class="price">65 درهم</div><button class="btn">أضف للسلة</button></div>
      </div>
      <div class="card reveal">
        <h4 style="margin:0 0 8px">سِيدس و بطاطا مقلية</h4>
        <div style="color:var(--muted);font-size:14px;margin-bottom:10px">بطاطا مقرمشة مع صوص انتخابي</div>
        <div style="display:flex;justify-content:space-between;align-items:center"><div class="price">28 درهم</div><button class="btn">أضف للسلة</button></div>
      </div>
    </div>
  </section>

  <section class="gallery" aria-label="صور الأطعمة">
    <div class="slider reveal">
      <div class="slides" id="slides">
        <div class="slide" style="background-image:url('https://images.unsplash.com/photo-1550547660-d9450f859349?q=80&w=1200&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder')"></div>
        <div class="slide" style="background-image:url('https://images.unsplash.com/photo-1544025162-d76694265947?q=80&w=1200&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder')"></div>
        <div class="slide" style="background-image:url('https://images.unsplash.com/photo-1565299624946-b28f40a0ae38?q=80&w=1200&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder')"></div>
      </div>
    </div>
    <div style="padding:10px 0">
      <h3 style="margin:0 0 10px">لمحة عن أطباقنا</h3>
      <p style="color:var(--muted)">تشكيلة من الصور التي تُظهر جودة تقديمنا وحرصنا على التفاصيل. تصفح أكثر لترى تشكيلتنا كاملة.</p>
      <div style="display:flex;gap:8px;margin-top:16px"><button class="btn" onclick="prevSlide()">السابق</button><button class="btn" onclick="nextSlide()">التالي</button></div>
    </div>
  </section>

  <section class="features">
    <div class="feat reveal">
      <div style="font-size:34px">🍔</div>
      <div style="font-weight:700;margin-top:8px">جودة مضمونة</div>
      <div style="color:var(--muted);margin-top:6px">مكونات محلية وطازجة يومياً</div>
    </div>
    <div class="feat reveal">
      <div style="font-size:34px">⏱️</div>
      <div style="font-weight:700;margin-top:8px">سرعة وموثوقية</div>
      <div style="color:var(--muted);margin-top:6px">توصيل خلال أقصر وقت ممكن</div>
    </div>
    <div class="feat reveal">
      <div style="font-size:34px">💬</div>
      <div style="font-weight:700;margin-top:8px">دعم العملاء</div>
      <div style="color:var(--muted);margin-top:6px">ردود سريعة وودودة</div>
    </div>
  </section>

  <section class="testimonials">
    <h3 style="text-align:right;margin:0 0 18px">آراء الزبائن</h3>
    <div class="test-cards">
      <div class="test reveal"><strong>سعيد</strong><p style="color:var(--muted)">أفضل بيرجر جربته في حياتي — طعم ولا أروع!</p></div>
      <div class="test reveal"><strong>مريم</strong><p style="color:var(--muted)">خدمة سريعة والبرغر كان طري وذو نكهة مميزة.</p></div>
      <div class="test reveal"><strong>أحمد</strong><p style="color:var(--muted)">الخيارات النباتية ممتازة — أوصي به.</p></div>
    </div>
  </section>

  <section id="contact" class="contact">
    <h3 style="text-align:right;margin:0 0 12px">اتصل بنا</h3>
    <form onsubmit="event.preventDefault();alert('تم إرسال الطلب - هذا نموذج تجريبي');">
      <input placeholder="الاسم" required />
      <input placeholder="الهاتف أو البريد" required />
      <textarea placeholder="رسالتك / الطلب" rows="4"></textarea>
      <div style="grid-column:1/-1;display:flex;justify-content:flex-end"><button class="btn">ارسل</button></div>
    </form>
  </section>

  <footer>
    &copy; 2025 بيرجر الغرب — جميع الحقوق محفوظة • تصميم سريع
  </footer>

  <script>
    // Simple reveal on scroll
    const reveals = document.querySelectorAll('.reveal');
    const obs = new IntersectionObserver((entries)=>{
      entries.forEach(e=>{ if(e.isIntersecting) e.target.classList.add('show'); });
    },{threshold:0.12});
    reveals.forEach(r=>obs.observe(r));

    // Slider logic
    const slides = document.getElementById('slides');
    let idx = 0;
    function updateSlide(){
      const w = slides.children[0].getBoundingClientRect().width + 6; // gap
      slides.style.transform = `translateX(${-(w*idx)}px)`;
    }
    function nextSlide(){ idx = Math.min(idx+1, slides.children.length-1); updateSlide(); }
    function prevSlide(){ idx = Math.max(idx-1,0); updateSlide(); }
    // auto slide
    setInterval(()=>{ idx = (idx+1) % slides.children.length; updateSlide(); },4500);

    // small parallax on mouse
    document.addEventListener('mousemove', (e)=>{
      const el = document.querySelector('.floating-burger');
      if(!el) return;
      const x = (e.clientX - window.innerWidth/2)/30;
      const y = (e.clientY - window.innerHeight/2)/30;
      el.style.transform = `translate(${x}px,${y}px) rotate(-8deg)`;
    });
  </script>
</body>
</html>
