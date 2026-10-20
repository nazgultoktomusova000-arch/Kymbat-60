
<!DOCTYPE html>
<html lang="ky">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Кымбаттын 60 жаш мааракеси</title>

<link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Marck+Script&family=Cormorant+Garamond:wght@400;500;600&display=swap" rel="stylesheet">

<style>
*{box-sizing:border-box}
body{margin:0;background:#fff7e9;color:#79552f;font-family:'Cormorant Garamond',serif}
#envelope{position:fixed;inset:0;z-index:10;display:flex;align-items:center;justify-content:center;background:#f8e5c5;perspective:1200px;overflow:hidden}
.door{position:absolute;top:0;width:50%;height:100%;background-image:url('assets/01-envelope.jpeg');background-size:200% 100%;transition:transform 1.5s ease}
.left{left:0;background-position:left;transform-origin:left}
.right{right:0;background-position:right;transform-origin:right}
#envelope.open .left{transform:rotateY(-110deg)}
#envelope.open .right{transform:rotateY(110deg)}
.seal{z-index:2;border:5px double #fff0b0;border-radius:50%;width:145px;height:145px;background:radial-gradient(#f6df94,#b48129);color:white;font:30px 'Great Vibes',cursive;box-shadow:0 4px 20px #76501d66;cursor:pointer}
#envelope.open .seal{opacity:0;pointer-events:none}
.hint{position:absolute;bottom:8%;z-index:3;text-align:center;font-size:14px;letter-spacing:2px}
#site{display:none}
.page{position:relative;width:100%;max-width:700px;margin:auto;line-height:0}
.page img{display:block;width:100%;height:auto}
.text{position:absolute;inset:0;display:flex;align-items:center;justify-content:center;text-align:center;padding:10%;line-height:1.35}
.poem{font-size:clamp(14px,3.5vw,23px);font-weight:600;color:#785538}
.poem p{margin:9px 0}
.invite{font-size:clamp(15px,4vw,24px);color:#765333}
.script{font:clamp(36px,8vw,57px) 'Great Vibes',cursive;color:#aa7b32;line-height:1.1}
.details{padding-top:20%;align-items:flex-start;font-size:clamp(18px,4.5vw,27px);color:#805d32}
.details .script{font-size:clamp(43px,10vw,68px)}
.details p{margin:8px 0}
.address{font-size:.8em}
a.map{display:inline-block;padding:8px 16px;border:1px solid #b58b42;border-radius:24px;color:#79552f;text-decoration:none;line-height:1.2;font-size:16px}
.last{align-items:flex-end;padding-bottom:24%;font-size:clamp(17px,4vw,25px)}
.music{position:fixed;right:12px;top:12px;z-index:8;border:1px solid #b58b42;border-radius:25px;background:#fff9ed;color:#79552f;padding:10px 14px;display:none}
</style>
</head>
<body>

<div id="envelope">
  <div class="door left"></div>
  <div class="door right"></div>
  <button class="seal" onclick="openSite()">Кымбат<br>60 жаш</button>
  <div class="hint">ЧАКЫРУУНУ АЧУУ ҮЧҮН МӨӨРДҮ БАСЫҢЫЗ</div>
</div>

<audio id="music" src="assets/bek-borbiev.mp3" loop></audio>
<button class="music" id="musicBtn" onclick="toggleMusic()">♫ Музыканы токтотуу</button>

<main id="site">

<section class="page">
<img src="assets/02-yurt-poem.jpeg" alt="Кыргыз боз үйү">
<div class="text"><div class="poem">
<p>АЛЛАДАН НАСИП БОЛУП БАГЫБЫЗГА,</p>
<p>АР ЖЫЛЫ ЖАШ КОШУЛУП ЖАШЫБЫЗГА.</p>
<p>БУЙРУДУ УШУЛ КҮНҮ ЖАРАТКАНДАН,</p>
<p>АК ДАСТОРКОН ЖАЙЫЛЫП БААРЫБЫЗГА.</p>
<p>БАТАҢЫЗДАРДЫ БЕРҮҮНҮ СУРАНАБЫЗ,</p>
<p>КОНОК БОЛУП САЛТАНАТТУУ ТОЮБУЗДА!</p>
</div></div>
</section>

<section class="page">
<img src="assets/03-invitation.jpeg" alt="Кооз алтын алкак">
<div class="text"><div class="invite">
<div class="script">Биздин кадырлуу<br>конокторубуз!</div>
<p>СИЗДЕРДИ</p>
<p><b>КЫМБАТТЫН 60 ЖАШ КУТТУУ МААРАКЕСИНЕ</b></p>
<p>КЕЛИП, АК ДАСТОРКОНДО БАТА БЕРИП, КАДЫРЛУУ КОНОГУБУЗ БОЛУУГА ЧАКЫРАБЫЗ!</p>
<p><i>Сиздердин келишиңиздер — биз үчүн чоң кубаныч!</i></p>
</div></div>
</section>

<section class="page">
<img src="assets/04-details.jpeg" alt="Тойдун маалыматы">
<div class="text details"><div>
<div class="script">Кымбат</div>
<p><b>60 ЖАШ МААРАКЕСИ</b></p>
<p>📅 16.11.2026</p>
<p>🕓 Саат 16:00</p>
<p>📍 Ресторан «Алтын Арашан»</p>
<p>Бишкек шаары</p>
<p class="address">7-Апрель көчөсү, Алматинская тарапта, Ахунбаев шакекчесине жетпей, оң жакта.</p>
<a class="map" href="https://www.google.com/maps/search/?api=1&query=Алтын+Арашан+Бишкек" target="_blank">Картадан көрүү ↗</a>
</div></div>
</section>

<section class="page">
<img src="assets/05-blessing.jpeg" alt="Кыргыз элинин улуттук салты">
<div class="text last"><div>
<div class="script">Ак батаңыздарды<br>аябаңыздар!</div>
<p>Келип, кубанычыбызга ортоктош болуп, ак дасторкондон даам татып кетиңиздер.</p>
<p>Сиздерди чыдамсыздык менен күтөбүз!</p>
</div></div>
</section>
</main>

<script>
async function openSite(){
  const envelope=document.getElementById('envelope');
  envelope.classList.add('open');
  const music=document.getElementById('music');
  document.getElementById('musicBtn').style.display='block';
  try{await music.play()}catch(e){}
  setTimeout(()=>{
    envelope.style.display='none';
    document.getElementById('site').style.display='block';
  },1500);
}
async function toggleMusic(){
  const m=document.getElementById('music');
  const b=document.getElementById('musicBtn');
  if(m.paused){
    try{await m.play();b.textContent='♫ Музыканы токтотуу'}catch(e){}
  }else{
    m.pause();b.textContent='♫ Музыканы улантуу';
  }
}
</script>
</body>
</html>
