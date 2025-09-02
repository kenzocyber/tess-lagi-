# tess-lagi-
<title>Kenzo | Ethical Hacker</title>
<script src="https://cdn.tailwindcss.com"></script>
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>

<style>
/* Background Gradient */
body {
  background: linear-gradient(-45deg, #0a0f1a, #111827, #0b2c3d, #16213e);
  background-size: 400% 400%;
  animation: gradientMove 15s ease infinite;
  font-family: 'Courier New', monospace;
  color: #cbd5e1;
}
@keyframes gradientMove {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

/* Neon Border Glow */
.card {
  border: 1px solid #00e0d6;
  border-radius: 0.5rem;
  padding: 1rem;
  background-color: rgba(10, 15, 25, 0.85);
  position: relative;
  overflow: hidden;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.card::before {
  content: "";
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: conic-gradient(from 0deg,#00e0d6,transparent,#00e0d6,transparent);
  animation: spin 6s linear infinite;
  z-index: 0;
  opacity: 0.4;
}
.card > * { position: relative; z-index: 1; }
.card:hover { transform: scale(1.03); box-shadow: 0 0 15px #00e0d6; }
@keyframes spin { 100% { transform: rotate(360deg); } }

/* Floating Particles */
.particles { position: fixed; top:0; left:0; width:100%; height:100%; z-index:-1; overflow:hidden; }
.particle { position:absolute; width:3px;height:3px; background:#00e0d6; border-radius:50%; opacity:0.35; animation: float 14s linear infinite; }
@keyframes float { from{transform:translateY(100vh) scale(0.4);opacity:0} 20%{opacity:0.7} to{transform:translateY(-10vh) scale(0.9);opacity:0} }

/* Glitch Text Effect */
.glitch { font-size:1.5rem; font-weight:bold; color:#00fff7; position:relative; display:inline-block; }
.glitch::before,.glitch::after{ content:attr(data-text); position:absolute; left:0;width:100%;overflow:hidden;clip:rect(0,900px,0,0);}
.glitch::before{ animation:glitchTop 2s infinite linear alternate-reverse; color:#ff00ff;}
.glitch::after{ animation:glitchBottom 1.5s infinite linear alternate-reverse; color:#00ffea;}
@keyframes glitchTop {0%{clip:rect(0,9999px,0,0);transform:translate(0);}10%{clip:rect(0,9999px,50%,0);transform:translate(-2px,-2px);}20%{clip:rect(0,9999px,0,0);transform:translate(0);}30%{clip:rect(0,9999px,50%,0);transform:translate(2px,2px);}100%{clip:rect(0,9999px,0,0);transform:translate(0);}}
@keyframes glitchBottom {0%{clip:rect(0,9999px,0,0);transform:translate(0);}10%{clip:rect(50%,9999px,100%,0);transform:translate(2px,-1px);}20%{clip:rect(0,9999px,0,0);transform:translate(0);}30%{clip:rect(50%,9999px,100%,0);transform:translate(-2px,1px);}100%{clip:rect(0,9999px,0,0);transform:translate(0);}}
</style>

<body>
<div class="particles"></div>

<!-- Judul -->
<h1 class="text-center mb-4 glitch" data-text="Kenzo — Ethical Hacker">Kenzo — Ethical Hacker</h1>
<p class="text-center text-sm text-slate-300 mb-6">Security Researcher & Pentester</p>

<!-- About / Visi Misi -->
<section class="card mx-2 mb-4" data-aos="fade-up">
  <h2 class="text-base font-bold text-cyan-300 mb-2">About Me & Visi Misi</h2>
  <p class="text-xs text-slate-300">Saya Kenzo, fokus dalam keamanan siber & ethical hacking. Tujuan saya adalah mengamankan sistem dan berbagi pengetahuan dengan komunitas.</p>
  <p class="text-xs text-slate-300 mt-2"><strong>Visi:</strong> Menjadi hacker etis yang memberi dampak positif bagi keamanan digital.</p>
  <p class="text-xs text-slate-300"><strong>Misi:</strong> Edukasi, eksplorasi sistem, berbagi pengetahuan, dan membantu perusahaan memperkuat keamanan mereka.</p>
</section>

<!-- Skills -->
<section class="card mx-2 mb-4" data-aos="fade-up">
  <h3 class="text-base font-bold text-cyan-300 mb-2">Skills</h3>
  <ul class="space-y-1 text-xs">
    <li>Web App Pentesting ⭐⭐⭐⭐⭐</li>
    <li>API Security ⭐⭐⭐⭐☆</li>
    <li>Network Hardening ⭐⭐⭐⭐☆</li>
    <li>Reverse Engineering ⭐⭐⭐☆</li>
    <li>OSINT & Threat Intel ⭐⭐⭐⭐⭐</li>
    <li>Social Engineering ⭐⭐⭐⭐☆</li>
    <li>Exploit Development ⭐⭐⭐⭐☆</li>
    <li>Malware Analysis ⭐⭐⭐☆☆</li>
    <li>Cloud Security ⭐⭐⭐⭐☆</li>
  </ul>
</section>

<!-- Projects -->
<section class="card mx-2 mb-4" data-aos="fade-up">
  <h3 class="text-base font-bold text-cyan-300 mb-2">Projects</h3>
  <ul class="space-y-1 text-xs">
    <li>Enterprise Audit ⭐⭐⭐⭐⭐</li>
    <li>Cloud Infra Review ⭐⭐⭐⭐☆</li>
    <li>Bug Bounty Findings ⭐⭐⭐⭐⭐</li>
    <li>API Security Hardening ⭐⭐⭐⭐☆</li>
    <li>XSS Detector ⭐⭐⭐⭐⭐</li>
    <li>AutoRecon ⭐⭐⭐⭐☆</li>
    <li>Nethunter-Termux ⭐⭐⭐⭐☆</li>
    <li>OSINT Automation Tool ⭐⭐⭐⭐☆</li>
  </ul>
</section>

<!-- Blog -->
<section class="card mx-2 mb-4" data-aos="fade-up">
  <h3 class="text-base font-bold text-cyan-300 mb-2">Blog</h3>
  <p class="text-xs text-slate-300">Berisi tips hacking, writeup bug bounty, dan insight keamanan digital. <a href="#" class="underline text-cyan-400">Visit My Blog</a></p>
</section>

<!-- Tools & Fitur Lainnya -->
<section class="card mx-2 mb-4" data-aos="fade-up">
  <h3 class="text-base font-bold text-cyan-300 mb-2">Tools & Fitur Lainnya</h3>
  <p class="text-xs text-slate-300">Kumpulan tools pribadi, script otomatis, dan fitur pelacakan etis. Bisa diakses oleh tim internal & edukasi.</p>
</section>

<!-- Promo Kelas & Dukungan -->
<section class="card mx-2 mb-4" data-aos="fade-up">
  <h3 class="text-base font-bold text-cyan-300 mb-2">Dukungan & Kelas</h3>
  <p class="text-xs text-slate-300 mb-2">
    Dukung oleh: <strong>Berita Payakumbuh</strong> dan <strong>Kominfo</strong>
  </p>
  <p class="text-xs text-slate-300 mb-2">
    Halo saya Kenzo, saya membuka <strong>kelas pemula</strong> untuk belajar Termux dan Linux secara praktis dan etis. Di kelas ini, Anda akan belajar:
    <ul class="list-disc ml-4 mt-1">
      <li>Dasar-dasar Linux & Termux</li>
      <li>Menguasai perintah terminal</li>
      <li>Praktik OSINT & ethical hacking sederhana</li>
      <li>Membuat tools hacking edukatif dan aman</li>
    </ul>
  </p>
  <p class="text-xs text-slate-300">Jika Anda berminat, segera hubungi kami melalui kontak di bawah.</p>
</section>

<!-- Search Skills / Projects / Contact -->
<section class="card mx-2 mb-4" data-aos="fade-up">
  <h3 class="text-base font-bold text-cyan-300 mb-2">Search</h3>
  <input id="searchInput" type="text" placeholder="Cari Skills / Projects / WA / Gmail..."
    class="w-full text-xs p-2 rounded bg-black text-white border border-cyan-400 mb-2 focus:outline-none focus:ring-2 focus:ring-cyan-400 transition-all" />
  <button id="searchBtn" class="w-full bg-cyan-500 text-black py-1 rounded font-bold text-xs hover:bg-cyan-400 transition-all mb-2">Search</button>
  <div id="searchResults" class="text-xs text-slate-300"></div>
</section>

<!-- Footer -->
<footer class="text-center text-[10px] text-slate-500 mt-6" data-aos="fade-up">
  <div>Website ini dibuat oleh <strong>Kenzo</strong></div>
  <div>Email: <a href="mailto:pykcyber@gmail.com" class="underline">pykcyber@gmail.com</a></div>
  <div>WA: <a href="https://wa.me/6283143490913" class="underline">+62 831-4349-0913</a></div>
  <div>© 2025 Kenzo. Semua hak cipta dilindungi.</div>
</footer>

<script>
AOS.init();

// Floating particles
const particlesContainer = document.querySelector('.particles');
for (let i = 0; i < 40; i++) {
  const p = document.createElement('div');
  p.classList.add('particle');
  p.style.left = Math.random() * 100 + 'vw';
  p.style.animationDuration = (10 + Math.random() * 10) + 's';
  p.style.opacity = Math.random() * 0.4 + 0.2;
  particlesContainer.appendChild(p);
}

// Search Functionality
const data = [
  { type: 'skill', name: 'Web App Pentesting' },
  { type: 'skill', name: 'API Security' },
  { type: 'skill', name: 'Network Hardening' },
  { type: 'skill', name: 'Reverse Engineering' },
  { type: 'skill', name: 'OSINT & Threat Intel' },
  { type: 'skill', name: 'Social Engineering' },
  { type: 'skill', name: 'Exploit Development' },
  { type: 'skill', name: 'Malware Analysis' },
  { type: 'skill', name: 'Cloud Security' },
  { type: 'project', name: 'Enterprise Audit' },
  { type: 'project', name: 'Cloud Infra Review' },
  { type: 'project', name: 'Bug Bounty Findings' },
  { type: 'project', name: 'API Security Hardening' },
  { type: 'project', name: 'XSS Detector' },
  { type: 'project', name: 'AutoRecon' },
  { type: 'project', name: 'Nethunter-Termux' },
  { type: 'project', name: 'OSINT Automation Tool' },
  { type: 'contact', name: 'pykcyber@gmail.com' },
  { type: 'contact', name: '+62 831-4349-0913' }
];

const input = document.getElementById('searchInput');
const button = document.getElementById('searchBtn');
const resultsDiv = document.getElementById('searchResults');

button.addEventListener('click', () => {
  const query = input.value.toLowerCase();
  const results = data.filter(item => item.name.toLowerCase().includes(query));
  if(results.length === 0){
    resultsDiv.innerHTML = '<p>Tidak ditemukan.</p>';
    return;
  }
  resultsDiv.innerHTML = results.map(item => `<p>${item.type.toUpperCase()}: ${item.name}</p>`).join('');
});
</script>
</body>
