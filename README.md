# adanaa-lahmacun
<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Adana Lahmacun — Adana’nın ateşinden, sofranıza</title>
<meta name="description" content="Adana Lahmacun: özenle hazırlanan lezzetler, sıcak bir sofra ve Türk mutfağının vazgeçilmez tadı.">
<meta property="og:title" content="Adana Lahmacun"><meta property="og:description" content="Adana’nın ateşinden, sofranıza.">
<link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,600;0,800;1,600&family=Manrope:wght@400;600;800&display=swap" rel="stylesheet">
<style>
:root{--bg:#151412;--bg2:#211E1B;--red:#D94132;--or:#F08A3C;--cream:#F5EBDD;--mut:#B8B0A5;--ease:cubic-bezier(.22,1,.36,1);color-scheme:dark;box-sizing:border-box}
*,*::before,*::after{box-sizing:inherit}
html{scroll-behavior:smooth;scroll-padding-top:70px;height:auto}
body{margin:0;background:var(--bg);color:var(--cream);font:400 1rem/1.65 Manrope,system-ui,sans-serif;overflow-x:hidden;padding-top:env(safe-area-inset-top,0px);padding-bottom:calc(64px + env(safe-area-inset-bottom,0px))}
h1,h2,h3{font-family:'Playfair Display',Georgia,serif;font-weight:800;line-height:1.05;margin:0}
a{color:inherit}img{max-width:100%}
:focus-visible{outline:2px solid var(--or);outline-offset:3px}
.wrap{max-width:1200px;margin:auto;padding:0 22px}
section{padding:84px 0}
.light{background:var(--cream);color:#2a2420}.light .mut{color:#6b6258}
.mut{color:var(--mut)}
h2{font-size:clamp(2rem,6vw,3.6rem)}
.btn{display:inline-flex;align-items:center;justify-content:center;min-height:48px;padding:0 26px;border-radius:999px;border:1.5px solid var(--red);background:var(--red);color:#fff;font:800 .95rem Manrope;text-decoration:none;cursor:pointer;transition:transform .25s var(--ease),background .25s,color .25s}
.btn:hover{transform:translateY(-2px);background:var(--or);border-color:var(--or);color:#151412}.btn:active{transform:scale(.97)}
.btn.ghost{background:transparent;color:inherit;border-color:currentColor}
.btn.ghost:hover{background:var(--cream);color:#151412;border-color:var(--cream)}
.btn[aria-disabled=true]{opacity:.45;pointer-events:none}
.note{font-size:.8rem;color:var(--mut);margin:.5rem 0 0}
/* intro */
#intro{position:fixed;inset:0;z-index:100;background:var(--bg);display:grid;place-content:center;text-align:center;transition:opacity .6s,transform .6s var(--ease)}
#intro.out{opacity:0;transform:scale(1.04);pointer-events:none}
#intro .mark{overflow:hidden}
#intro .mark span{display:block;font:800 clamp(1.8rem,7vw,3.4rem) 'Playfair Display',serif;letter-spacing:.06em;animation:up .7s var(--ease) both}
#intro i{display:block;height:2px;background:var(--red);margin:14px auto;width:0;animation:w .6s .4s var(--ease) forwards}
#intro p{margin:0;color:var(--mut);font-style:italic;opacity:0;animation:f .5s .8s forwards}
@keyframes up{from{transform:translateY(105%)}to{transform:none}}@keyframes w{to{width:100%}}@keyframes f{to{opacity:1}}
/* nav */
header{position:fixed;top:env(safe-area-inset-top,0px);left:0;right:0;z-index:50;transition:background .4s,backdrop-filter .4s}
header.sc{background:rgba(21,20,18,.94);backdrop-filter:blur(8px)}
.nav{display:flex;align-items:center;justify-content:space-between;height:68px}
.logo{font:800 1.15rem 'Playfair Display',serif;letter-spacing:.08em;text-decoration:none;transition:letter-spacing .4s var(--ease)}.logo:hover{letter-spacing:.12em}
.links{display:flex;gap:30px}
.links a{position:relative;text-decoration:none;font-weight:600;font-size:.92rem;padding:6px 0}
.links a::after{content:"";position:absolute;left:0;bottom:0;height:2px;width:100%;background:var(--red);transform:scaleX(0);transform-origin:left;transition:transform .35s var(--ease)}
.links a:hover::after,.links a.on::after{transform:scaleX(1)}
.burger{display:none;background:none;border:0;color:inherit;width:48px;height:48px;font-size:1.6rem;cursor:pointer}
#mm{position:fixed;inset:0;z-index:60;background:var(--bg);display:flex;flex-direction:column;justify-content:center;padding:30px;gap:6px;transform:translateY(-100%);transition:transform .5s var(--ease);visibility:hidden}
#mm.open{transform:none;visibility:visible}
#mm a{font:800 2.4rem 'Playfair Display',serif;text-decoration:none;opacity:0;transform:translateY(20px);transition:.5s var(--ease)}
#mm.open a{opacity:1;transform:none;transition-delay:calc(var(--i)*70ms + 150ms)}
#mm .x{position:absolute;top:calc(14px + env(safe-area-inset-top,0px));right:14px;background:none;border:0;color:inherit;font-size:2rem;width:48px;height:48px;cursor:pointer}
/* hero */
.hero{min-height:100svh;display:flex;align-items:center;padding:110px 0 70px;position:relative;overflow:hidden;background:radial-gradient(60% 60% at 75% 50%,rgba(217,65,50,.28),transparent 70%),var(--bg)}
.hero .wrap{display:grid;grid-template-columns:1.1fr .9fr;gap:30px;align-items:center}
.eyebrow{font-weight:800;font-size:.8rem;letter-spacing:.14em;color:var(--or);margin:0 0 18px}
.hero h1{font-size:clamp(2.6rem,8.5vw,6rem)}
.hero h1 span{display:block;overflow:hidden;padding-bottom:.08em}
.hero h1 b{display:block;font-weight:800;animation:up .9s var(--ease) both;animation-delay:calc(var(--d) + 1.3s)}
.hero p.lead{max-width:440px;color:var(--mut);margin:22px 0 28px;animation:f .8s 2.2s both}
.ctas{display:flex;gap:12px;flex-wrap:wrap;animation:f .8s 2.4s both}
.art{position:relative;aspect-ratio:1;width:min(100%,520px);margin:auto;animation:pop 1.2s 1.5s var(--ease) both;transition:transform .3s ease-out}
@keyframes pop{from{opacity:0;transform:scale(.88)}to{opacity:1}}
.plate{position:absolute;inset:6%;border-radius:50%;background:radial-gradient(circle at 50% 50%,#2a2622 0 62%,#3a342e 63% 100%);box-shadow:0 40px 80px rgba(0,0,0,.6)}
.lah{position:absolute;inset:14%;border-radius:50%;overflow:hidden;background:
 radial-gradient(circle at 30% 35%,#b33a22 0 7%,transparent 8%),radial-gradient(circle at 62% 28%,#c4482a 0 6%,transparent 7%),radial-gradient(circle at 55% 62%,#a8321f 0 8%,transparent 9%),radial-gradient(circle at 28% 66%,#c0472b 0 6%,transparent 7%),radial-gradient(circle at 72% 58%,#b83d25 0 5%,transparent 6%),
 radial-gradient(circle at 50% 50%,#c9702f 0 55%,#8d4a1d 80%,#2b1608 100%)}
.lah::after{content:"";position:absolute;inset:0;background:linear-gradient(105deg,transparent 35%,rgba(255,235,200,.28) 50%,transparent 65%);transform:translateX(-120%);animation:sweep 6s 3s infinite}
@keyframes sweep{to{transform:translateX(120%)}}
.lemon{position:absolute;right:2%;bottom:12%;width:22%;aspect-ratio:1;border-radius:50% 50% 50% 0;background:radial-gradient(circle,#f6e27a 0 40%,#e8c23a 41%);transform:rotate(-30deg);box-shadow:0 10px 25px rgba(0,0,0,.5)}
.tag{position:absolute;background:var(--cream);color:#151412;font-weight:800;font-size:.75rem;padding:6px 12px;border-radius:99px;animation:drift 7s ease-in-out infinite}
@keyframes drift{50%{transform:translateY(-8px)}}
.scroll{position:absolute;left:50%;bottom:20px;width:2px;height:40px;background:linear-gradient(var(--or),transparent);animation:sd 1.8s infinite}
@keyframes sd{from{transform:translateY(-8px);opacity:0}50%{opacity:1}to{transform:translateY(8px);opacity:0}}
/* marquee */
.strip{background:var(--red);overflow:hidden;white-space:nowrap;padding:16px 0}
.strip div{display:inline-flex;animation:mq 28s linear infinite}
.strip:hover div,.strip:focus-within div{animation-play-state:paused}
.strip span{font:600 1.5rem 'Playfair Display',serif;font-style:italic;padding-right:2rem}
@keyframes mq{to{transform:translateX(-50%)}}
/* menu */
.mhead{display:flex;justify-content:space-between;align-items:end;gap:20px;flex-wrap:wrap;margin-bottom:30px}
.tabs{display:flex;gap:8px;overflow-x:auto;padding:4px 0 14px;margin-bottom:10px;scrollbar-width:none}
.tabs button{flex:none;min-height:44px;padding:0 20px;border-radius:99px;border:1.5px solid rgba(42,36,32,.3);background:transparent;color:inherit;font:800 .9rem Manrope;cursor:pointer;transition:.3s var(--ease)}
.tabs button[aria-selected=true]{background:var(--red);border-color:var(--red);color:#fff}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:22px}
.card{background:#fff8ee;border:1px solid rgba(42,36,32,.12);text-align:left;color:inherit;font:inherit;padding:0;cursor:pointer;display:flex;flex-direction:column;animation:cin .5s var(--ease) both;animation-delay:calc(var(--i)*60ms);transition:transform .35s var(--ease),background .3s}
.card:hover{transform:translateY(-6px);background:#fff}
@keyframes cin{from{opacity:0;transform:translateY(16px)}}
.ph{aspect-ratio:4/3;overflow:hidden;background:#2b2724;display:grid;place-items:center}
.ph i{width:62%;aspect-ratio:1;border-radius:50%;background:radial-gradient(circle,hsl(var(--h) 60% 52%) 0 50%,hsl(var(--h) 55% 28%) 100%);transition:transform .6s var(--ease)}
.card:hover .ph i{transform:scale(1.12)}
.cb{padding:16px 18px 20px;position:relative}
.cb h3{font-size:1.35rem}.cb p{font-size:.9rem;margin:6px 0 12px;color:#6b6258}
.price{font-weight:800;font-size:.82rem;color:var(--red)}
.cb::after{content:"";position:absolute;left:18px;bottom:0;height:3px;width:0;background:var(--red);transition:width .4s var(--ease)}.card:hover .cb::after{width:calc(100% - 36px)}
dialog{background:var(--bg2);color:var(--cream);border:1px solid var(--red);max-width:420px;width:calc(100% - 40px);padding:28px}
dialog::backdrop{background:rgba(0,0,0,.7)}
/* feature/about */
.split{display:grid;grid-template-columns:1fr 1fr;gap:56px;align-items:center}
.photo{aspect-ratio:4/5;overflow:hidden;position:relative;background:radial-gradient(circle at 40% 40%,#d9722e,#7a3216 55%,#1c0f08);clip-path:inset(0 0 0 0)}
.rv .photo{clip-path:inset(0 100% 0 0);transition:clip-path 1.2s var(--ease)}.rv.in .photo{clip-path:inset(0)}
.photo::after{content:"Görsel yer tutucu";position:absolute;left:14px;bottom:12px;font-size:.72rem;color:rgba(255,255,255,.75)}
.big{font:italic 600 6rem/1 'Playfair Display',serif;color:var(--red)}
.hl{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:30px}
.hl div{border-top:2px solid var(--red);padding-top:12px;font-weight:800}
.hl small{display:block;font-weight:400;color:#6b6258}
/* gallery */
.gal{display:grid;grid-template-columns:repeat(4,1fr);grid-auto-rows:150px;gap:10px}
.gal button{position:relative;border:0;padding:0;cursor:zoom-in;overflow:hidden;color:#fff;background:hsl(var(--h) 55% 30%)}
.gal button:nth-child(1){grid-row:span 2;grid-column:span 2}.gal button:nth-child(4){grid-row:span 2}
.gal button::before{content:"";position:absolute;inset:0;background:radial-gradient(circle at 50% 50%,hsl(var(--h) 65% 48%) 0,transparent 65%);transition:transform .7s var(--ease)}
.gal button:hover::before{transform:scale(1.25)}
.gal span{position:absolute;inset:auto 0 0;padding:30px 12px 10px;background:linear-gradient(transparent,rgba(0,0,0,.75));font-weight:600;font-size:.85rem;text-align:left;opacity:0;transition:opacity .3s}
.gal button:hover span,.gal button:focus-visible span{opacity:1}
#lb{position:fixed;inset:0;z-index:90;background:rgba(10,9,8,.95);display:grid;place-items:center;opacity:0;visibility:hidden;transition:.35s}
#lb.open{opacity:1;visibility:visible}
#lb .big-img{width:min(86vw,720px);aspect-ratio:4/3;transform:scale(.9);transition:transform .45s var(--ease);display:grid;place-items:end start;padding:18px;font-weight:600}
#lb.open .big-img{transform:none}
#lb button{position:absolute;background:none;border:0;color:#fff;font-size:2.2rem;width:56px;height:56px;cursor:pointer}
#lb .p{left:8px}#lb .n{right:8px}#lb .c{top:calc(10px + env(safe-area-inset-top,0px));right:8px}
/* reviews */
.rate{display:flex;align-items:center;gap:26px;flex-wrap:wrap;margin-top:24px}
.num{font:800 5rem 'Playfair Display',serif;line-height:1}
.stars{position:relative;font-size:2rem;letter-spacing:4px;color:rgba(42,36,32,.2)}
.stars b{position:absolute;inset:0;overflow:hidden;width:0;color:var(--red);transition:width 1.6s var(--ease);white-space:nowrap;font-weight:400}
/* location/contact/footer */
.loc{background:var(--bg2)}
.map{aspect-ratio:4/3;background:repeating-linear-gradient(45deg,#26221f 0 14px,#2b2724 14px 28px);display:grid;place-items:center;border:1px solid rgba(245,235,221,.12);text-align:center;padding:20px}
.pin{width:26px;height:26px;border-radius:50% 50% 50% 0;background:var(--red);transform:rotate(-45deg);margin:0 auto 12px}
dl{margin:20px 0}dt{font-weight:800;color:var(--or);font-size:.85rem}dd{margin:0 0 14px}
.final{text-align:center;background:var(--red);padding:90px 0}
.final .btn{background:var(--cream);color:#151412;border-color:var(--cream)}.final .btn:hover{background:#151412;color:var(--cream);border-color:#151412}
.final .btn.ghost{background:transparent;color:#fff;border-color:#fff}
footer{border-top:2px solid var(--red);padding:50px 0 30px}
.fg{display:grid;grid-template-columns:1.4fr 1fr 1fr;gap:30px}
footer a{display:block;text-decoration:none;color:var(--mut);padding:3px 0;transition:color .2s}footer a:hover{color:var(--or)}
.bar{display:none}
#top{position:fixed;right:16px;bottom:calc(80px + env(safe-area-inset-bottom,0px));width:48px;height:48px;border-radius:50%;border:1px solid var(--mut);background:var(--bg);color:var(--cream);cursor:pointer;opacity:0;pointer-events:none;transition:.3s;z-index:40}
#top.show{opacity:1;pointer-events:auto}
.rv .t{opacity:0;transform:translateY(24px);transition:.9s var(--ease)}.rv.in .t{opacity:1;transform:none}
.rv .t:nth-child(2){transition-delay:.12s}.rv .t:nth-child(3){transition-delay:.24s}
@media(max-width:820px){
 .links,.nav .btn{display:none}.burger{display:block}
 .hero .wrap,.split,.fg{grid-template-columns:1fr}
 .art{width:min(86%,380px)}.hero{padding-top:90px}
 .gal{grid-template-columns:repeat(2,1fr);grid-auto-rows:130px}.gal button:nth-child(1){grid-column:span 2}
 section{padding:64px 0}.hl{grid-template-columns:1fr}
 .bar{display:grid;grid-template-columns:1fr 1fr;position:fixed;left:0;right:0;bottom:0;z-index:45;background:var(--bg2);border-top:1px solid var(--red);padding:8px 12px calc(8px + env(safe-area-inset-bottom,0px));gap:10px}
 .bar .btn{min-height:46px}
}
@media(min-width:821px){body{padding-bottom:0}#top{bottom:20px}}
@media(prefers-reduced-motion:reduce){*,*::before,*::after{animation-duration:.01ms!important;animation-delay:0s!important;animation-iteration-count:1!important;transition-duration:.01ms!important;scroll-behavior:auto!important}.strip div{animation:none}}
</style>
</head>
<body>
<div id="intro" aria-hidden="true"><div class="mark"><span>ADANA LAHMACUN</span></div><i></i><p>Adana’nın ateşinden, sofranıza.</p></div>

<header id="hd"><div class="wrap nav">
 <a class="logo" href="#ana" id="logo">ADANA LAHMACUN</a>
 <nav class="links" aria-label="Ana menü"></nav>
 <a class="btn" href="#menu">Menüyü Keşfet</a>
 <button class="burger" id="bg" aria-label="Menüyü aç" aria-expanded="false">☰</button>
</div></header>
<div id="mm" role="dialog" aria-label="Menü"><button class="x" id="mx" aria-label="Kapat">×</button></div>

<main>
<section class="hero" id="ana"><div class="wrap">
 <div>
  <p class="eyebrow">ADANA’NIN GELENEKSEL LEZZETİ</p>
  <h1><span><b style="--d:0s">Bir Lezzet.</b></span><span><b style="--d:.12s">Bir Gelenek.</b></span><span><b style="--d:.24s">Adana Lahmacun.</b></span></h1>
  <p class="lead">Özenle hazırlanan lezzetler, sıcak bir sofra ve Türk mutfağının vazgeçilmez tadı.</p>
  <div class="ctas"><a class="btn" href="#menu">Menüyü Keşfet</a><a class="btn ghost" href="#iletisim">Bizi Ziyaret Et</a></div>
 </div>
 <div class="art" id="art" role="img" aria-label="Lahmacun, limon ve maydanoz çizimi (yer tutucu görsel)">
  <div class="plate"></div><div class="lah"></div><div class="lemon"></div>
  <span class="tag" style="top:8%;left:2%">Maydanoz</span><span class="tag" style="top:20%;right:0;animation-delay:-2s">Baharat</span><span class="tag" style="bottom:6%;left:12%;animation-delay:-4s">Limon</span>
 </div>
</div><div class="scroll" aria-hidden="true"></div></section>

<div class="strip" aria-hidden="true"><div id="mq"></div></div>

<section class="light" id="menu"><div class="wrap">
 <div class="mhead"><div><h2>Lezzetin En Güzel Hali</h2><p class="mut">Menümüzü keşfedin, favori lezzetinizi seçin.</p></div><a class="btn ghost" href="#iletisim">Tüm Menüyü Gör</a></div>
 <div class="tabs" role="tablist" aria-label="Menü kategorileri" id="tabs"></div>
 <div class="grid" id="grid" role="tabpanel" aria-live="polite"></div>
 <p class="note" style="color:#6b6258">Bu ürünler örnek içeriktir; restoranın doğrulanmış menüsü değildir. Fiyatlar onaylandığında güncellenecektir.</p>
</div></section>

<section><div class="wrap split rv">
 <div class="photo" role="img" aria-label="Yakın plan lahmacun (yer tutucu görsel)"></div>
 <div><div class="big t">1</div><h2 class="t">Her Lokmada Bir Adana Hikâyesi.</h2><p class="mut t">İnce açılmış hamur, baharatlı kıyma, taze maydanoz ve bir dilim limon. Adana sofrasının sade ama güçlü tadı, her tabakta yeniden anlatılıyor.</p><a class="btn t" href="#menu">Menüyü Keşfet</a></div>
</div></section>

<section class="light" id="hakkimizda"><div class="wrap split rv">
 <div><h2 class="t">Lezzetin Ardındaki Ruh</h2><p class="t" style="color:#6b6258">Sıcak bir karşılama, taze hazırlanan yemekler ve geleneğe saygı. Restoranın hikâyesi ve atmosferi onaylandığında bu alan güncellenecek.</p>
  <div class="hl t"><div>Lezzet<small>Taze malzeme</small></div><div>Misafirperverlik<small>Sıcak sofra</small></div><div>Gelenek<small>Adana mutfağı</small></div></div></div>
 <div class="photo" style="aspect-ratio:1" role="img" aria-label="Restoran atmosferi (yer tutucu görsel)"></div>
</div></section>

<section id="galeri"><div class="wrap"><h2 style="margin-bottom:10px">Galeri</h2><p class="mut" style="margin-bottom:26px">Gerçek restoran fotoğrafları eklenene kadar yer tutucu görseller gösterilir.</p><div class="gal" id="gal"></div></div></section>

<section class="light"><div class="wrap"><h2>Misafirlerimizin Görüşü</h2>
 <div class="rate" id="rate"><div class="num">3,6</div><div><div class="stars" aria-label="5 üzerinden 3,6">★★★★★<b id="fill" style="--w:72%">★★★★★</b></div><p class="mut" style="margin:6px 0 0">48 değerlendirme · Google Haritalar’da gösterilen puan</p></div></div>
 <p style="margin-top:22px"><a class="btn ghost cfg" data-k="mapsUrl" href="#" target="_blank" rel="noopener">Google’da Değerlendirmeleri Oku</a></p><p class="note cfg-n" data-k="mapsUrl"></p>
</div></section>

<section class="loc" id="iletisim"><div class="wrap split rv">
 <div><h2 class="t">Bizi Ziyaret Edin</h2><dl class="t"><dt>Adres</dt><dd id="adr"></dd><dt>Çalışma saatleri</dt><dd id="hrs"></dd><dt>Telefon</dt><dd id="tel"></dd></dl>
  <div class="ctas t"><a class="btn cfg" data-k="mapsUrl" href="#" target="_blank" rel="noopener">Yol Tarifi Al</a><a class="btn ghost cfg" data-k="phone" data-p="tel:" href="#">Şimdi Ara</a></div><p class="note cfg-n" data-k="mapsUrl"></p></div>
 <div class="map t"><div><div class="pin"></div><strong>Adana Lahmacun</strong><p class="mut" style="margin:6px 0 0" id="mapnote">Konum doğrulanmadı. Harita bağlantısı eklenince burada görünecek.</p></div></div>
</div></section>

<section class="final"><div class="wrap"><h2 style="color:#fff">Bugün Ne Yesek?</h2><p style="margin:14px 0 28px">Sevdiğiniz lezzeti seçin ve bizimle iletişime geçin.</p>
 <div class="ctas" style="justify-content:center;animation:none"><a class="btn" href="#menu">Menüye Bak</a><a class="btn ghost cfg" data-k="phone" data-p="tel:" href="#">Telefonla İletişim</a><a class="btn ghost cfg" data-k="whatsapp" data-w="1" href="#" target="_blank" rel="noopener">WhatsApp ile Sipariş</a></div>
 <p class="note cfg-n" data-k="phone" style="color:#fff"></p></div></section>
</main>

<footer><div class="wrap"><div class="fg">
 <div><div class="logo">ADANA LAHMACUN</div><p class="mut" style="max-width:320px">Adana mutfağının sade ve güçlü tadı, sıcak bir sofrada.</p></div>
 <div id="fl"></div>
 <div><a class="cfg" data-k="mapsUrl" href="#" target="_blank" rel="noopener">Google Haritalar</a><a class="cfg" data-k="instagram" href="#" target="_blank" rel="noopener">Instagram</a><a class="cfg" data-k="phone" data-p="tel:" href="#">Telefon</a></div>
</div><p class="note" style="margin-top:30px">© <span id="yr"></span> Adana Lahmacun</p></div></footer>

<div class="bar"><a class="btn" href="#menu">Menü</a><a class="btn ghost cfg" data-k="phone" data-p="tel:" href="#">Ara</a></div>
<button id="top" aria-label="Yukarı çık">↑</button>
<dialog id="dlg"><h3 id="dt"></h3><p id="dd" class="mut"></p><p id="dp" style="font-weight:800;color:var(--or)"></p><button class="btn" id="dc">Kapat</button></dialog>
<div id="lb" role="dialog" aria-modal="true" aria-label="Galeri"><button class="c" aria-label="Kapat">×</button><button class="p" aria-label="Önceki">‹</button><div class="big-img" id="li"></div><button class="n" aria-label="Sonraki">›</button></div>

<script>
/* ===== EDITABLE CONFIG — fill in verified details; empty values disable the related buttons ===== */
const CONFIG={
 phone:"",            // e.g. "+90..."
 whatsapp:"",         // digits only, e.g. "90..."
 address:"",
 mapsUrl:"",
 instagram:"",
 hours:[],            // e.g. [{d:"Pazartesi–Pazar",t:"09:00–22:00"}]
 waText:"Merhaba, Adana Lahmacun menüsü ve sipariş seçenekleri hakkında bilgi almak istiyorum.",
 nav:[["ana","Ana Sayfa"],["menu","Menümüz"],["hakkimizda","Hakkımızda"],["galeri","Galeri"],["iletisim","İletişim"]],
 cats:["Lahmacun","Kebaplar","Pideler","Mezeler","Tatlılar","İçecekler"],
 items:[ // price:null until verified
  {c:0,n:"Adana Lahmacun",d:"İnce hamur üzerinde baharatlı kıyma, yanında limon ve maydanoz.",p:null,h:12},
  {c:0,n:"Klasik Lahmacun",d:"Geleneksel tarifle sade ve hafif bir klasik.",p:null,h:20},
  {c:0,n:"Fındık Lahmacun",d:"Küçük boy, bol çeşitle paylaşmaya uygun.",p:null,h:28},
  {c:1,n:"Adana Kebap",d:"Közde pişirilen acılı kıyma kebabı.",p:null,h:8},
  {c:2,n:"Kıymalı Pide",d:"Fırında pişen, kıymalı geleneksel pide.",p:null,h:30},
  {c:4,n:"Künefe",d:"Sıcak servis edilen şerbetli tatlı.",p:null,h:38},
  {c:5,n:"Ayran",d:"Soğuk servis edilen geleneksel içecek.",p:null,h:48}],
 gallery:[["Lahmacun yakın plan",14],["Izgara",8],["Restoran atmosferi",32],["Masa düzeni",40],["Baharatlar",24],["Fırın ateşi",18]]
};
const $=(s,r=document)=>r.querySelector(s),$$=(s,r=document)=>[...r.querySelectorAll(s)];
const RM=matchMedia('(prefers-reduced-motion:reduce)').matches;
const PRICE_NA="Fiyat bilgisi için iletişime geçin";
/* intro */
const intro=$('#intro');const endIntro=()=>{intro.classList.add('out');setTimeout(()=>intro.remove(),700)};
try{sessionStorage.getItem('al')||sessionStorage.setItem('al','1');}catch(e){}
setTimeout(endIntro,RM?0:1500);
/* nav */
$('.links').innerHTML=CONFIG.nav.map(([i,t])=>`<a href="#${i}" data-s="${i}">${t}</a>`).join('');
const mm=$('#mm');mm.insertAdjacentHTML('beforeend',CONFIG.nav.map(([i,t],k)=>`<a href="#${i}" style="--i:${k}">${t}</a>`).join(''));
$('#fl').innerHTML=CONFIG.nav.map(([i,t])=>`<a href="#${i}">${t}</a>`).join('');
const bg=$('#bg');
const setMM=o=>{mm.classList.toggle('open',o);bg.setAttribute('aria-expanded',o);document.body.style.overflow=o?'hidden':'';if(o)$('#mx').focus();else if(document.activeElement.closest('#mm'))bg.focus()};
bg.onclick=()=>setMM(true);$('#mx').onclick=()=>setMM(false);$$('#mm a').forEach(a=>a.onclick=()=>setMM(false));
addEventListener('scroll',()=>{$('#hd').classList.toggle('sc',scrollY>40);$('#top').classList.toggle('show',scrollY>700)},{passive:true});
$('#top').onclick=()=>scrollTo({top:0});
const so=new IntersectionObserver(es=>es.forEach(e=>{if(e.isIntersecting)$$('.links a').forEach(a=>a.classList.toggle('on',a.dataset.s===e.target.id))}),{rootMargin:'-45% 0px -50% 0px'});
CONFIG.nav.forEach(([i])=>so.observe($('#'+i)));
/* marquee */
const mt="GERÇEK LEZZET • ADANA RUHU • SICAK SOFRA • TÜRK MUTFAĞI • ";
$('#mq').innerHTML=`<span>${mt.repeat(4)}</span><span>${mt.repeat(4)}</span>`;
/* menu */
let cat=0;const tabs=$('#tabs'),grid=$('#grid');
tabs.innerHTML=CONFIG.cats.map((c,i)=>`<button role="tab" id="t${i}" aria-selected="${i===0}" tabindex="${i===0?0:-1}">${c}</button>`).join('');
function renderMenu(){
 const its=CONFIG.items.filter(x=>x.c===cat);
 grid.setAttribute('aria-labelledby','t'+cat);
 grid.innerHTML=its.length?its.map((x,i)=>`<button class="card" style="--i:${i}" data-n="${CONFIG.items.indexOf(x)}"><div class="ph" style="--h:${x.h}"><i></i></div><div class="cb"><h3>${x.n}</h3><p>${x.d}</p><span class="price">${x.p?x.p:PRICE_NA}</span></div></button>`).join(''):`<p class="mut">Bu kategori için ürünler yakında eklenecek.</p>`;
}
const pick=i=>{cat=i;$$('button',tabs).forEach((b,k)=>{b.setAttribute('aria-selected',k===i);b.tabIndex=k===i?0:-1});renderMenu()};
tabs.onclick=e=>{const b=e.target.closest('button');if(b)pick($$('button',tabs).indexOf(b))};
tabs.onkeydown=e=>{const n=CONFIG.cats.length;let i=cat;if(e.key==='ArrowRight')i=(cat+1)%n;else if(e.key==='ArrowLeft')i=(cat+n-1)%n;else return;pick(i);$$('button',tabs)[i].focus();e.preventDefault()};
grid.onclick=e=>{const c=e.target.closest('.card');if(!c)return;const x=CONFIG.items[c.dataset.n];$('#dt').textContent=x.n;$('#dd').textContent=x.d;$('#dp').textContent=x.p||PRICE_NA;$('#dlg').showModal()};
$('#dc').onclick=()=>$('#dlg').close();
renderMenu();
/* gallery + lightbox */
const gal=$('#gal'),lb=$('#lb');let gi=0,lastF;
gal.innerHTML=CONFIG.gallery.map(([c,h],i)=>`<button style="--h:${h}" data-i="${i}" aria-label="${c} — büyüt"><span>${c}</span></button>`).join('');
const showLB=i=>{gi=(i+CONFIG.gallery.length)%CONFIG.gallery.length;const [c,h]=CONFIG.gallery[gi];const f=$('#li');f.style.background=`radial-gradient(circle,hsl(${h} 65% 50%),hsl(${h} 55% 18%))`;f.textContent=c+' (yer tutucu görsel)'};
const openLB=i=>{lastF=document.activeElement;showLB(i);lb.classList.add('open');document.body.style.overflow='hidden';$('.c',lb).focus()};
const closeLB=()=>{lb.classList.remove('open');document.body.style.overflow='';lastF&&lastF.focus()};
gal.onclick=e=>{const b=e.target.closest('button');if(b)openLB(+b.dataset.i)};
$('.c',lb).onclick=closeLB;$('.p',lb).onclick=()=>showLB(gi-1);$('.n',lb).onclick=()=>showLB(gi+1);
lb.onclick=e=>{if(e.target===lb)closeLB()};
let tx=0;lb.addEventListener('touchstart',e=>tx=e.touches[0].clientX,{passive:true});
lb.addEventListener('touchend',e=>{const d=e.changedTouches[0].clientX-tx;if(Math.abs(d)>50)showLB(gi+(d<0?1:-1))});
addEventListener('keydown',e=>{
 if(e.key==='Escape'){if(lb.classList.contains('open'))closeLB();if(mm.classList.contains('open'))setMM(false)}
 if(lb.classList.contains('open')){if(e.key==='ArrowRight')showLB(gi+1);if(e.key==='ArrowLeft')showLB(gi-1)}
});
/* contact config: disable anything unconfigured, never output a broken link */
$$('.cfg').forEach(a=>{
 const k=a.dataset.k,v=CONFIG[k];
 if(v){a.href=a.dataset.w?`https://wa.me/${v}?text=${encodeURIComponent(CONFIG.waText)}`:(a.dataset.p||'')+v;a.removeAttribute('aria-disabled')}
 else{a.removeAttribute('href');a.setAttribute('aria-disabled','true');a.removeAttribute('target')}
});
const NOTES={mapsUrl:"Harita bağlantısı henüz eklenmedi.",phone:"İletişim bilgileri henüz eklenmedi."};
$$('.cfg-n').forEach(n=>{if(!CONFIG[n.dataset.k])n.textContent=NOTES[n.dataset.k]});
$('#adr').textContent=CONFIG.address||"Adres henüz eklenmedi.";
$('#tel').textContent=CONFIG.phone||"Telefon henüz eklenmedi.";
$('#hrs').innerHTML=CONFIG.hours.length?CONFIG.hours.map(h=>`${h.d}: ${h.t}`).join('<br>'):"Çalışma saatleri henüz eklenmedi.";
if(CONFIG.mapsUrl)$('#mapnote').innerHTML=`<a href="${CONFIG.mapsUrl}" target="_blank" rel="noopener">Haritada aç</a>`;
$('#yr').textContent=new Date().getFullYear();
/* reveals + rating */
const io=new IntersectionObserver(es=>es.forEach(e=>{if(e.isIntersecting){e.target.classList.add('in');io.unobserve(e.target)}}),{threshold:.2});
$$('.rv').forEach(r=>io.observe(r));
const rio=new IntersectionObserver(es=>es.forEach(e=>{if(e.isIntersecting){$('#fill').style.width='72%';rio.disconnect()}}),{threshold:.5});
rio.observe($('#rate'));
/* hero parallax (desktop pointer only) */
if(!RM&&matchMedia('(hover:hover) and (min-width:821px)').matches){const a=$('#art');$('.hero').addEventListener('mousemove',e=>{const x=(e.clientX/innerWidth-.5)*14,y=(e.clientY/innerHeight-.5)*14;a.style.transform=`translate(${x}px,${y}px)`})}
/* disabled anchors must not scroll */
document.addEventListener('click',e=>{const a=e.target.closest('a[aria-disabled=true]');if(a)e.preventDefault()});
</script>
</body>
</html>