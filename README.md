
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Story Komiku</title>
<style>
*{margin:0;padding:0;box-sizing:border-box}
body{background:#080e20;color:white;font-family:Arial,sans-serif}
header{padding:18px 6%;background:#101b35;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:15px}
.logo{font-size:25px;font-weight:bold;color:#36baff}
nav a{color:white;text-decoration:none;margin:8px;font-size:14px}
.hero{margin:22px auto;width:90%;min-height:300px;border-radius:18px;background:linear-gradient(90deg,#071226 5%,transparent),url('https://images.unsplash.com/photo-1578632767115-351597cf2477?w=1400') center/cover;display:flex;align-items:center;padding:35px}
.hero h1{font-size:38px;margin-bottom:12px}
.hero p{color:#d2e5ff;max-width:400px;line-height:1.6}
.btn{display:inline-block;margin-top:18px;background:#168bff;color:white;padding:12px 22px;border-radius:8px;text-decoration:none}
section{padding:20px 6%}
h2{margin-bottom:18px;color:#42baff}
.search{width:100%;padding:14px;border:1px solid #263c61;border-radius:10px;background:#101b35;color:white;margin-bottom:25px}
.categories{display:flex;gap:10px;flex-wrap:wrap;margin-bottom:25px}
.categories span{background:#152849;padding:10px 16px;border-radius:20px;color:#64c7ff}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(145px,1fr));gap:17px}
.card{background:#111e38;border-radius:12px;overflow:hidden;border:1px solid #203759;transition:.2s}
.card:hover{transform:translateY(-5px);border-color:#36baff}
.card img{width:100%;height:210px;object-fit:cover;display:block}
.card h3{font-size:15px;padding:10px 10px 4px}
.card p{font-size:12px;color:#a8bedc;padding:0 10px 12px}
footer{text-align:center;padding:35px;color:#8298b9;background:#101b35;margin-top:35px}
</style>
</head>
<body>

<header>
<div class="logo">✦ STORY KOMIKU</div>
<nav>
<a href="#">Beranda</a>
<a href="#komik">Komik</a>
<a href="#creator">Creator Studio</a>
<a href="#komunitas">Komunitas</a>
</nav>
</header>

<div class="hero">
<div>
<h1>Dunia Cerita Tanpa Batas</h1>
<p>Baca berbagai cerita menarik, temukan dunia baru, dan ciptakan komikmu sendiri bersama Story Komiku!</p>
<a href="#komik" class="btn">Jelajahi Komik →</a>
</div>
</div>

<section id="komik">
<h2>✦ Jelajahi Dunia Komik</h2>
<input class="search" id="search" placeholder="Cari judul komik..." oninput="cari()">
<div class="categories">
<span>Manga</span><span>Manhwa</span><span>Manhua</span><span>Action</span><span>Fantasy</span><span>Romance</span>
</div>

<div class="grid" id="daftar">
<div class="card"><img src="https://images.unsplash.com/photo-1578632767115-351597cf2477?w=500"><h3>Petualangan Baru</h3><p>Fantasy • Petualangan</p></div>
<div class="card"><img src="https://images.unsplash.com/photo-1614583225154-5fcdda07019e?w=500"><h3>Dunia Imajinasi</h3><p>Action • Fantasy</p></div>
<div class="card"><img src="https://images.unsplash.com/photo-1601850494422-3cf14624b0b3?w=500"><h3>Legenda Sang Hero</h3><p>Adventure • Action</p></div>
<div class="card"><img src="https://images.unsplash.com/photo-1613376023733-0a73315d9b06?w=500"><h3>Rahasia Dunia</h3><p>Mystery • Fantasy</p></div>
</div>
</section>

<section id="creator">
<h2>✦ Creator Studio</h2>
<p>Punya cerita sendiri? Bersiaplah menjadi creator di Story Komiku!</p>
<a href="#" class="btn">Segera Hadir</a>
</section>

<section id="komunitas">
<h2>✦ Komunitas Komiku</h2>
<p>Tempat berkumpulnya pembaca dan pencipta cerita.</p>
</section>

<footer>
© 2026 Story Komiku — Read, Create, Imagine.
</footer>

<script>
function cari(){
let q=document.getElementById('search').value.toLowerCase();
document.querySelectorAll('.card').forEach(card=>{
card.style.display=card.innerText.toLowerCase().includes(q)?'block':'none';
});
}
</script>
</body>
</html>

