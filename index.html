<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Work and Public - Fixed Edition</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700&display=swap" rel="stylesheet">
  <style>
    /* التنسيقات الأساسية */
    *{margin:0;padding:0;box-sizing:border-box}
    body{ background:#000; color:#0f0; font-family:'Cairo',sans-serif; overflow-x:hidden; }
    .content{ position:relative; z-index:2; text-align:center; padding:40px 20px; }
    
    /* تأثير النقاط */
    #dots { position:fixed; inset:0; z-index:1; pointer-events:none; display:none; }
    .dot { position:absolute; width:4px; height:4px; background:#0f0; border-radius:50%; box-shadow:0 0 6px #0f0; animation:float 10s infinite linear; }
    @keyframes float { 0%{transform:translateY(110vh)} 100%{transform:translateY(-10vh)} }

    /* الجدول */
    .table-wrapper { width: 100%; max-width: 1000px; margin: 30px auto; overflow-x: auto; border: 1px solid #0f0; background: rgba(0,20,0,0.9); }
    table { width: 100%; border-collapse: collapse; color: #fff; min-width: 600px; }
    th, td { padding: 12px; border: 1px solid rgba(0,255,0,0.2); }
    th { background: #0f0; color: #000; }
    
    /* الأزرار */
    .controls { display:flex; gap:10px; justify-content:center; margin-top:20px; }
    .btn { padding:12px 20px; background:#000; border:1px solid #0f0; color:#0f0; cursor:pointer; transition: 0.2s; font-family: 'Cairo'; }
    .btn:active { transform: scale(0.9); }
    
    .status-done { color: #0f0; }
    .status-wait { color: #ff0; }
    .link-direct { color: #0ff; font-size: 0.8rem; }
  </style>
</head>
<body>

<div id="dots"></div>

<div class="content">
  <h1 style="font-size: 2.5rem; text-shadow: 0 0 10px #0f0;">مرحباً بالجميع</h1>
  
  <p id="typewriter" style="margin: 20px 0; min-height: 1.5em;"></p>

  <div class="table-wrapper">
    <table>
      <thead>
        <tr>
          <th>العمل</th>
          <th>الجانب</th>
          <th>الحالة</th>
          <th>الرابط</th>
        </tr>
      </thead>
      <tbody id="tableBody"></tbody>
    </table>
  </div>

  <div class="controls">
    <button class="btn" id="musicBtn" onclick="toggleMusic()">🎵 تحميل الموسيقى</button>
    <button class="btn" id="effectBtn" onclick="toggleEffects()">✨ التأثيرات: متوقفة</button>
  </div>
</div>

<div id="player"></div> <script>
// 1. البيانات
const worksData = [
  {n: "website not name", s: "يمين", st: "قيد الإنشاء", u: "-"},
  {n: "lovers anime", s: "وسط", st: "مكتمل", u: "https://lovers-anime.com"},
  {n: "service mail", s: "يسار", st: "مكتمل", u: "https://mail-service.com"},
  {n: "more", s: "يمين", st: "قيد إنشاء لاحقاً", u: "-"},
  {n: "plateform", s: "وسط", st: "قيد إنشاء", u: "🔒 Private"}
];

// 2. تعبئة الجدول
const tbody = document.getElementById('tableBody');
worksData.forEach(w => {
  tbody.innerHTML += `<tr>
    <td>${w.n}</td>
    <td>${w.s}</td>
    <td class="${w.st === 'مكتمل' ? 'status-done' : 'status-wait'}">${w.st}</td>
    <td><a class="link-direct" href="${w.u}" target="_blank">${w.u}</a></td>
  </tr>`;
});

// 3. التحكم بالموسيقى (طريقة آمنة)
let player;
let isPlaying = false;

function toggleMusic() {
  const btn = document.getElementById('musicBtn');
  
  // إذا لم يتم تحميل API اليوتيوب بعد
  if (!window.YT) {
    btn.innerText = "⏳ جاري الاتصال...";
    const tag = document.createElement('script');
    tag.src = "https://www.youtube.com/iframe_api";
    document.body.appendChild(tag);
    return;
  }

  if (!player) {
    player = new YT.Player('player', {
      height: '0', width: '0', videoId: 'I-AlgFRP5CM',
      playerVars: { 'autoplay': 1, 'loop': 1, 'playlist': 'I-AlgFRP5CM' },
      events: {
        'onReady': (e) => { 
            e.target.playVideo(); 
            isPlaying = true;
            btn.innerText = "⏸️ إيقاف المعزوفة";
        },
        'onStateChange': (e) => {
            if(e.data == 1) { isPlaying = true; btn.innerText = "⏸️ إيقاف المعزوفة"; }
            else { isPlaying = false; btn.innerText = "▶️ تشغيل المعزوفة"; }
        }
      }
    });
  } else {
    if (isPlaying) { player.pauseVideo(); } else { player.playVideo(); }
  }
}

// 4. التحكم بالتأثيرات (بناءً على طلبك الأخير)
function toggleEffects() {
  const dotsContainer = document.getElementById('dots');
  const btn = document.getElementById('effectBtn');

  if (dotsContainer.style.display === 'none' || dotsContainer.style.display === '') {
    // تشغيل
    if (dotsContainer.innerHTML === "") { // إنشاء النقاط لأول مرة فقط
      for (let i = 0; i < 20; i++) {
        const d = document.createElement('div');
        d.className = 'dot';
        d.style.left = Math.random() * 100 + '%';
        d.style.animationDelay = Math.random() * 5 + 's';
        dotsContainer.appendChild(d);
      }
    }
    dotsContainer.style.display = 'block';
    btn.innerText = "✨ التأثيرات: تعمل";
    btn.style.boxShadow = "0 0 10px #0f0";
  } else {
    // إيقاف
    dotsContainer.style.display = 'none';
    btn.innerText = "🌑 التأثيرات: متوقفة";
    btn.style.boxShadow = "none";
  }
}

// 5. تأثير الكتابة
let i = 0;
const text = "لم يتم نشر اي مشاريع بعد الان.. تذكر المقولة دائماً.";
function type() {
  if (i < text.length) {
    document.getElementById("typewriter").innerHTML += text.charAt(i);
    i++;
    setTimeout(type, 50);
  }
}
window.onload = type;
</script>
</body>
</html>
