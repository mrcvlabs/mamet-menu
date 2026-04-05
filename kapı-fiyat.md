<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mamet Kebap - Fiyat Listesi</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=Noto+Sans:wght@400;600;700&family=Amiri:wght@400;700&display=swap');

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    background: #f5e6c8;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    padding: 20px;
    font-family: 'Noto Sans', Arial, sans-serif;
  }

  .menu-container {
    width: 700px;
    max-width: 100%;
    background: linear-gradient(135deg, #fdf6e3 0%, #f7eed5 50%, #fdf6e3 100%);
    position: relative;
    padding: 50px 40px;
  }

  /* Dis cerceve - Urfa kilim/bakir motifli */
  .menu-container::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    border: 12px solid #8B1A1A;
    background: transparent;
    pointer-events: none;
  }

  .menu-container::after {
    content: '';
    position: absolute;
    top: 6px; left: 6px; right: 6px; bottom: 6px;
    border: 3px solid #D4A017;
    pointer-events: none;
  }

  /* Ic cerceve */
  .inner-frame {
    border: 2px solid #8B1A1A;
    padding: 30px 25px;
    position: relative;
  }

  .inner-frame::before {
    content: '';
    position: absolute;
    top: 4px; left: 4px; right: 4px; bottom: 4px;
    border: 1px solid #D4A017;
    pointer-events: none;
  }

  /* Kose suslemeleri */
  .corner {
    position: absolute;
    width: 30px;
    height: 30px;
    border-color: #D4A017;
    z-index: 2;
  }
  .corner-tl { top: 14px; left: 14px; border-top: 3px solid; border-left: 3px solid; }
  .corner-tr { top: 14px; right: 14px; border-top: 3px solid; border-right: 3px solid; }
  .corner-bl { bottom: 14px; left: 14px; border-bottom: 3px solid; border-left: 3px solid; }
  .corner-br { bottom: 14px; right: 14px; border-bottom: 3px solid; border-right: 3px solid; }

  /* Ust motif - Urfa tarzi geometrik desen */
  .top-ornament {
    text-align: center;
    color: #8B1A1A;
    font-size: 18px;
    letter-spacing: 6px;
    margin-bottom: 8px;
  }

  /* Baslik */
  .restaurant-name {
    text-align: center;
    font-family: 'Amiri', 'Playfair Display', serif;
    font-size: 42px;
    font-weight: 900;
    color: #8B1A1A;
    text-shadow: 1px 1px 2px rgba(139, 26, 26, 0.2);
    margin-bottom: 2px;
    letter-spacing: 3px;
  }

  .subtitle {
    text-align: center;
    font-family: 'Amiri', serif;
    font-size: 16px;
    color: #A0522D;
    letter-spacing: 8px;
    text-transform: uppercase;
    margin-bottom: 5px;
  }

  .divider {
    text-align: center;
    color: #D4A017;
    font-size: 16px;
    letter-spacing: 4px;
    margin: 8px 0;
  }

  .divider-line {
    border: none;
    height: 2px;
    background: linear-gradient(90deg, transparent, #D4A017, #8B1A1A, #D4A017, transparent);
    margin: 10px 0;
  }

  /* Kategori */
  .category {
    margin-bottom: 14px;
  }

  .category-title {
    font-family: 'Amiri', 'Playfair Display', serif;
    font-size: 20px;
    font-weight: 700;
    color: #8B1A1A;
    text-align: center;
    margin-bottom: 6px;
    letter-spacing: 2px;
    position: relative;
  }

  .category-title::before,
  .category-title::after {
    content: '~';
    margin: 0 8px;
    color: #D4A017;
  }

  /* Menu ogesi */
  .menu-item {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    padding: 2px 5px;
    font-size: 14px;
  }

  .menu-item:nth-child(even) {
    background: rgba(212, 160, 23, 0.06);
  }

  .item-name {
    font-weight: 600;
    color: #3e2723;
    flex-shrink: 0;
  }

  .item-dots {
    flex-grow: 1;
    border-bottom: 1px dotted #c9a96e;
    margin: 0 6px;
    min-width: 20px;
    height: 12px;
  }

  .item-price {
    font-weight: 700;
    color: #8B1A1A;
    white-space: nowrap;
    font-size: 14px;
  }

  /* Alt kisim */
  .footer {
    text-align: center;
    margin-top: 12px;
    font-family: 'Amiri', serif;
    font-size: 13px;
    color: #A0522D;
    font-style: italic;
    letter-spacing: 1px;
  }

  .bottom-ornament {
    text-align: center;
    color: #8B1A1A;
    font-size: 14px;
    letter-spacing: 6px;
    margin-top: 8px;
  }

  /* Baski icin */
  @media print {
    body { background: white; padding: 0; }
    .menu-container { 
      width: 100%; 
      box-shadow: none;
      page-break-inside: avoid;
    }
  }
</style>
</head>
<body>

<div class="menu-container">
  <div class="corner corner-tl"></div>
  <div class="corner corner-tr"></div>
  <div class="corner corner-bl"></div>
  <div class="corner corner-br"></div>

  <div class="inner-frame">

    <div class="top-ornament">&#9670; &#9674; &#9670; &#9674; &#9670;</div>

    <div class="restaurant-name">MAMET KEBAP</div>
    <div class="subtitle">Urfa Mutfagi</div>

    <div class="divider">&#10040; &#10040; &#10040;</div>
    <hr class="divider-line">

    <!-- Kebap Cesitleri -->
    <div class="category">
      <div class="category-title">Kebap Cesitleri</div>
      <div class="menu-item"><span class="item-name">Adana Kebab</span><span class="item-dots"></span><span class="item-price">430 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Urfa Kebab</span><span class="item-dots"></span><span class="item-price">430 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Tavuk Sis</span><span class="item-dots"></span><span class="item-price">380 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kanat Izgara</span><span class="item-dots"></span><span class="item-price">380 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Alinazik Kebab</span><span class="item-dots"></span><span class="item-price">520 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Alti Ezmeli Kebab</span><span class="item-dots"></span><span class="item-price">520 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Ciger Sis</span><span class="item-dots"></span><span class="item-price">520 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Domatesli Kebab</span><span class="item-dots"></span><span class="item-price">520 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kuzu Pirzola</span><span class="item-dots"></span><span class="item-price">750 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kuzu Sis Kebab</span><span class="item-dots"></span><span class="item-price">520 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Lokum Sis Kebab</span><span class="item-dots"></span><span class="item-price">750 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Patlicanli Kebab</span><span class="item-dots"></span><span class="item-price">520 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Vali Kebabi (1 Kisilik)</span><span class="item-dots"></span><span class="item-price">900 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Yogurtlu Kebab</span><span class="item-dots"></span><span class="item-price">520 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Sis Beyti Kebab</span><span class="item-dots"></span><span class="item-price">520 &#8378;</span></div>
    </div>

    <hr class="divider-line">

    <!-- Durum Cesitleri -->
    <div class="category">
      <div class="category-title">Durum Cesitleri</div>
      <div class="menu-item"><span class="item-name">Adana Durum</span><span class="item-dots"></span><span class="item-price">250 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Ciger Durum</span><span class="item-dots"></span><span class="item-price">300 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kuzu Durum</span><span class="item-dots"></span><span class="item-price">300 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Tavuk Durum</span><span class="item-dots"></span><span class="item-price">200 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Urfa Durum</span><span class="item-dots"></span><span class="item-price">250 &#8378;</span></div>
    </div>

    <hr class="divider-line">

    <!-- Pide Cesitleri -->
    <div class="category">
      <div class="category-title">Pide Cesitleri</div>
      <div class="menu-item"><span class="item-name">Karisik Pide</span><span class="item-dots"></span><span class="item-price">380 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kasarli Pide</span><span class="item-dots"></span><span class="item-price">300 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kasarli-Yumurtali Pide</span><span class="item-dots"></span><span class="item-price">350 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kusbasili Pide</span><span class="item-dots"></span><span class="item-price">340 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kusbasili-Kasarli Pide</span><span class="item-dots"></span><span class="item-price">360 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kiymali Pide</span><span class="item-dots"></span><span class="item-price">330 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kiymali-Kasarli Pide</span><span class="item-dots"></span><span class="item-price">350 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Sebzeli-Kasarli Pide</span><span class="item-dots"></span><span class="item-price">360 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Sucuklu-Kasarli Pide</span><span class="item-dots"></span><span class="item-price">360 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kasarli Cantik</span><span class="item-dots"></span><span class="item-price">120 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kusbasili Cantik</span><span class="item-dots"></span><span class="item-price">130 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Kiymali Cantik</span><span class="item-dots"></span><span class="item-price">120 &#8378;</span></div>
    </div>

    <hr class="divider-line">

    <!-- Lahmacun Cesitleri -->
    <div class="category">
      <div class="category-title">Lahmacun Cesitleri</div>
      <div class="menu-item"><span class="item-name">Acili Lahmacun</span><span class="item-dots"></span><span class="item-price">140 &#8378;</span></div>
      <div class="menu-item"><span class="item-name">Acisiz Lahmacun</span><span class="item-dots"></span><span class="item-price">140 &#8378;</span></div>
    </div>

    <hr class="divider-line">

    <!-- Corba, Tatli, Icecek - yan yana -->
    <div style="display: flex; gap: 20px;">
      <div class="category" style="flex: 1;">
        <div class="category-title">Corbalar</div>
        <div class="menu-item"><span class="item-name">Ezogelin</span><span class="item-dots"></span><span class="item-price">100 &#8378;</span></div>
        <div class="menu-item"><span class="item-name">Mercimek</span><span class="item-dots"></span><span class="item-price">100 &#8378;</span></div>
      </div>
      <div class="category" style="flex: 1;">
        <div class="category-title">Tatli</div>
        <div class="menu-item"><span class="item-name">Fistikli Baklava</span><span class="item-dots"></span><span class="item-price">200 &#8378;</span></div>
      </div>
    </div>

    <hr class="divider-line">

    <!-- Icecek Cesitleri -->
    <div class="category">
      <div class="category-title">Icecek Cesitleri</div>
      <div style="display: flex; gap: 15px;">
        <div style="flex: 1;">
          <div class="menu-item"><span class="item-name">Acik Ayran</span><span class="item-dots"></span><span class="item-price">70 &#8378;</span></div>
          <div class="menu-item"><span class="item-name">Buyuk Ayran</span><span class="item-dots"></span><span class="item-price">50 &#8378;</span></div>
          <div class="menu-item"><span class="item-name">Kucuk Ayran</span><span class="item-dots"></span><span class="item-price">40 &#8378;</span></div>
          <div class="menu-item"><span class="item-name">Salgam</span><span class="item-dots"></span><span class="item-price">70 &#8378;</span></div>
          <div class="menu-item"><span class="item-name">Sira</span><span class="item-dots"></span><span class="item-price">80 &#8378;</span></div>
          <div class="menu-item"><span class="item-name">Su</span><span class="item-dots"></span><span class="item-price">20 &#8378;</span></div>
        </div>
        <div style="flex: 1;">
          <div class="menu-item"><span class="item-name">Kola</span><span class="item-dots"></span><span class="item-price">70 &#8378;</span></div>
          <div class="menu-item"><span class="item-name">Fanta</span><span class="item-dots"></span><span class="item-price">70 &#8378;</span></div>
          <div class="menu-item"><span class="item-name">Gazoz</span><span class="item-dots"></span><span class="item-price">70 &#8378;</span></div>
          <div class="menu-item"><span class="item-name">Soda</span><span class="item-dots"></span><span class="item-price">40 &#8378;</span></div>
          <div class="menu-item"><span class="item-name">Meyve Suyu</span><span class="item-dots"></span><span class="item-price">70 &#8378;</span></div>
        </div>
      </div>
    </div>

    <hr class="divider-line">

    <div class="footer">Afiyet olsun!</div>
    <div class="bottom-ornament">&#9670; &#9674; &#9670; &#9674; &#9670;</div>

  </div>
</div>

</body>
</html>
