<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Sharma Vaishnoo Menu</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <style>
    :root {
      --bg: #f5eee6;
      --card: #ffffff;
      --primary: #c0392b;
      --primary-soft: rgba(192, 57, 43, 0.08);
      --accent: #f4d03f;
      --text-main: #2c3e50;
      --text-muted: #7f8c8d;
      --border-soft: #ecdcd0;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI",
        Roboto, sans-serif;
      background: radial-gradient(circle at top, #ffe9c7 0, #f5eee6 40%, #f0e4da 100%);
      color: var(--text-main);
      min-height: 100vh;
      padding: 16px;
      display: flex;
      justify-content: center;
    }

    .page {
      width: 100%;
      max-width: 900px;
    }

    .brand-card {
      background: linear-gradient(135deg, #c0392b, #8e2a21);
      border-radius: 20px;
      padding: 18px 20px;
      box-shadow: 0 14px 30px rgba(0, 0, 0, 0.25);
      color: #fff;
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      margin-bottom: 16px;
    }

    .brand-left {
      display: flex;
      flex-direction: column;
      gap: 4px;
    }

    .logo-circle {
      width: 52px;
      height: 52px;
      border-radius: 50%;
      border: 2px solid rgba(255, 255, 255, 0.7);
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 800;
      font-size: 20px;
      margin-bottom: 6px;
      background: rgba(0, 0, 0, 0.12);
    }

    .brand-name {
      font-size: 24px;
      font-weight: 800;
      letter-spacing: 2px;
      text-transform: uppercase;
    }

    .brand-tagline {
      font-size: 13px;
      opacity: 0.9;
    }

    .brand-right {
      display: flex;
      flex-direction: column;
      gap: 6px;
      align-items: flex-end;
      min-width: 160px;
    }

    .chip-row {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      justify-content: flex-end;
    }

    .chip {
      font-size: 11px;
      padding: 4px 8px;
      border-radius: 999px;
      background: rgba(255, 255, 255, 0.15);
      border: 1px solid rgba(255, 255, 255, 0.3);
      backdrop-filter: blur(4px);
      white-space: nowrap;
    }

    .last-updated {
      font-size: 11px;
      opacity: 0.85;
    }

    .menu-card {
      background: var(--card);
      border-radius: 20px;
      padding: 16px 18px 20px;
      box-shadow: 0 10px 26px rgba(0, 0, 0, 0.12);
      border: 1px solid var(--border-soft);
      backdrop-filter: blur(6px);
    }

    .menu-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 10px;
      margin-bottom: 10px;
      padding-bottom: 8px;
      border-bottom: 1px dashed var(--border-soft);
    }

    .menu-title {
      font-size: 18px;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 1.5px;
      display: flex;
      align-items: center;
      gap: 6px;
    }

    .veg-dot {
      width: 12px;
      height: 12px;
      border-radius: 3px;
      border: 2px solid #2ecc71;
      position: relative;
      display: inline-block;
    }

    .veg-dot::after {
      content: "";
      position: absolute;
      inset: 2px;
      background: #2ecc71;
    }

    .mini-note {
      font-size: 11px;
      color: var(--text-muted);
      text-align: right;
    }

    .section {
      margin-top: 14px;
      padding: 10px 10px 12px;
      border-radius: 14px;
      background: linear-gradient(
        135deg,
        rgba(255, 255, 255, 0.9),
        rgba(252, 243, 230, 0.9)
      );
      border: 1px solid rgba(255, 255, 255, 0.7);
    }

    .section-header {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      margin-bottom: 6px;
    }

    .section-title {
      font-size: 15px;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    .section-subtitle {
      font-size: 11px;
      color: var(--text-muted);
    }

    .item-row {
      display: flex;
      justify-content: space-between;
      gap: 10px;
      padding: 4px 0;
      border-bottom: 1px dotted rgba(0, 0, 0, 0.06);
    }

    .item-row:last-child {
      border-bottom: none;
      padding-bottom: 0;
    }

    .item-left {
      max-width: 70%;
    }

    .item-name {
      font-size: 14px;
      font-weight: 600;
    }

    .item-note {
      font-size: 11px;
      color: var(--text-muted);
    }

    .item-price {
      font-size: 13px;
      font-weight: 700;
      white-space: nowrap;
    }

    .footer-note {
      margin-top: 12px;
      font-size: 11px;
      color: var(--text-muted);
      text-align: center;
    }

    .footer-note strong {
      color: var(--primary);
    }

    @media (max-width: 560px) {
      body {
        padding: 10px;
      }
      .brand-card {
        padding: 14px;
      }
      .menu-card {
        padding: 12px 12px 16px;
      }
      .brand-right {
        align-items: flex-start;
      }
      .menu-header {
        flex-direction: column;
        align-items: flex-start;
      }
      .mini-note {
        text-align: left;
      }
    }
  </style>
</head>
<body>
  <div class="page">
    <!-- Top red brand header -->
    <header class="brand-card">
      <div class="brand-left">
        <div class="logo-circle">SV</div>
        <div class="brand-name">Sharma Vaishnoo</div>
        <div class="brand-tagline">Fresh · Desi · Family Dhaba</div>
      </div>
      <div class="brand-right">
        <div class="chip-row">
          <span class="chip">Pure Veg</span>
          <span class="chip">Home-style Taste</span>
          <span class="chip">Packed & Dine-in</span>
        </div>
        <div class="last-updated">
          Menu last updated: <strong>10 Dec 2025</strong>
        </div>
      </div>
    </header>

    <!-- White menu card -->
    <main class="menu-card">
      <div class="menu-header">
        <div class="menu-title">
          <span class="veg-dot"></span>
          <span>MAIN MENU</span>
        </div>
        <div class="mini-note">
          Rates in INR · Half / Full where mentioned
        </div>
      </div>

      <!-- Paneer Section -->
      <section class="section">
        <div class="section-header">
          <div class="section-title">Paneer Dishes</div>
          <div class="section-subtitle">Half / Full</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Kadhai Paneer</div>
          </div>
          <div class="item-price">₹ 90 / 180</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Paneer Butter Masala</div>
          </div>
          <div class="item-price">₹ 90 / 180</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Paneer Bhujiya</div>
          </div>
          <div class="item-price">₹ 100 / 200</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Shahi Paneer</div>
          </div>
          <div class="item-price">₹ 70 / 140</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Matar Paneer</div>
          </div>
          <div class="item-price">₹ 70 / 140</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Palak Paneer</div>
          </div>
          <div class="item-price">₹ 70 / 140</div>
        </div>
      </section>

      <!-- Dal Section -->
      <section class="section">
        <div class="section-header">
          <div class="section-title">Dal & Gravies</div>
          <div class="section-subtitle">Half / Full</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Dal Makhni</div>
          </div>
          <div class="item-price">₹ 60 / 120</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Dal Fry</div>
          </div>
          <div class="item-price">₹ 50 / 100</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Rajma Masala</div>
          </div>
          <div class="item-price">₹ 60 / 110</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Chana Masala</div>
          </div>
          <div class="item-price">₹ 60 / 110</div>
        </div>
      </section>

      <!-- Breads Section -->
      <section class="section">
        <div class="section-header">
          <div class="section-title">Breads</div>
          <div class="section-subtitle">Per piece</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Tandoori Roti</div>
            <div class="item-note">Plain</div>
          </div>
          <div class="item-price">₹ 6</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Butter Roti</div>
          </div>
          <div class="item-price">₹ 7</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Aloo Naan</div>
          </div>
          <div class="item-price">₹ 25</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Butter Naan</div>
          </div>
          <div class="item-price">₹ 30</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Laccha Parantha</div>
          </div>
          <div class="item-price">₹ 25</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Paneer Parantha</div>
          </div>
          <div class="item-price">₹ 40</div>
        </div>
      </section>

      <!-- Rice Section -->
      <section class="section">
        <div class="section-header">
          <div class="section-title">Rice</div>
          <div class="section-subtitle">Half / Full</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Plain Rice</div>
          </div>
          <div class="item-price">₹ 30 / 60</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Rajma Chawal</div>
          </div>
          <div class="item-price">₹ 50 / 100</div>
        </div>

        <div class="item-row">
          <div class="item-left">
            <div class="item-name">Dal Chawal</div>
          </div>
          <div class="item-price">₹ 50 / 100</div>
        </div>
      </section>

      <p class="footer-note">
        Scan the QR code at table to open this menu on your phone.<br />
        <strong>Sharma Vaishnoo Dhabba</strong> · Taste that feels like home.
      </p>
    </main>
  </div>
</body>
</html>
