# https-github.com-openaiexamples-foryousayangg
<!doctype html>
<html lang="ms">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>For you sayanggkuhh Daniea 💖</title>
  <style>
    :root{
      --bg:#fff6fb;
      --card:#ffeef7;
      --accent:#ff6b9a;
      --text:#3b2b2b;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: "Helvetica Neue", Arial, sans-serif;
      background: linear-gradient(180deg,var(--bg),#fff);
      color:var(--text);
      display:flex;
      align-items:center;
      justify-content:center;
      min-height:100vh;
      padding:20px;
    }
    .card{
      width:100%;
      max-width:720px;
      background:var(--card);
      border-radius:18px;
      padding:28px;
      box-shadow:0 10px 30px rgba(0,0,0,0.08);
      text-align:center;
      position:relative;
      overflow:hidden;
    }
    h1{margin:0 0 8px;font-size:30px;color:var(--accent)}
    p{margin:0 0 18px;line-height:1.5}
    .heart{
      font-size:46px;
      display:inline-block;
      transform-origin:center;
      animation:beat 1s infinite;
    }
    @keyframes beat{
      0%{transform:scale(1)}
      50%{transform:scale(1.12)}
      100%{transform:scale(1)}
    }
    .photo{
      width:120px;height:120px;border-radius:50%;
      object-fit:cover;border:6px solid #fff;box-shadow:0 8px 20px rgba(0,0,0,0.12);
      margin:12px auto;
    }
    .btn{
      display:inline-block;
      margin-top:12px;
      padding:10px 18px;
      border-radius:12px;
      background:var(--accent);
      color:white;
      text-decoration:none;
      font-weight:600;
      cursor:pointer;
      box-shadow:0 6px 16px rgba(255,107,154,0.25);
    }
    footer{font-size:13px;color:#6b5353;margin-top:14px}
    /* small floating hearts */
    .confetti{
      position:absolute; inset:0; pointer-events:none;
    }
    .confetti span{
      position:absolute;
      font-size:18px;
      opacity:0.9;
      animation:float 4s linear infinite;
    }
    @keyframes float{
      0%{transform:translateY(0) rotate(0); opacity:1}
      100%{transform:translateY(-160px) rotate(360deg); opacity:0}
    }
    @media (max-width:420px){
      h1{font-size:24px}
      .card{padding:18px}
    }

    body {
      background: #ffeaf4;
      font-family: Arial, sans-serif;
      text-align: center;
      padding: 50px;
    }
    h1 {
      color: #ff4d88;
      font-size: 40px;
    }
    .photo {
      display: block;
      margin: 20px auto;
      width: 200px;
      height: 200px;
      object-fit: cover;
      border-radius: 60%; /* buat gambar jadi bulat */
      border: 6px solid #fff; /* bingkai putih */
      box-shadow: 0 8px 20px rgba(0,0,0,0.2); /* bayang lembut */
    }
  </style>
</head>
<body>
  <div class="card">
    <div class="confetti" aria-hidden="true">
      <span style="left:8%; top:85%;">💖</span>
      <span style="left:24%; top:90%;">🌸</span>
      <span style="left:42%; top:88%;">💗</span>
      <span style="left:62%; top:92%;">✨</span>
      <span style="left:78%; top:87%;">🌼</span>
    </div>

    <h1>For you sayanggg 💕💕💕</h1>
    <img src="gfgt.jpg" alt="" class="photo">
    <!-- Letakkan gambar jika nak — tukar src kepada nama fail gambar yang sama folder -->


    <p> Hi yayangggg <span class="heart">💓</span><br>
      Saya cuma na cakap,terima kasih sbb terima saya dalam hidup awak , saya tau awak masih dalam trauma,
      tpi izinkan saya untuk bawak awak keluar dari dari zon tu yee sayanggg. saya tau ,
      saya tk boleh na janji 100% untuk awak sembuh. tpi saya janji saya akan buat sehabis
      baik saya. terima kasihh sayanggg sbb bagi saya peluang untuk masuk ke hati awak.
      saya harap kita dapat capai apa yang kita impikan yee sayanggg . cuba awakk tekan button bawahh tuu hehe💖</p>

    <button class="btn" onclick="surprise()">tekann la yayangggg ✨</button>

    <audio id="audio" preload="auto">
      <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_3c2e0b4d0a.mp3?filename=happy-ambient-1084.mp3" type="audio/mpeg">
    </audio>

    <footer>— dari sapa lgi klu bkn bf awakk hehe ❤️</footer>
  </div>

  <script>
    function surprise(){
      // mainkan audio (jika browser benarkan)
      const a = document.getElementById('audio');
      a.play().catch(()=>{/* autoplay blocked, user must tap */});
      // buat mesej mudah
      alert("Love youu so muchhh sayangggg 💕❤️");
    }
    // buat animasi rawak untuk confetti hearts
    const spans = document.querySelectorAll('.confetti span');
    spans.forEach((el, i)=>{
      el.style.animationDelay = (i*0.5)+'s';
      el.style.fontSize = (14 + Math.round(Math.random()*18))+'px';
    });
  </script>
</body>
</html>
