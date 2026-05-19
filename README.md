<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>BLENDIX – Produktwebsite</title>

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:Arial,Helvetica,sans-serif
    }

    body{
      background:#fbfbfa;
      color:#0d2419
    }

    .container{
      width:min(1120px,88%);
      margin:auto
    }

    header{
      height:92px;
      display:flex;
      align-items:center;
      justify-content:space-between;
      background:#fff
    }

    .logo{
      font-size:34px;
      font-weight:900;
      letter-spacing:-1px;
      color:#0b2418
    }

    nav{
      display:flex;
      gap:58px;
      align-items:center;
      font-weight:700;
      font-size:15px
    }

    nav a{
      text-decoration:none;
      color:#111
    }

    .order{
      background:#0b2418;
      color:white;
      padding:16px 28px;
      border-radius:10px;
      display:flex;
      gap:10px;
      align-items:center;
      text-decoration:none;
      font-weight:800;
      box-shadow:0 6px 14px rgba(0,0,0,.12)
    }

    .hero-img{
      width:100%;
      display:block;
      border-radius:10px;
      margin:12px auto 0;
      box-shadow:0 8px 18px rgba(0,0,0,.05)
    }

    section{
      padding:36px 0
    }

    .title{
      text-align:center;
      font-size:28px;
      font-weight:900;
      letter-spacing:.5px;
      margin-bottom:8px
    }

    .line{
      width:70px;
      height:3px;
      background:#0b2418;
      margin:0 auto 18px
    }

    .subtitle{
      text-align:center;
      font-size:18px;
      margin-bottom:28px;
      color:#222
    }

    .products{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:22px
    }

    .card{
      background:white;
      border:1px solid #ddd;
      border-radius:10px;
      display:grid;
      grid-template-columns:42% 58%;
      align-items:center;
      min-height:295px;
      padding:28px;
      box-shadow:0 8px 20px rgba(0,0,0,.04)
    }

    .product-visual{
      height:350px;
      display:flex;
      align-items:center;
      justify-content:center
    }

    .product-img{
      max-height:350px;
      width:auto;
      object-fit:contain;
      display:block;
      margin:auto;
      filter:drop-shadow(0 10px 18px rgba(0,0,0,.18));
    }

    .card h3{
      font-size:26px;
      line-height:1.2;
      margin-bottom:18px;
      color:#0b2418
    }

    .checks{
      list-style:none;
      margin-bottom:22px;
      font-size:17px;
      line-height:1.85
    }

    .checks li:before{
      content:"✓";
      background:#0b2418;
      color:white;
      border-radius:50%;
      font-size:13px;
      margin-right:12px;
      padding:2px 5px
    }

    .price{
      font-size:42px;
      font-weight:900;
      color:#0b2418;
      display:inline-block;
      margin-right:28px
    }

    .price sup{
      font-size:24px
    }

    .buy{
      background:#0b2418;
      color:white;
      border:none;
      border-radius:7px;
      padding:13px 22px;
      font-weight:800;
      font-size:15px;
      cursor:pointer
    }

    .benefits{
      background:#fbf0df;
      border-radius:10px;
      display:grid;
      grid-template-columns:repeat(4,1fr);
      margin-top:20px;
      padding:28px 18px;
      text-align:center
    }

    .benefit{
      border-right:1px solid #d8cdbf;
      padding:0 22px
    }

    .benefit:last-child{
      border-right:none
    }

    .icon{
      font-size:34px;
      margin-bottom:10px
    }

    .benefit h4{
      font-size:15px;
      margin-bottom:8px
    }

    .benefit p{
      font-size:14px;
      line-height:1.45;
      color:#111
    }

    .about{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:62px;
      align-items:center;
      padding-bottom:55px
    }

    .gym-img{
      height:300px;
      border-radius:12px;
      overflow:hidden;
      display:flex;
      align-items:center;
      justify-content:center;
      background:#eee;
    }

    .gym-img img{
      width:100%;
      height:100%;
      object-fit:cover;
      display:block;
    }

    .about h2{
      font-size:30px;
      margin-bottom:10px
    }

    .about .small-line{
      width:55px;
      height:3px;
      background:#0b2418;
      margin-bottom:22px
    }

    .about p{
      font-size:17px;
      line-height:1.65;
      margin-bottom:28px;
      color:#111
    }

    .about-icons{
      display:grid;
      grid-template-columns:repeat(3,1fr);
      text-align:center;
      font-weight:800;
      font-size:14px
    }

    .about-icons div{
      font-size:36px
    }

    .about-icons span{
      display:block;
      font-size:14px;
      margin-top:8px
    }

    footer{
      background:linear-gradient(135deg,#0b2418,#173929);
      color:white;
      padding:42px 0 18px
    }

    .footer-grid{
      display:grid;
      grid-template-columns:1.5fr 1fr 1fr 1fr;
      gap:34px
    }

    .footer-logo{
      font-size:34px;
      font-weight:900
    }

    .footer-slogan{
      font-size:18px;
      font-weight:900;
      margin-top:8px
    }

    footer h4{
      font-size:14px;
      margin-bottom:14px
    }

    footer p,
    footer a{
      display:block;
      color:white;
      text-decoration:none;
      font-size:14px;
      line-height:1.8
    }

    .copy{
      text-align:center;
      border-top:1px solid rgba(255,255,255,.22);
      margin-top:30px;
      padding-top:18px;
      font-size:14px
    }

    @media(max-width:850px){

      nav{
        display:none
      }

      .products,
      .about,
      .footer-grid{
        grid-template-columns:1fr
      }

      .card{
        grid-template-columns:1fr;
        text-align:center
      }

      .benefits{
        grid-template-columns:1fr
      }

      .benefit{
        border-right:none;
        border-bottom:1px solid #d8cdbf;
        padding:18px
      }

      .benefit:last-child{
        border-bottom:none
      }

      .container{
        width:92%
      }
    }
  </style>
</head>

<body>

  <header class="container">
    <div class="logo">BLENDIX</div>

    <nav>
      <a href="#produkte">Produkte</a>
      <a href="#ueber">Über uns</a>
      <a href="#vorteile">Vorteile</a>
      <a href="#kontakt">Kontakt</a>
    </nav>

    <a class="order" href="#produkte">🛒 Jetzt bestellen</a>
  </header>

  <main>

    <div class="container">
      <img class="hero-img"
      src="./Silver and Blue Modern Soda Drink Presentation 4.jpg"
      alt="Blendix Werbebanner">
    </div>

    <section id="produkte" class="container">

      <h1 class="title">UNSERE PRODUKTE</h1>

      <div class="line"></div>

      <p class="subtitle">
        Hochwertige Shaker für deinen aktiven Lifestyle.
      </p>

      <div class="products">

        <div class="card">

          <div class="product-visual">
            <img src="./blendix-250ml.jpg"
            alt="Blendix Shaker 250ML"
            class="product-img">
          </div>

          <div>
            <h3>BLENDIX SHAKER<br>250ML</h3>

            <ul class="checks">
              <li>BPA-FREI</li>
              <li>Leicht & kompakt</li>
              <li>Auslaufsicher</li>
              <li>Perfekt für unterwegs</li>
            </ul>

            <div class="price">
              19<sup>99</sup>
            </div>

            <button class="buy">
              Jetzt kaufen
            </button>
          </div>

        </div>

        <div class="card">

          <div class="product-visual">
            <img src="./blendix-500ml.jpg"
            alt="Blendix Shaker 500ML"
            class="product-img">
          </div>

          <div>
            <h3>BLENDIX SHAKER<br>500ML</h3>

            <ul class="checks">
              <li>BPA-FREI</li>
              <li>Spülmaschinenfest</li>
              <li>Auslaufsicher</li>
              <li>Extra Volumen</li>
            </ul>

            <div class="price">
              29<sup>99</sup>
            </div>

            <button class="buy">
              Jetzt kaufen
            </button>
          </div>

        </div>

      </div>

      <div id="vorteile" class="benefits">

        <div class="benefit">
          <div class="icon">♧</div>
          <h4>BPA-FREI</h4>
          <p>Gesundheit steht bei uns an erster Stelle.</p>
        </div>

        <div class="benefit">
          <div class="icon">▣</div>
          <h4>SPÜLMASCHINENFEST</h4>
          <p>Einfach reinigen und mehr Zeit für dich.</p>
        </div>

        <div class="benefit">
          <div class="icon">♢</div>
          <h4>AUSLAUFSICHER</h4>
          <p>Kein Auslaufen, 100% sicher.</p>
        </div>

        <div class="benefit">
          <div class="icon">♤</div>
          <h4>HOCHWERTIG</h4>
          <p>Robustes Material für den Alltag.</p>
        </div>

      </div>

    </section>

    <section id="ueber" class="container about">

      <div class="gym-img">
        <img src="./blendix-gym.jpg"
        alt="Blendix Lifestyle">
      </div>

      <div>

        <h2>ÜBER BLENDIX</h2>

        <div class="small-line"></div>

        <p>
          BLENDIX steht für Qualität, Funktionalität und modernes Design.
          Unsere Shaker sind die perfekten Begleiter für Sport,
          Arbeit und Alltag. Mix deinen Erfolg – jeden Tag!
        </p>

        <div class="about-icons">

          <div>
            🏋️
            <span>Für Sport & Fitness</span>
          </div>

          <div>
            💼
            <span>Für Arbeit & Alltag</span>
          </div>

          <div>
            ♡
            <span>Für deinen Lifestyle</span>
          </div>

        </div>

      </div>

    </section>

  </main>

  <footer id="kontakt">

    <div class="container footer-grid">

      <div>
        <div class="footer-logo">BLENDIX</div>
        <div class="footer-slogan">
          MIX DEINEN ERFOLG
        </div>
      </div>

      <div>
        <h4>NAVIGATION</h4>

        <a href="#produkte">Produkte</a>
        <a href="#ueber">Über uns</a>
        <a href="#vorteile">Vorteile</a>
        <a href="#kontakt">Kontakt</a>
      </div>

      <div>
        <h4>KONTAKT</h4>

        <p>✉ info@shakerblendix.de</p>
        <p>☎ +49 176 12345678</p>
        <p>◎ @shakerblendix</p>
        <p>🌐 www.shakerblendix.de</p>
      </div>

      <div>
        <h4>FOLGE UNS</h4>

        <p style="font-size:30px">
          ◎ ♪
        </p>
      </div>

    </div>

    <div class="container copy">
      © 2026 BLENDIX – Alle Rechte vorbehalten.
    </div>

  </footer>

</body>
</html>
