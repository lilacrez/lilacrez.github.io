<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>iPhone Projem</title>
  
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif; user-select: none; }
    body { background: #121212; display: flex; justify-content: center; align-items: center; height: 100vh; }

    /* iPhone Kasası */
    .iphone {
      width: 340px; height: 700px;
      background: linear-gradient(135deg, #1e3c72 0%, #2a5298 50%, #ff758c 100%);
      border: 12px solid #222; border-radius: 50px;
      box-shadow: 0 25px 50px rgba(0,0,0,0.8), inset 0 0 0 2px #555;
      position: relative; overflow: hidden; display: flex; flex-direction: column;
    }

    /* Üst Bar & Dynamic Island */
    .status-bar { display: flex; justify-content: space-between; align-items: center; padding: 14px 24px 5px; color: white; font-size: 13px; font-weight: 600; z-index: 10; }
    .dynamic-island { width: 95px; height: 26px; background: #000; border-radius: 20px; }

    /* Kaydırılabilir Ana Ekran Sayfaları */
    .screens-container {
      display: flex; flex: 1; overflow-x: auto; scroll-snap-type: x mandatory;
      scroll-behavior: smooth; scrollbar-width: none;
    }
    .screens-container::-webkit-scrollbar { display: none; }

    .screen {
      min-width: 100%; height: 100%; scroll-snap-align: start;
      padding: 25px 20px; display: grid; grid-template-columns: repeat(4, 1fr);
      grid-auto-rows: 85px; gap: 15px; align-content: start;
    }

    /* Uygulama İkonları */
    .app { display: flex; flex-direction: column; align-items: center; cursor: pointer; transition: transform 0.15s; }
    .app:active { transform: scale(0.88); }
    .app-icon {
      width: 56px; height: 56px; border-radius: 14px; display: flex;
      justify-content: center; align-items: center; font-size: 26px;
      background: rgba(255,255,255,0.9); box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }
    .app-name { color: white; font-size: 11px; margin-top: 5px; text-shadow: 0 1px 3px rgba(0,0,0,0.6); }

    /* Alt Dock */
    .dock {
      margin: 0 15px 15px; padding: 12px; background: rgba(255, 255, 255, 0.25);
      backdrop-filter: blur(15px); border-radius: 28px; display: flex; justify-content: space-around;
    }

    /* Açılan Uygulama Penceresi */
    .app-window {
      position: absolute; top: 0; left: 0; width: 100%; height: 100%;
      background: #fff; z-index: 20; display: none; flex-direction: column;
      animation: openApp 0.25s ease-out;
    }
    @keyframes openApp { from { transform: scale(0.8); opacity: 0; } to { transform: scale(1); opacity: 1; } }
    .app-header { padding: 45px 20px 15px; background: #f2f2f7; font-weight: bold; font-size: 22px; border-bottom: 1px solid #ddd; }
    .app-content { padding: 20px; flex: 1; font-size: 15px; color: #333; }

    /* Alt Ana Ekran Çizgisi (Home Bar) */
    .home-bar-area { position: absolute; bottom: 0; width: 100%; height: 25px; display: flex; justify-content: center; align-items: center; z-index: 30; cursor: pointer; }
    .home-bar { width: 120px; height: 5px; background: rgba(255,255,255,0.8); border-radius: 10px; }
    .app-window.active ~ .home-bar-area .home-bar { background: #000; }
  </style>
</head>
<body>

<div class="iphone">
  <!-- Üst Bilgi Çubuğu -->
  <div class="status-bar">
    <span id="clock">12:00</span>
    <div class="dynamic-island"></div>
    <span>5G 🔋</span>
  </div>

  <!-- Kaydırılabilir Ekranlar -->
  <div class="screens-container">
    <!-- 1. Sayfa -->
    <div class="screen">
      <div class="app" onclick="openApp('Notlar', 'Buraya kendi notlarını yazabilirsin.')">
        <div class="app-icon" style="background:#ffcc00;">📝</div>
        <span class="app-name">Notlar</span>
      </div>
      <div class="app" onclick="openApp('Hakkımda', 'Merhaba, bu benim iPhone projem!')">
        <div class="app-icon" style="background:#34c759;">👤</div>
        <span class="app-name">Profil</span>
      </div>
      <div class="app" onclick="openApp('Mesajlar', 'Burada mesajlaşma ekranı olacak.')">
        <div class="app-icon" style="background:#30d158;">💬</div>
        <span class="app-name">Mesajlar</span>
      </div>
      <div class="app" onclick="openApp('Ayarlar', 'iOS Web Sürümü 1.0')">
        <div class="app-icon" style="background:#8e8e93;">⚙️</div>
        <span class="app-name">Ayarlar</span>
      </div>
    </div>
  </div>

  <!-- Alt Sabit Menü (Dock) -->
  <div class="dock">
    <div class="app" onclick="openApp('Telefon', 'Arama ekranı')">
      <div class="app-icon" style="background:#34c759; margin:0;">📞</div>
    </div>
    <div class="app" onclick="openApp('Safari', 'İnternet tarayıcısı')">
      <div class="app-icon" style="background:#007aff; margin:0;">🧭</div>
    </div>
  </div>

  <!-- Uygulama Penceresi -->
  <div class="app-window" id="appWindow">
    <div class="app-header" id="appTitle">Uygulama</div>
    <div class="app-content" id="appBody">İçerik</div>
  </div>

  <!-- Ana Ekrana Dönme Çizgisi -->
  <div class="home-bar-area" onclick="closeApp()">
    <div class="home-bar"></div>
  </div>
</div>

<script>
  // Saati canlı güncelle
  function updateClock() {
    const now = new Date();
    document.getElementById('clock').innerText = now.toTimeString().slice(0, 5);
  }
  setInterval(updateClock, 1000);
  updateClock();

  // Uygulama açma ve kapatma
  function openApp(title, content) {
    document.getElementById('appTitle').innerText = title;
    document.getElementById('appBody').innerText = content;
    const win = document.getElementById('appWindow');
    win.style.display = 'flex';
    win.classList.add('active');
  }

  function closeApp() {
    const win = document.getElementById('appWindow');
    win.style.display = 'none';
    win.classList.remove('active');
  }
</script>

</body>
</html>
