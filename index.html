<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <title>VocabGacor</title>
  <link href="https://fonts.googleapis.com/css2?family=Instrument+Serif:ital@0;1&family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,600;1,9..40,300&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --bg: #f7f6f3;
      --surface: #ffffff;
      --border: #e8e4dd;
      --border-dark: #d4cec5;
      --ink: #1a1916;
      --ink-2: #5c5850;
      --ink-3: #9c9589;
      --accent: #2d6a4f;
      --accent-light: #52b788;
      --accent-bg: #f0faf5;
      --accent-border: #b7e4c7;
      --danger: #c1440e;
      --danger-bg: #fdf3ef;
      --danger-border: #f5c4b0;
      --gold: #b5860d;
      --gold-bg: #fdf8ec;
      --radius-sm: 8px;
      --radius-md: 14px;
      --radius-lg: 20px;
    }

    body {
      font-family: 'DM Sans', sans-serif;
      background: var(--bg);
      color: var(--ink);
      min-height: 100svh;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 0 16px 60px;
      position: relative;
      overflow-x: hidden;
    }

    /* Subtle background texture */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background-image:
        radial-gradient(circle at 15% 20%, rgba(82,183,136,0.06) 0%, transparent 50%),
        radial-gradient(circle at 85% 75%, rgba(45,106,79,0.05) 0%, transparent 50%);
      pointer-events: none;
      z-index: 0;
    }

    /* ===== HEADER ===== */
    .header {
      position: sticky;
      top: 0;
      z-index: 50;
      width: 100%;
      max-width: 480px;
      background: rgba(247,246,243,0.88);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      padding: 14px 0 12px;
      display: flex;
      flex-direction: column;
      gap: 12px;
    }

    .header-top {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .wordmark {
      font-family: 'Instrument Serif', serif;
      font-size: 22px;
      color: var(--ink);
      letter-spacing: -0.01em;
    }
    .wordmark em {
      font-style: italic;
      color: var(--accent);
    }

    .header-meta {
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .lang-pill {
      font-size: 11px;
      font-weight: 500;
      color: var(--ink-3);
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 99px;
      padding: 4px 10px;
      letter-spacing: 0.04em;
    }

    .combo-tag {
      font-size: 11px;
      font-weight: 600;
      color: var(--gold);
      background: var(--gold-bg);
      border: 1px solid #e8d08a;
      border-radius: 99px;
      padding: 4px 10px;
      letter-spacing: 0.02em;
      opacity: 0;
      transform: scale(0.85);
      transition: opacity 0.25s, transform 0.25s cubic-bezier(0.34,1.56,0.64,1);
    }
    .combo-tag.visible {
      opacity: 1;
      transform: scale(1);
    }
    .combo-tag.pop { animation: tagPop 0.3s ease; }
    @keyframes tagPop { 50% { transform: scale(1.12); } }

    /* Progress */
    .progress-wrap {
      display: flex;
      align-items: center;
      gap: 10px;
    }
    .progress-bar {
      flex: 1;
      height: 3px;
      background: var(--border);
      border-radius: 99px;
      overflow: hidden;
    }
    .progress-fill {
      height: 100%;
      background: linear-gradient(90deg, var(--accent), var(--accent-light));
      border-radius: 99px;
      transition: width 0.5s cubic-bezier(0.4,0,0.2,1);
    }
    .progress-label {
      font-size: 11px;
      font-weight: 500;
      color: var(--ink-3);
      min-width: 36px;
      text-align: right;
      letter-spacing: 0.03em;
    }

    /* ===== STATS ROW ===== */
    .stats-row {
      position: relative;
      z-index: 1;
      width: 100%;
      max-width: 480px;
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 8px;
      margin: 16px 0;
    }

    .stat {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius-md);
      padding: 14px 10px 12px;
      text-align: center;
    }

    .stat-label {
      font-size: 10px;
      font-weight: 500;
      color: var(--ink-3);
      letter-spacing: 0.08em;
      text-transform: uppercase;
      margin-bottom: 6px;
    }

    .stat-value {
      font-family: 'Instrument Serif', serif;
      font-size: 30px;
      line-height: 1;
      color: var(--ink);
      transition: color 0.2s;
    }
    .stat-value.green { color: var(--accent); }
    .stat-value.gold  { color: var(--gold); }

    .bump { animation: bumpAnim 0.35s cubic-bezier(0.34,1.56,0.64,1); }
    @keyframes bumpAnim { 0%{transform:scale(1)} 40%{transform:scale(1.22)} 100%{transform:scale(1)} }

    /* ===== CARD ===== */
    .card {
      position: relative;
      z-index: 1;
      width: 100%;
      max-width: 480px;
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius-lg);
      overflow: hidden;
      transition: border-color 0.3s, box-shadow 0.3s;
    }

    .card.correct {
      border-color: var(--accent-border);
      box-shadow: 0 0 0 4px rgba(82,183,136,0.08);
    }
    .card.wrong {
      border-color: var(--danger-border);
      box-shadow: 0 0 0 4px rgba(193,68,14,0.06);
    }

    /* Word area */
    .word-section {
      padding: 36px 24px 28px;
      text-align: center;
      border-bottom: 1px solid var(--border);
      position: relative;
      background: linear-gradient(180deg, #fafaf8 0%, var(--surface) 100%);
    }

    .word-caption {
      font-size: 10px;
      font-weight: 500;
      color: var(--ink-3);
      letter-spacing: 0.14em;
      text-transform: uppercase;
      margin-bottom: 14px;
    }

    #word {
      font-family: 'Instrument Serif', serif;
      font-size: clamp(34px, 10vw, 52px);
      line-height: 1.15;
      color: var(--ink);
      letter-spacing: -0.02em;
      word-wrap: break-word;
    }

    .word-enter { animation: wordEnter 0.4s cubic-bezier(0.16,1,0.3,1); }
    @keyframes wordEnter {
      from { opacity: 0; transform: translateY(-8px); filter: blur(3px); }
      to   { opacity: 1; transform: translateY(0);    filter: blur(0); }
    }

    /* Input section */
    .input-section {
      padding: 20px 20px 8px;
    }

    .input-label {
      font-size: 11px;
      font-weight: 500;
      color: var(--ink-3);
      letter-spacing: 0.06em;
      margin-bottom: 8px;
      display: block;
    }

    .input-wrapper {
      position: relative;
    }

    #answer {
      width: 100%;
      padding: 14px 44px 14px 16px;
      font-family: 'DM Sans', sans-serif;
      font-size: 15px;
      font-weight: 400;
      background: var(--bg);
      border: 1.5px solid var(--border-dark);
      border-radius: var(--radius-md);
      color: var(--ink);
      outline: none;
      transition: border-color 0.2s, box-shadow 0.2s, background 0.2s;
      caret-color: var(--accent);
      -webkit-appearance: none;
    }
    #answer::placeholder { color: var(--ink-3); font-weight: 300; }
    #answer:focus {
      border-color: var(--accent);
      background: var(--surface);
      box-shadow: 0 0 0 3px rgba(82,183,136,0.12);
    }
    #answer.correct-input {
      border-color: var(--accent) !important;
      background: var(--accent-bg) !important;
      color: var(--accent);
      box-shadow: 0 0 0 3px rgba(82,183,136,0.1) !important;
    }
    #answer.wrong-input {
      border-color: var(--danger) !important;
      background: var(--danger-bg) !important;
      color: var(--danger);
      box-shadow: 0 0 0 3px rgba(193,68,14,0.08) !important;
      animation: shake 0.32s ease;
    }
    @keyframes shake {
      0%,100%{ transform: translateX(0); }
      25%{ transform: translateX(-5px); }
      75%{ transform: translateX(5px); }
    }

    .input-icon {
      position: absolute;
      right: 14px;
      top: 50%;
      transform: translateY(-50%);
      width: 20px;
      height: 20px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      opacity: 0;
      transition: opacity 0.2s;
    }
    .input-icon.show { opacity: 1; }
    .input-icon.ok { background: var(--accent); }
    .input-icon.fail { background: var(--danger); }
    .input-icon svg { width: 11px; height: 11px; }

    /* Buttons */
    .btn-section {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
      padding: 16px 20px 20px;
    }

    button {
      font-family: 'DM Sans', sans-serif;
      font-size: 14px;
      font-weight: 500;
      border: none;
      border-radius: var(--radius-md);
      cursor: pointer;
      padding: 13px 16px;
      transition: all 0.18s ease;
      letter-spacing: 0.01em;
    }
    button:active { transform: scale(0.97); }

    .btn-primary {
      background: var(--accent);
      color: #fff;
      box-shadow: 0 2px 8px rgba(45,106,79,0.25), inset 0 1px 0 rgba(255,255,255,0.15);
    }
    .btn-primary:hover { background: #256042; box-shadow: 0 4px 14px rgba(45,106,79,0.3); }

    .btn-secondary {
      background: var(--surface);
      color: var(--ink-2);
      border: 1.5px solid var(--border-dark);
    }
    .btn-secondary:hover { border-color: var(--ink-3); color: var(--ink); }

    /* Hint */
    .input-hint {
      font-size: 11px;
      color: var(--ink-3);
      padding: 0 20px 16px;
      letter-spacing: 0.03em;
    }

    /* Result */
    .result-panel {
      padding: 0 20px;
      padding-bottom: 4px;
    }

    .result-box {
      border-radius: var(--radius-sm);
      padding: 12px 14px;
      margin-bottom: 12px;
      animation: resultIn 0.28s cubic-bezier(0.34,1.56,0.64,1);
    }
    @keyframes resultIn {
      from { opacity: 0; transform: scale(0.95) translateY(4px); }
      to   { opacity: 1; transform: scale(1)    translateY(0); }
    }

    .result-box.correct-box {
      background: var(--accent-bg);
      border: 1px solid var(--accent-border);
    }
    .result-box.wrong-box {
      background: var(--danger-bg);
      border: 1px solid var(--danger-border);
    }
    .result-box.warn-box {
      background: var(--gold-bg);
      border: 1px solid #e8d08a;
      color: var(--gold);
      font-size: 13px;
      text-align: center;
    }

    .result-label {
      font-size: 10px;
      font-weight: 600;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      margin-bottom: 5px;
    }
    .result-label.green { color: var(--accent); }
    .result-label.red   { color: var(--danger); }

    .result-answers {
      font-size: 12px;
      color: var(--ink-2);
      line-height: 1.8;
      font-weight: 300;
    }

    /* ===== PERFECT OVERLAY ===== */
    #overlay {
      display: none;
      position: fixed;
      inset: 0;
      background: rgba(247,246,243,0.97);
      z-index: 999;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      gap: 12px;
      text-align: center;
      padding: 24px;
    }
    #overlay.show { display: flex; }

    .overlay-icon {
      font-size: 48px;
      margin-bottom: 4px;
      animation: iconBounce 0.5s cubic-bezier(0.34,1.56,0.64,1);
    }
    @keyframes iconBounce {
      from { transform: scale(0); opacity: 0; }
      to   { transform: scale(1); opacity: 1; }
    }

    .overlay-title {
      font-family: 'Instrument Serif', serif;
      font-size: clamp(40px, 12vw, 64px);
      color: var(--ink);
      letter-spacing: -0.02em;
      line-height: 1;
    }
    .overlay-title em {
      font-style: italic;
      color: var(--accent);
    }

    .overlay-sub {
      font-size: 14px;
      color: var(--ink-3);
      font-weight: 300;
      margin-top: 4px;
    }
    .overlay-sub strong { color: var(--ink); font-weight: 500; }

    .btn-restart {
      margin-top: 16px;
      padding: 14px 40px;
      background: var(--accent);
      color: #fff;
      border-radius: var(--radius-md);
      font-size: 15px;
      font-weight: 500;
      box-shadow: 0 4px 16px rgba(45,106,79,0.25);
    }

    /* Confetti */
    .confetti-wrap { position: fixed; inset: 0; pointer-events: none; z-index: 998; overflow: hidden; }
    .confetti-dot {
      position: absolute;
      border-radius: 2px;
      animation: confettiFall linear forwards;
    }
    @keyframes confettiFall {
      0%   { opacity: 1; transform: translateY(-20px) rotate(0deg); }
      100% { opacity: 0; transform: translateY(110vh) rotate(540deg); }
    }

    /* Divider */
    .divider {
      height: 1px;
      background: var(--border);
      margin: 0 20px;
    }
  </style>
</head>
<body>

  <!-- Perfect Overlay -->
  <div id="overlay">
    <div class="confetti-wrap" id="confettiWrap"></div>
    <div class="overlay-icon">🏆</div>
    <div class="overlay-title">Vocab<em>Gacor</em></div>
    <p style="font-size:13px;font-weight:500;letter-spacing:0.06em;text-transform:uppercase;color:var(--accent);margin-top:4px;">Sempurna!</p>
    <div class="overlay-sub">
      Skor <strong id="finalScore">0</strong> dari <strong id="finalTotal">0</strong>
      &nbsp;·&nbsp; Akurasi <strong id="finalAcc">100%</strong>
    </div>
    <button class="btn-restart" onclick="restartQuiz()">Ulangi →</button>
  </div>

  <!-- Header -->
  <div class="header">
    <div class="header-top">
      <div class="wordmark">Vocab<em>Gacor</em></div>
      <div class="header-meta">
        <div class="combo-tag" id="comboTag">🔥 3x Combo</div>
        <div class="lang-pill">EN · ID</div>
      </div>
    </div>
    <div class="progress-wrap">
      <div class="progress-bar">
        <div class="progress-fill" id="progressFill" style="width:0%"></div>
      </div>
      <span class="progress-label" id="progressLabel">0%</span>
    </div>
  </div>

  <!-- Stats -->
  <div class="stats-row">
    <div class="stat">
      <div class="stat-label">Kata ke</div>
      <div class="stat-value green" id="statIndex">1</div>
    </div>
    <div class="stat">
      <div class="stat-label">Skor</div>
      <div class="stat-value gold" id="statScore">0</div>
    </div>
    <div class="stat">
      <div class="stat-label">Akurasi</div>
      <div class="stat-value" id="statAcc">—</div>
    </div>
  </div>

  <!-- Card -->
  <div class="card" id="mainCard">
    <div class="word-section">
      <div class="word-caption">🇬🇧 English</div>
      <div id="word">Loading…</div>
    </div>

    <div class="input-section">
      <label class="input-label" for="answer">Arti dalam Bahasa Indonesia</label>
      <div class="input-wrapper">
        <input type="text" id="answer"
          placeholder="Ketik jawabanmu…"
          autocomplete="off" autocorrect="off"
          autocapitalize="none" spellcheck="false"
          inputmode="text">
        <div class="input-icon" id="inputIcon"></div>
      </div>
    </div>

    <div class="input-hint" id="inputHint">Tekan Enter untuk cek · Tab untuk lewati</div>

    <div class="result-panel" id="resultPanel"></div>

    <div class="divider"></div>

    <div class="btn-section">
      <button class="btn-primary" onclick="checkAnswer()">Cek Jawaban</button>
      <button class="btn-secondary" onclick="nextWord()">Lewati →</button>
    </div>
  </div>

  <script>
    const vocab = [
      { en: "Action", id: ["tindakan", "aksi", "perbuatan", "gerakan"] }, { en: "Actual", id: ["sebenarnya", "sebetulnya", "nyata"] }, { en: "Analog", id: ["analog", "tidak digital"] }, { en: "Apron", id: ["celemek", "kain penutup baju"] }, { en: "Area", id: ["daerah", "wilayah", "kawasan"] }, { en: "Armor", id: ["baju zirah", "baju besi", "pelindung"] }, { en: "Arrive", id: ["tiba", "sampai", "datang"] }, { en: "Attempt", id: ["percobaan", "usaha", "mencoba"] }, { en: "Baker", id: ["tukang roti", "pembuat kue"] }, { en: "Bakery", id: ["toko roti", "pabrik roti"] }, { en: "Basket", id: ["keranjang"] }, { en: "Battle", id: ["pertempuran", "peperangan", "perjuangan"] }, { en: "Beast", id: ["binatang buas", "makhluk"] }, { en: "Beauty", id: ["kecantikan", "keindahan"] }, { en: "Behind", id: ["di belakang", "tertinggal"] }, { en: "Bloodthirsty", id: ["haus darah", "kejam"] }, { en: "Bone", id: ["tulang", "duri"] }, { en: "Book", id: ["buku", "memesan"] }, { en: "Borrow", id: ["meminjam"] }, { en: "Bowl", id: ["mangkuk"] }, { en: "Brave", id: ["berani", "gagah"] }, { en: "Bread", id: ["roti"] }, { en: "Bridge", id: ["jembatan", "menjembatani"] }, { en: "Brilliant", id: ["cemerlang", "cerdas", "brilian"] }, { en: "Brother", id: ["saudara laki-laki"] }, { en: "Burn", id: ["membakar", "terbakar", "hangus"] }, { en: "Bypass", id: ["jalan pintas", "memintas", "mengabaikan"] }, { en: "Capable", id: ["mampu", "cakap", "sanggup"] }, { en: "Cause", id: ["penyebab", "alasan", "menyebabkan"] }, { en: "Cautious", id: ["berhati-hati", "waspada"] }, { en: "Cave", id: ["gua"] }, { en: "Character", id: ["karakter", "tokoh", "sifat"] }, { en: "Check", id: ["memeriksa", "mengecek", "cek"] }, { en: "Chef", id: ["koki", "juru masak"] }, { en: "City", id: ["kota"] }, { en: "Climb", id: ["memanjat", "mendaki", "kenaikan"] }, { en: "Clock", id: ["jam", "waktu"] }, { en: "Code", id: ["kode", "sandi", "memprogram"] }, { en: "Company", id: ["perusahaan", "perseroan", "teman"] }, { en: "Compete", id: ["bersaing", "bertanding", "berlomba"] }, { en: "Conflict", id: ["konflik", "pertentangan", "perselisihan"] }, { en: "Connect", id: ["menghubungkan", "menyambungkan"] }, { en: "Connection", id: ["koneksi", "hubungan", "sambungan"] }, { en: "Container", id: ["wadah", "kontainer", "tempat"] }, { en: "Convince", id: ["meyakinkan"] }, { en: "Cook", id: ["memasak", "koki"] }, { en: "Creature", id: ["makhluk", "ciptaan"] }, { en: "Criminal", id: ["penjahat", "kriminal", "pidana"] }, { en: "Damage", id: ["kerusakan", "merusak", "kerugian"] }, { en: "Dance", id: ["menari", "tarian", "pesta dansa"] }, { en: "Dangerous", id: ["berbahaya"] }, { en: "Dead", id: ["mati", "padam", "sunyi"] }, { en: "Defeat", id: ["mengalahkan", "kekalahan"] }, { en: "Defense", id: ["pertahanan", "pembelaan"] }, { en: "Deliver", id: ["mengirimkan", "menyampaikan", "mengantarkan"] }, { en: "Demand", id: ["permintaan", "menuntut"] }, { en: "Device", id: ["perangkat", "alat", "perlengkapan"] }, { en: "Digital", id: ["digital"] }, { en: "Disable", id: ["menonaktifkan", "melumpuhkan"] }, { en: "Drive", id: ["mengemudi", "menyetir", "dorongan", "memacu"] }, { en: "Dust", id: ["debu", "membersihkan debu"] }, { en: "Eat", id: ["makan"] }, { en: "Electric", id: ["listrik", "elektrik"] }, { en: "Element", id: ["elemen", "unsur", "bagian"] }, { en: "Eliminate", id: ["menghapuskan", "menyingkirkan", "melenyapkan"] }, { en: "Embarrassment", id: ["rasa malu", "kemaluan"] }, { en: "Enemy", id: ["musuh"] }, { en: "Engineer", id: ["insinyur", "ahli mesin", "merekayasa"] }, { en: "Event", id: ["acara", "peristiwa", "kejadian"] }, { en: "Expect", id: ["mengharapkan", "menduga", "menantikan"] }, { en: "Expectation", id: ["harapan", "ekspektasi", "dugaan"] }, { en: "Expert", id: ["ahli", "pakar"] }, { en: "Fact", id: ["fakta", "kenyataan"] }, { en: "Fail", id: ["gagal", "melalaikan"] }, { en: "Famous", id: ["terkenal", "termasyhur"] }, { en: "Fear", id: ["ketakutan", "takut"] }, { en: "Fight", id: ["berkelahi", "bertengkar", "perjuangan"] }, { en: "Fire", id: ["api", "kebakaran", "memecat", "menembak"] }, { en: "Flee", id: ["melarikan diri", "kabur"] }, { en: "Flower", id: ["bunga"] }, { en: "Forest", id: ["hutan"] }, { en: "Forget", id: ["lupa", "melupakan"] }, { en: "Friend", id: ["teman", "kawan", "sahabat"] }, { en: "Gadget", id: ["gawai", "peranti elektronik"] }, { en: "Game", id: ["permainan", "pertandingan"] }, { en: "Gap", id: ["celah", "kesenjangan", "jurang pemisah"] }, { en: "Giant", id: ["raksasa", "sangat besar"] }, { en: "Glass", id: ["kaca", "gelas"] }, { en: "Global", id: ["global", "mendunia", "menyeluruh"] }, { en: "Grass", id: ["rumput"] }, { en: "Guest", id: ["tamu"] }, { en: "Hardware", id: ["perangkat keras", "perkakas"] }, { en: "Hat", id: ["topi"] }, { en: "Heavy", id: ["berat", "lebat", "padat"] }, { en: "Hero", id: ["pahlawan"] }, { en: "High-tech", id: ["teknologi tinggi", "canggih"] }, { en: "Homemade", id: ["buatan sendiri", "buatan rumah"] }, { en: "Hungry", id: ["lapar"] }, { en: "Hurry", id: ["buru-buru", "bergegas", "kegesaan"] }, { en: "Identity", id: ["identitas", "jati diri"] }, { en: "Impress", id: ["mengesankan", "memberi kesan"] }, { en: "Ingredient", id: ["bahan", "ramuan"] }, { en: "Interest", id: ["minat", "kepentingan", "bunga"] }, { en: "Invest", id: ["berinvestasi", "menanam modal"] }, { en: "Investigate", id: ["menyelidiki", "mengusut"] }, { en: "Invitation", id: ["undangan", "ajakan"] }, { en: "Issue", id: ["masalah", "isu", "terbitan"] }, { en: "Journey", id: ["perjalanan", "bepergian"] }, { en: "Key", id: ["kunci", "tombol", "utama"] }, { en: "Kingdom", id: ["kerajaan"] }, { en: "Kitchen", id: ["dapur"] }, { en: "Knight", id: ["ksatria"] }, { en: "Lazy", id: ["malas"] }, { en: "Lead", id: ["memimpin", "menuntun", "timbal"] }, { en: "Local", id: ["lokal", "setempat"] }, { en: "Lock", id: ["mengunci", "kunci", "gembok"] }, { en: "Logic", id: ["logika", "nalar"] }, { en: "Lonely", id: ["kesepian", "sunyi"] }, { en: "Lose", id: ["kalah", "kehilangan", "menghilangkan"] }, { en: "Lunch", id: ["makan siang"] }, { en: "Main", id: ["utama", "pokok"] }, { en: "Maintain", id: ["memelihara", "mempertahankan", "merawat"] }, { en: "Map", id: ["peta", "memetakan"] }, { en: "Marriage", id: ["pernikahan", "perkawinan"] }, { en: "Meal", id: ["makanan", "hidangan"] }, { en: "Mentor", id: ["mentor", "pembimbing"] }, { en: "Midnight", id: ["tengah malam"] }, { en: "Monster", id: ["monster", "raksasa"] }, { en: "Morning", id: ["pagi"] }, { en: "Mountain", id: ["gunung"] }, { en: "Naive", id: ["naif", "polos", "lugu"] }, { en: "Necessary", id: ["perlu", "penting", "niscaya"] }, { en: "Network", id: ["jaringan", "jejaring"] }, { en: "Notice", id: ["pemberitahuan", "memperhatikan", "catatan"] }, { en: "Offline", id: ["luring", "tidak terhubung internet"] }, { en: "Online", id: ["daring", "terhubung internet"] }, { en: "Order", id: ["pesanan", "perintah", "memesan"] }, { en: "Oven", id: ["oven", "pemanggang"] }, { en: "Owner", id: ["pemilik"] }, { en: "Path", id: ["jalan setapak", "jalur"] }, { en: "Peace", id: ["perdamaian", "ketenangan"] }, { en: "Physical", id: ["fisik", "jasmani"] }, { en: "Pitch", id: ["lemparan", "nada", "mempresentasikan ide"] }, { en: "Place", id: ["tempat", "menempatkan"] }, { en: "Portable", id: ["portabel", "mudah dibawa"] }, { en: "Prestigious", id: ["bergengsi", "prestisius"] }, { en: "Prince", id: ["pangeran"] }, { en: "Protect", id: ["melindungi", "menjaga"] }, { en: "Public", id: ["umum", "publik", "masyarakat"] }, { en: "Quality", id: ["kualitas", "mutu"] }, { en: "Reality", id: ["kenyataan", "realitas"] }, { en: "Realize", id: ["menyadari", "mewujudkan"] }, { en: "Remote", id: ["terpencil", "jauh"] }, { en: "Resolve", id: ["menyelesaikan", "membulatkan tekad"] }, { en: "Roar", id: ["mengaum", "raungan"] }, { en: "Role", id: ["peran", "tugas"] }, { en: "Royal", id: ["kerajaan", "ningrat"] }, { en: "Scare", id: ["menakuti", "kaget"] }, { en: "Scream", id: ["berteriak", "jeritan"] }, { en: "Secure", id: ["aman", "mengamankan"] }, { en: "Share", id: ["berbagi", "membagikan", "saham"] }, { en: "Shepherd", id: ["gembala"] }, { en: "Shield", id: ["perisai", "pelindung", "tameng"] }, { en: "Shiny", id: ["berkilau", "mengkilap"] }, { en: "Shoe", id: ["sepatu"] }, { en: "Shortcut", id: ["jalan pintas"] }, { en: "Silver", id: ["perak", "warna perak"] }, { en: "Skill", id: ["keterampilan", "keahlian"] }, { en: "Slipper", id: ["sandal", "selop"] }, { en: "Smell", id: ["bau", "mencium bau", "aroma"] }, { en: "Smoke", id: ["asap", "merokok"] }, { en: "Social", id: ["sosial", "kemasyarakatan"] }, { en: "Sophisticated", id: ["canggih", "rumit", "mutakhir"] }, { en: "Steal", id: ["mencuri"] }, { en: "Steam", id: ["uap", "mengukus"] }, { en: "Story", id: ["cerita", "kisah"] }, { en: "Stranger", id: ["orang asing"] }, { en: "Strike", id: ["memukul", "mogok", "serangan"] }, { en: "Struggle", id: ["perjuangan", "berjuang", "pergulatan"] }, { en: "Summit", id: ["puncak", "pertemuan tingkat tinggi"] }, { en: "Superior", id: ["unggul", "atasan", "lebih baik"] }, { en: "Surprise", id: ["kejutan", "mengejutkan", "heran"] }, { en: "Sword", id: ["pedang"] }, { en: "Tech", id: ["teknologi"] }, { en: "Terrorize", id: ["meneror", "menakut-nakuti"] }, { en: "Theme", id: ["tema", "topik"] }, { en: "Threat", id: ["ancaman"] }, { en: "Track", id: ["melacak", "jalur", "lintasan"] }, { en: "Trap", id: ["menjebak", "perangkap"] }, { en: "Trim", id: ["memangkas", "merapikan"] }, { en: "Truth", id: ["kebenaran"] }, { en: "Tunnel", id: ["terowongan"] }, { en: "Turn", id: ["berbelok", "giliran", "memutar"] }, { en: "Upload", id: ["mengunggah"] }, { en: "Use", id: ["menggunakan", "kegunaan"] }, { en: "Value", id: ["nilai", "menghargai"] }, { en: "Venture", id: ["usaha", "petualangan", "berspekulasi"] }, { en: "Victim", id: ["korban"] }, { en: "Video", id: ["video", "rekaman gambar"] }, { en: "Village", id: ["desa", "kampung"] }, { en: "Violent", id: ["kekerasan", "kasar", "beringas"] }, { en: "Viral", id: ["viral", "menyebar luas"] }, { en: "Voice", id: ["suara", "menyuarakan"] }, { en: "Warn", id: ["memperingatkan"] }, { en: "Waste", id: ["limbah", "sampah", "membuang"] }, { en: "Weapon", id: ["senjata"] }, { en: "Whisk", id: ["mengocok", "pengocok telur"] }, { en: "Wife", id: ["istri"] }, { en: "Wolf", id: ["serigala"] }, { en: "Wood", id: ["kayu", "hutan kecil"] }, { en: "Wool", id: ["wol", "bulu domba"] }
    ];

    let idx = 0, score = 0, answered = 0, combo = 0;
    let checked = false, hasAnswered = false;

    const SVG_OK   = `<svg viewBox="0 0 12 12" fill="none"><polyline points="2,6 5,9 10,3" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>`;
    const SVG_FAIL = `<svg viewBox="0 0 12 12" fill="none"><line x1="3" y1="3" x2="9" y2="9" stroke="white" stroke-width="2" stroke-linecap="round"/><line x1="9" y1="3" x2="3" y2="9" stroke="white" stroke-width="2" stroke-linecap="round"/></svg>`;

    function shuffle(arr) {
      for (let i = arr.length - 1; i > 0; i--) {
        const j = Math.floor(Math.random() * (i + 1));
        [arr[i], arr[j]] = [arr[j], arr[i]];
      }
    }

    function updateStats() {
      document.getElementById('statIndex').textContent = idx + 1;
      document.getElementById('statScore').textContent = score;
      document.getElementById('statAcc').textContent = answered > 0
        ? Math.round((score / answered) * 100) + '%' : '—';
      const pct = Math.round(((idx + 1) / vocab.length) * 100);
      document.getElementById('progressFill').style.width = pct + '%';
      document.getElementById('progressLabel').textContent = pct + '%';
    }

    function bump(id) {
      const el = document.getElementById(id);
      el.classList.remove('bump');
      void el.offsetWidth;
      el.classList.add('bump');
    }

    function setIcon(type) {
      const el = document.getElementById('inputIcon');
      el.className = 'input-icon';
      el.innerHTML = '';
      if (!type) return;
      el.classList.add('show', type);
      el.innerHTML = type === 'ok' ? SVG_OK : SVG_FAIL;
    }

    function updateCombo(correct) {
      const tag = document.getElementById('comboTag');
      if (correct) {
        combo++;
        if (combo >= 3) {
          tag.textContent = `🔥 ${combo}x Combo`;
          tag.classList.add('visible');
          tag.classList.remove('pop');
          void tag.offsetWidth;
          tag.classList.add('pop');
        }
      } else {
        combo = 0;
        tag.classList.remove('visible');
      }
    }

    function loadWord() {
      const wordEl = document.getElementById('word');
      wordEl.textContent = vocab[idx].en;
      wordEl.classList.remove('word-enter');
      void wordEl.offsetWidth;
      wordEl.classList.add('word-enter');

      const input = document.getElementById('answer');
      input.value = '';
      input.className = '';
      input.disabled = false;
      setIcon('');

      document.getElementById('mainCard').className = 'card';
      document.getElementById('resultPanel').innerHTML = '';
      document.getElementById('inputHint').textContent = 'Tekan Enter untuk cek · Tab untuk lewati';

      checked = false;
      hasAnswered = false;
      updateStats();
      setTimeout(() => input.focus(), 80);
    }

    function checkAnswer() {
      if (checked) { nextWord(); return; }

      const input = document.getElementById('answer');
      const user = input.value.toLowerCase().trim();
      const correct = vocab[idx].id.map(v => v.toLowerCase().trim());
      const panel = document.getElementById('resultPanel');

      if (!user) {
        panel.innerHTML = `<div class="result-box warn-box">⚠ Isi jawaban dulu ya!</div>`;
        return;
      }

      checked = true;
      input.disabled = true;

      if (correct.includes(user)) {
        input.classList.add('correct-input');
        setIcon('ok');
        document.getElementById('mainCard').classList.add('correct');
        document.getElementById('inputHint').textContent = 'Benar! Lanjut otomatis…';
        panel.innerHTML = `
          <div class="result-box correct-box">
            <div class="result-label green">✓ Benar</div>
            <div class="result-answers">${vocab[idx].id.join('  ·  ')}</div>
          </div>`;

        if (!hasAnswered) {
          score++;
          hasAnswered = true;
          answered++;
          bump('statScore');
          updateStats();
          updateCombo(true);
        }

        if (idx === vocab.length - 1 && score === vocab.length) {
          setTimeout(showPerfect, 1000);
        } else {
          setTimeout(nextWord, 1400);
        }

      } else {
        input.classList.add('wrong-input');
        setIcon('fail');
        document.getElementById('mainCard').classList.add('wrong');
        document.getElementById('inputHint').textContent = 'Enter lagi untuk kata berikutnya';
        panel.innerHTML = `
          <div class="result-box wrong-box">
            <div class="result-label red">✕ Salah</div>
            <div class="result-answers">${vocab[idx].id.join('  ·  ')}</div>
          </div>`;

        if (!hasAnswered) {
          hasAnswered = true;
          answered++;
          updateStats();
          updateCombo(false);
        }
        input.disabled = false;
        setTimeout(() => input.focus(), 50);
      }
    }

    function nextWord() {
      idx++;
      if (idx >= vocab.length) {
        const acc = Math.round((score / vocab.length) * 100);
        if (score === vocab.length) { showPerfect(); return; }
        alert(`Kuis Selesai!\n\nSkor: ${score} dari ${vocab.length}\nAkurasi: ${acc}%\n\nDimulai dari awal.`);
        idx = 0; score = 0; answered = 0; combo = 0;
        updateCombo(false);
        loadWord();
        return;
      }
      loadWord();
    }

    function showPerfect() {
      document.getElementById('finalScore').textContent = score;
      document.getElementById('finalTotal').textContent = vocab.length;
      document.getElementById('finalAcc').textContent = '100%';
      document.getElementById('overlay').classList.add('show');
      spawnConfetti();
    }

    function restartQuiz() {
      document.getElementById('overlay').classList.remove('show');
      document.getElementById('confettiWrap').innerHTML = '';
      idx = 0; score = 0; answered = 0; combo = 0;
      updateCombo(false);
      shuffle(vocab);
      loadWord();
    }

    function spawnConfetti() {
      const wrap = document.getElementById('confettiWrap');
      const colors = ['#2d6a4f','#52b788','#b7e4c7','#b5860d','#fbbf24','#d4cec5','#1a1916'];
      for (let i = 0; i < 70; i++) {
        const d = document.createElement('div');
        d.className = 'confetti-dot';
        d.style.left = Math.random() * 100 + 'vw';
        d.style.background = colors[Math.floor(Math.random() * colors.length)];
        const size = 5 + Math.random() * 7;
        d.style.width = size + 'px';
        d.style.height = size + 'px';
        d.style.animationDuration = (2 + Math.random() * 3) + 's';
        d.style.animationDelay = (Math.random() * 1.5) + 's';
        wrap.appendChild(d);
      }
    }

    document.getElementById('answer').addEventListener('keydown', e => {
      if (e.key === 'Enter') { e.preventDefault(); checkAnswer(); }
      if (e.key === 'Tab')   { e.preventDefault(); nextWord(); }
    });

    window.onload = () => { shuffle(vocab); loadWord(); };
  </script>
</body>
</html>
