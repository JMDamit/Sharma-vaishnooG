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
      font-size
