<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>NEPUS | المؤسسة الوطنية لتوريد وتجهيز الزي المهني</title>
  <meta name="description" content="المؤسسة الوطنية لتوريد وتجهيز الزي المهني (NEPUS) — توريد وتصنيع وتخصيص الزي المهني للمستشفيات والفنادق والمصانع والقطاعات المختلفة." />

  <!-- Tailwind CDN -->
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet" />
  <style>
    :root{
      --brand-blue:#004C97; /* أزرق رسمي */
      --brand-blue-600:#0a5fb3;
      --brand-gray:#4A4A4A; /* رمادي داكن */
      --brand-gray-200:#D9D9D9; /* رمادي فاتح */
    }
    .brand-gradient{background:linear-gradient(135deg,var(--brand-blue),#0b6fd6);} 
    .container{max-width:1100px}
    .logo-mark{width:42px;height:42px}
    html{scroll-behavior:smooth}
  </style>
</head>
<body class="bg-white text-gray-800">
  <!-- Header -->
  <header class="sticky top-0 z-50 bg-white/90 backdrop-filter backdrop-blur border-b border-gray-100">
    <div class="container mx-auto px-4 py-3 flex items-center justify-between">
      <div class="flex items-center space-x-3 space-x-reverse">
        <!-- Simple shield + NU monogram -->
        <svg class="logo-mark" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
          <path d="M32 4l22 8v18c0 16-10 26-22 30C20 56 10 46 10 30V12l22-8z" fill="var(--brand-blue)"/>
          <path d="M22 22h6v18h-6V22zm14 0c3.866 0 7 3.134 7 7v11h-6V29a1 1 0 00-1-1h-5v-6h5z" fill="white"/>
        </svg>
        <div>
          <p class="font-bold text-lg" style="color:var(--brand-blue)">NEPUS</p>
          <p class="text-xs text-gray-500">المؤسسة الوطنية لتوريد وتجهيز الزي المهني</p>
        </div>
      </div>
      <nav class="hidden md:flex items-center gap-6 text-sm">
        <a href="#about" class="hover:text-blue-800" style="color:var(--brand-blue)">من نحن</a>
        <a href="#services" class="hover:text-blue-800" style="color:var(--brand-blue)">الخدمات</a>
        <a href="#sectors" class="hover:text-blue-800" style="color:var(--brand-blue)">القطاعات</a>
        <a href="#why" class="hover:text-blue-800" style="color:var(--brand-blue)">لماذا نحن</a>
        <a href="#contact" class="px-4 py-2 rounded-lg text-white" style="background:var(--brand-blue)">تواصل معنا</a>
      </nav>
      <button onclick="document.getElementById('mnav').classList.toggle('hidden')" class="md:hidden px-3 py-2 rounded border" style="border-color:var(--brand-blue);color:var(--brand-blue)">القائمة</button>
    </div>
    <div id="mnav" class="md:hidden hidden border-t">
      <div class="px-4 py-3 flex flex-col gap-3 text-sm">
        <a href="#about" onclick="mhide()" class="text-blue-900">من نحن</a>
        <a href="#services" onclick="mhide()" class="text-blue-900">الخدمات</a>
        <a href="#sectors" onclick="mhide()" class="text-blue-900">القطاعات</a>
        <a href="#why" onclick="mhide()" class="text-blue-900">لماذا نحن</a>
        <a href="#contact" onclick="mhide()" class="px-4 py-2 rounded-lg text-white text-center" style="background:var(--brand-blue)">تواصل معنا</a>
      </div>
    </div>
  </header>

  <!-- Hero -->
  <section class="brand-gradient text-white">
    <div class="container mx-auto px-4 py-16 md:py-24 grid md:grid-cols-2 gap-8 items-center">
      <div>
        <h1 class="text-3xl md:text-5xl font-extrabold leading-tight">حلول متكاملة للزي المهني<br/>توريد • تصنيع • تخصيص</h1>
        <p class="mt-4 text-lg text-white/90">نخدم المستشفيات، الفنادق، المصانع، المطاعم، المدارس والجهات الحكومية عبر شبكة موثوقة من التصنيع والتوريد محليًا ودوليًا.</p>
        <div class="mt-6 flex gap-3">
          <a href="#contact" class="px-5 py-3 rounded-lg font-semibold" style="background:#ffffff;color:var(--brand-blue)">اطلب عرض سعر</a>
          <a href="#services" class="px-5 py-3 rounded-lg font-semibold border border-white/70">تعرّف على خدماتنا</a>
        </div>
      </div>
      <div class="bg-white/10 rounded-2xl p-6 md:p-8">
        <ul class="grid grid-cols-2 gap-4 text-sm">
          <li class="bg-white/15 rounded-lg p-4"><span class="block text-2xl font-bold">+50</span> عميل نشط</li>
          <li class="bg-white/15 rounded-lg p-4"><span class="block text-2xl font-bold">+10</span> قطاعات نخدمها</li>
          <li class="bg-white/15 rounded-lg p-4"><span class="block text-2xl font-bold">+8</span> دول توريد</li>
          <li class="bg-white/15 rounded-lg p-4"><span class="block text-2xl font-bold">ISO</span> التزام بالجودة</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- About -->
  <section id="about" class="py-16 md:py-20 bg-gray-50">
    <div class="container mx-auto px-4">
      <div class="max-w-3xl">
        <h2 class="text-2xl md:text-3xl font-bold mb-4" style="color:var(--brand-blue)">من نحن</h2>
        <p class="text-gray-700 leading-8">NEPUS — المؤسسة الوطنية لتوريد وتجهيز الزي المهني. نقدم حلولًا متكاملة تشمل دراسة الاحتياج، التصميم، اختيار الأقمشة، التصنيع، التفصيل الخاص، الطباعة والتطريز، ثم التغليف والتوصيل، مع التزام كامل بمعايير الجودة والمواعيد.</p>
      </div>
    </div>
  </section>

  <!-- Services -->
  <section id="services" class="py-16 md:py-20">
    <div class="container mx-auto px-4">
      <h2 class="text-2xl md:text-3xl font-bold mb-10" style="color:var(--brand-blue)">الخدمات</h2>
      <div class="grid md:grid-cols-3 gap-6">
        <div class="p-6 rounded-xl border border-gray-100 shadow-sm">
          <h3 class="font-bold mb-2 text-lg" style="color:var(--brand-blue)">توريد الزي للمصانع</h3>
          <p class="text-gray-600">ملابس صناعية مقاومة للاهتراء والحرارة مع خيارات عاكسة للسلامة ومقاسات دقيقة للعمال.</p>
        </div>
        <div class="p-6 rounded-xl border border-gray-100 shadow-sm">
          <h3 class="font-bold mb-2 text-lg" style="color:var(--brand-blue)">زي المدارس</h3>
          <p class="text-gray-600">تصميمات بأقمشة مريحة ومتينة، تفصيل للأعمار المختلفة، وخيارات ألوان وهوية مدرسية.</p>
        </div>
        <div class="p-6 rounded-xl border border-gray-100 shadow-sm">
          <h3 class="font-bold mb-2 text-lg" style="color:var(--brand-blue)">سكرابات طبية للمستشفيات</h3>
          <p class="text-gray-600">Scrubs طبية بأقمشة قابلة للتنفس وسريعة الجفاف، مقاومة للبقع مع تطريز شعارات الأقسام.</p>
        </div>
        <div class="p-6 rounded-xl border border-gray-100 shadow-sm">
          <h3 class="font-bold mb-2 text-lg" style="color:var(--brand-blue)">تصميم وتخصيص الهوية</h3>
          <p class="text-gray-600">نماذج مقاسات، لوحات ألوان، تطريز/طباعة، وباكجات جاهزة للتسليم.</p>
        </div>
        <div class="p-6 rounded-xl border border-gray-100 shadow-sm">
          <h3 class="font-bold mb-2 text-lg" style="color:var(--brand-blue)">عقود توريد سنوية</h3>
          <p class="text-gray-600">توريد مرحلي مع جداول تسليم وأسعار تفضيلية وخيارات إعادة الطلب السريع.</p>
        </div>
        <div class="p-6 rounded-xl border border-gray-100 shadow-sm">
          <h3 class="font-bold mb-2 text-lg" style="color:var(--brand-blue)">خدمات لوجستية</h3>
          <p class="text-gray-600">تغليف، ترميز، تتبع شحنات، وتسليم لمواقع متعددة داخل المملكة.</p>
        </div>
      </div>
      <div class="mt-8">
        <a href="#contact" class="inline-block px-5 py-3 rounded-lg text-white font-semibold" style="background:var(--brand-blue)">اطلب عرض سعر الآن</a>
      </div>
    </div>
  </section>

  <!-- Sectors -->
  <section id="sectors" class="py-16 md:py-20 bg-gray-50">
    <div class="container mx-auto px-4">
      <h2 class="text-2xl md:text-3xl font-bold mb-6" style="color:var(--brand-blue)">القطاعات التي نخدمها</h2>
      <div class="flex flex-wrap gap-3">
        <span class="px-4 py-2 rounded-full border" style="border-color:var(--brand-blue);color:var(--brand-blue)">المستشفيات والمراكز الطبية</span>
        <span class="px-4 py-2 rounded-full border" style="border-color:var(--brand-blue);color:var(--brand-blue)">الفنادق والضيافة</span>
        <span class="px-4 py-2 rounded-full border" style="border-color:var(--brand-blue);color:var(--brand-blue)">المصانع والتشغيل</span>
        <span class="px-4 py-2 rounded-full border" style="border-color:var(--brand-blue);color:var(--brand-blue)">المطاعم والمقاهي</span>
        <span class="px-4 py-2 rounded-full border" style="border-color:var(--brand-blue);color:var(--brand-blue)">المدارس والجامعات</span>
        <span class="px-4 py-2 rounded-full border" style="border-color:var(--brand-blue);color:var(--brand-blue)">الأمن والسلامة</span>
      </div>
    </div>
  </section>

  <!-- Why Us -->
  <section id="why" class="py-16 md:py-20">
    <div class="container mx-auto px-4">
      <h2 class="text-2xl md:text-3xl font-bold mb-6" style="color:var(--brand-blue)">لماذا NEPUS؟</h2>
      <div class="grid md:grid-cols-4 gap-6">
        <div class="p-6 rounded-xl bg-gray-50 border border-gray-100">
          <h3 class="font-bold mb-2" style="color:var(--brand-blue)">جودة مضمونة</h3>
          <p class="text-gray-600">مواد مُختبرة ومطابقة للمواصفات مع رقابة جودة في كل مرحلة.</p>
        </div>
        <div class="p-6 rounded-xl bg-gray-50 border border-gray-100">
          <h3 class="font-bold mb-2" style="color:var(--brand-blue)">التزام بالمواعيد</h3>
          <p class="text-gray-600">خطط إنتاج وشحن واضحة مع نقاط تسليم مرحلية.</p>
        </div>
        <div class="p-6 rounded-xl bg-gray-50 border border-gray-100">
          <h3 class="font-bold mb-2" style="color:var(--brand-blue)">أسعار تنافسية</h3>
          <p class="text-gray-600">قيمة عالية مقابل السعر ضمن عقود مرنة.</p>
        </div>
        <div class="p-6 rounded-xl bg-gray-50 border border-gray-100">
          <h3 class="font-bold mb-2" style="color:var(--brand-blue)">دعم مستمر</h3>
          <p class="text-gray-600">فريق خدمة عملاء يتابع الطلب من الاستشارة حتى التسليم.</p>
        </div>
      </div>
    </div>
  </section>
  <!-- Gallery / Sectors Visual -->
  <section id="gallery" class="py-16 md:py-20 bg-gray-50">
    <div class="container mx-auto px-4">
      <h2 class="text-2xl md:text-3xl font-bold mb-6" style="color:var(--brand-blue)">نماذج من القطاعات التي نخدمها</h2>
      <div class="grid md:grid-cols-3 gap-6">
        <figure class="overflow-hidden rounded-2xl border border-gray-100 shadow-sm">
          <img src="https://images.unsplash.com/photo-1581091014534-8987c1d1d1d5?q=80&w=1200&auto=format&fit=crop" alt="عمّال مصنع بزي موحد" class="w-full h-56 object-cover"/>
          <figcaption class="p-4">
            <h3 class="font-bold mb-1" style="color:var(--brand-blue)">المصانع</h3>
            <p class="text-gray-600 text-sm">عمّال يرتدون زيًّا موحدًا مع تجهيزات السلامة.</p>
          </figcaption>
        </figure>
        <figure class="overflow-hidden rounded-2xl border border-gray-100 shadow-sm">
          <img src="https://images.unsplash.com/photo-1588072432836-e10032774350?q=80&w=1200&auto=format&fit=crop" alt="طلاب بزي مدرسي موحد" class="w-full h-56 object-cover"/>
          <figcaption class="p-4">
            <h3 class="font-bold mb-1" style="color:var(--brand-blue)">المدارس</h3>
            <p class="text-gray-600 text-sm">طلاب داخل المدرسة بزي موحد منسّق ومريح.</p>
          </figcaption>
        </figure>
        <figure class="overflow-hidden rounded-2xl border border-gray-100 shadow-sm">
          <img src="https://images.unsplash.com/photo-1582719478250-c89cae4dc85b?q=80&w=1200&auto=format&fit=crop" alt="كوادر طبية ترتدي سكراب موحد" class="w-full h-56 object-cover"/>
          <figcaption class="p-4">
            <h3 class="font-bold mb-1" style="color:var(--brand-blue)">المستشفيات</h3>
            <p class="text-gray-600 text-sm">كوادر طبية ترتدي Scrubs موحدة وعملية.</p>
          </figcaption>
        </figure>
      </div>
    </div>
  </section>

  <!-- Clients -->
  <section id="clients" class="py-16 md:py-20">
    <div class="container mx-auto px-4">
      <div class="flex items-center justify-between gap-4 mb-6">
        <h2 class="text-2xl md:text-3xl font-bold" style="color:var(--brand-blue)">عملاؤنا</h2>
        <a href="#contact" class="hidden md:inline-block px-4 py-2 rounded-lg text-white" style="background:var(--brand-blue)">اطلب عرض سعر</a>
      </div>
      <p class="text-gray-700 mb-6">نخدم طيفًا واسعًا من العملاء في المملكة: قطاع الصحة، التعليم، الصناعة، الضيافة، والأمن والسلامة.</p>
      <div class="grid grid-cols-2 md:grid-cols-5 gap-4">
        <div class="h-20 rounded-xl border border-gray-200 flex items-center justify-center text-gray-500">شعار عميل</div>
        <div class="h-20 rounded-xl border border-gray-200 flex items-center justify-center text-gray-500">شعار عميل</div>
        <div class="h-20 rounded-xl border border-gray-200 flex items-center justify-center text-gray-500">شعار عميل</div>
        <div class="h-20 rounded-xl border border-gray-200 flex items-center justify-center text-gray-500">شعار عميل</div>
        <div class="h-20 rounded-xl border border-gray-200 flex items-center justify-center text-gray-500">شعار عميل</div>
      </div>
      <div class="mt-8">
        <a href="#contact" class="inline-block px-5 py-3 rounded-lg text-white font-semibold" style="background:var(--brand-blue)">اطلب عرض سعر الآن</a>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="py-16 md:py-20 bg-gray-50">
    <div class="container mx-auto px-4">
      <div class="grid md:grid-cols-2 gap-8 items-start">
        <div>
          <h2 class="text-2xl md:text-3xl font-bold mb-4" style="color:var(--brand-blue)">تواصل معنا</h2>
          <p class="text-gray-700 mb-6">اطلب عرض سعر أو راسلنا وسيتم التواصل خلال 24 ساعة عمل.</p>
          <ul class="space-y-3 text-gray-700">
            <li><strong>الإيميل:</strong> info@nepus.sa</li>
            <li><strong>الهاتف:</strong> +966 59 099 2632</li>
            <li><strong>العنوان:</strong> المملكة العربية السعودية</li>
          </ul>
          <div class="mt-4 flex gap-3">
            <a href="https://wa.me/966590992632" class="px-4 py-2 rounded-lg text-white" style="background:var(--brand-blue)">واتساب مباشر</a>
            <a href="mailto:info@nepus.sa" class="px-4 py-2 rounded-lg border" style="border-color:var(--brand-blue);color:var(--brand-blue)">إرسال بريد</a>
          </div>
        </div>
        <form onsubmit="event.preventDefault(); alert('تم إرسال طلبك بنجاح، سنعاود التواصل قريبًا.');" class="bg-white p-6 rounded-2xl shadow border border-gray-100">
          <div class="grid grid-cols-1 gap-4">
            <div>
              <label class="block text-sm mb-1">الاسم</label>
              <input type="text" required class="w-full rounded-lg border px-3 py-2" placeholder="الاسم الكامل" />
            </div>
            <div>
              <label class="block text-sm mb-1">البريد الإلكتروني</label>
              <input type="email" required class="w-full rounded-lg border px-3 py-2" placeholder="example@domain.com" />
            </div>
            <div>
              <label class="block text-sm mb-1">رقم الجوال</label>
              <input type="tel" class="w-full rounded-lg border px-3 py-2" placeholder="05xxxxxxxx" />
            </div>
            <div>
              <label class="block text-sm mb-1">الرسالة</label>
              <textarea rows="4" required class="w-full rounded-lg border px-3 py-2" placeholder="اكتب طلبك بشكل مختصر"></textarea>
            </div>
            <button type="submit" class="mt-2 px-5 py-3 rounded-lg text-white font-semibold" style="background:var(--brand-blue)">إرسال</button>
          </div>
        </form>
      </div>
    </div>
  </section>

  <footer class="py-8 border-t">
    <div class="container mx-auto px-4 text-sm text-gray-600 flex flex-col md:flex-row items-center justify-between gap-3">
      <p>© <span id="year"></span> NEPUS — جميع الحقوق محفوظة</p>
      <p>المؤسسة الوطنية لتوريد وتجهيز الزي المهني</p>
    </div>
  </footer>

  <script>
    function mhide(){document.getElementById('mnav').classList.add('hidden')}
    document.getElementById('year').textContent = new Date().getFullYear()
  </script>
</body>
</html>
