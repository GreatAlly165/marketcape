<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MarketCape Trading • Investment Plan</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * { margin:0; padding:0; box-sizing:border-box; }
    body {
      font-family: 'Inter', sans-serif;
      background: #0b0e1a;
      color: #eef2f6;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 1.5rem;
    }
    .app-container {
      max-width: 1350px;
      width: 100%;
      background: #141a2b;
      border-radius: 2.5rem;
      padding: 2rem 2.2rem 2.5rem;
      box-shadow: 0 20px 40px rgba(0,0,0,0.6);
    }
    .header {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 1.8rem;
    }
    .brand { display: flex; align-items: center; gap: 0.75rem; }
    .brand i { font-size: 2rem; color: #f7b731; background: #1f2740; padding: 10px; border-radius: 16px; }
    .brand h1 {
      font-weight: 700; font-size: 1.9rem;
      background: linear-gradient(135deg, #f7b731, #f5a623);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }
    .brand .domain-tag {
      font-size: 0.7rem;
      background: #1f2740;
      padding: 0.2rem 0.8rem;
      border-radius: 40px;
      color: #9aa4c9;
      font-weight: 400;
      letter-spacing: 0.3px;
      margin-left: 0.2rem;
      -webkit-text-fill-color: #9aa4c9;
      background-clip: unset;
    }
    .auth-section { display: flex; flex-wrap: wrap; gap: 0.8rem; align-items: center; }
    .auth-input {
      background: #1f2740; border: 1px solid #2c3550; border-radius: 40px;
      padding: 0.7rem 1.2rem; color: #eef2f6; font-size: 0.9rem; width: 150px;
    }
    .auth-input:focus { outline: none; border-color: #f7b731; box-shadow: 0 0 0 3px rgba(247,183,49,0.2); }
    .btn {
      background: #2c3550; border: none; color: white; font-weight: 600;
      padding: 0.7rem 1.6rem; border-radius: 40px; cursor: pointer; transition: 0.2s;
      font-size: 0.9rem; display: inline-flex; align-items: center; gap: 0.5rem;
    }
    .btn-primary { background: #f7b731; color: #0b0e1a; }
    .btn-primary:hover { background: #f5a623; transform: scale(1.02); }
    .btn-outline { background: transparent; border: 1px solid #3c4668; }
    .btn-outline:hover { background: #2c3550; }
    .btn-success { background: #2ecc71; color: #0b0e1a; }
    .btn-success:hover { background: #27ae60; }
    .user-badge {
      display: flex; align-items: center; gap: 0.6rem;
      background: #1f2740; padding: 0.3rem 1.2rem 0.3rem 0.9rem; border-radius: 40px;
    }
    .user-badge i { font-size: 1.2rem; color: #f7b731; }

    /* market ticker */
    .market-ticker {
      background: #0f1629; border-radius: 2rem; padding: 1rem 2rem; margin-bottom: 2rem;
      display: flex; flex-wrap: wrap; align-items: center; justify-content: space-between;
      border: 1px solid #28304a;
    }
    .coin-stats { display: flex; flex-wrap: wrap; gap: 2rem; }
    .coin-item { display: flex; align-items: center; gap: 0.5rem; }
    .coin-item i { font-size: 1.6rem; color: #f7b731; }
    .coin-price { font-weight: 700; font-size: 1.2rem; }
    .coin-change.positive { color: #2ecc71; }
    .coin-change.negative { color: #e74c3c; }
    .coin-name { color: #9aa4c9; font-weight: 500; margin-right: 0.2rem; }

    /* INVESTMENT PLAN CARDS */
    .plan-section {
      background: #0f1629; border-radius: 2rem; padding: 1.8rem 2rem; margin: 1.5rem 0 2rem;
      border: 1px solid #28304a;
    }
    .plan-title {
      font-size: 1.6rem; font-weight: 700; margin-bottom: 1.2rem;
      display: flex; align-items: center; gap: 0.8rem;
    }
    .plan-title i { color: #f7b731; }
    .plan-grid {
      display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1.5rem;
    }
    .plan-card {
      background: #1a2238; border-radius: 1.8rem; padding: 1.5rem 1.2rem;
      border: 1px solid #2c3550; transition: 0.2s;
      text-align: center;
    }
    .plan-card:hover { border-color: #f7b731; transform: translateY(-3px); }
    .plan-range { font-weight: 700; font-size: 1.1rem; color: #f7b731; }
    .plan-rate { font-size: 2rem; font-weight: 700; margin: 0.5rem 0; }
    .plan-rate small { font-size: 1rem; font-weight: 400; color: #9aa4c9; }
    .plan-desc { color: #9aa4c9; font-size: 0.9rem; }

    /* deposit / withdraw */
    .row-cards {
      display: flex; flex-wrap: wrap; gap: 1.5rem; margin-bottom: 1.8rem;
    }
    .card {
      background: #0f1629; border-radius: 2rem; padding: 1.5rem 2rem;
      flex: 1 1 240px; border: 1px solid #28304a;
    }
    .card-title { font-weight: 600; color: #9aa4c9; margin-bottom: 0.8rem; display: flex; align-items: center; gap: 0.6rem; }
    .card-address {
      background: #1a2238; padding: 0.8rem 1.2rem; border-radius: 60px;
      font-family: monospace; font-size: 0.9rem; word-break: break-all;
      border: 1px dashed #3c4668; color: #d6def0;
    }
    .withdraw-row { display: flex; flex-wrap: wrap; gap: 0.8rem; align-items: center; }
    .withdraw-row input {
      flex: 2; min-width: 160px; background: #1a2238; border: 1px solid #2c3550;
      border-radius: 40px; padding: 0.7rem 1.2rem; color: white;
    }

    /* trade */
    .trade-section {
      background: #0f1629; border-radius: 2rem; padding: 1.8rem 2.2rem;
      border: 1px solid #28304a; display: flex; flex-wrap: wrap;
      align-items: center; justify-content: space-between;
    }
    .trade-info { display: flex; flex-wrap: wrap; align-items: center; gap: 1.5rem; }
    .trade-info span { background: #1f2740; padding: 0.4rem 1.2rem; border-radius: 40px; font-size: 0.9rem; }
    .trade-btn {
      background: #f7b731; border: none; color: #0b0e1a; font-weight: 700;
      padding: 0.9rem 2.8rem; border-radius: 60px; font-size: 1.1rem; cursor: pointer;
      transition: 0.2s; box-shadow: 0 4px 12px rgba(247,183,49,0.3);
      display: flex; align-items: center; gap: 0.8rem;
    }
    .trade-btn:hover { background: #f5a623; transform: scale(1.03); }
    .expiry-badge { background: #2c3550; padding: 0.4rem 1.4rem; border-radius: 60px; font-weight: 500; }
    .expiry-badge i { margin-right: 0.6rem; color: #f7b731; }
    .status-msg {
      margin-top: 1.2rem; padding: 0.8rem 1.5rem; border-radius: 60px;
      background: #1f2740; border-left: 5px solid #f7b731; font-weight: 500;
    }
    hr { border: 0.5px solid #28304a; margin: 1.2rem 0; }
    @media (max-width: 760px) {
      .app-container { padding: 1.2rem; }
      .header { flex-direction: column; align-items: stretch; gap: 1rem; }
      .auth-input { width: 100%; }
      .trade-section { flex-direction: column; gap: 1.2rem; align-items: stretch; }
    }
  </style>
</head>
<body>
<div class="app-container" id="app">
  <!-- HEADER with domain tag shown as "marketcape.trading" -->
  <div class="header">
    <div class="brand">
      <i class="fas fa-chart-line"></i>
      <h1>MarketCape <span class="domain-tag">.trading</span></h1>
    </div>
    <div class="auth-section" id="authSection">
      <input type="text" class="auth-input" id="authEmail" placeholder="Email or username" value="investor@mc.io">
      <input type="password" class="auth-input" id="authPassword" placeholder="Password" value="pass123">
      <button class="btn btn-primary" id="loginBtn"><i class="fas fa-sign-in-alt"></i> Login</button>
      <button class="btn btn-outline" id="registerBtn"><i class="fas fa-user-plus"></i> Register</button>
      <div id="userDisplay" class="user-badge" style="display:none;">
        <i class="fas fa-user-circle"></i><span id="usernameDisplay">Trader</span>
        <button class="btn btn-outline" id="logoutBtn" style="padding:0.2rem 0.8rem; margin-left:0.3rem; font-size:0.8rem;">Logout</button>
      </div>
    </div>
  </div>

  <!-- MARKET TICKER -->
  <div class="market-ticker">
    <div class="coin-stats">
      <div class="coin-item"><i class="fab fa-bitcoin"></i><span class="coin-name">BTC</span><span class="coin-price" id="btcPrice">$67,842</span><span class="coin-change positive" id="btcChange">+2.4%</span></div>
      <div class="coin-item"><i class="fab fa-ethereum"></i><span class="coin-name">ETH</span><span class="coin-price" id="ethPrice">$3,521</span><span class="coin-change positive" id="ethChange">+1.8%</span></div>
      <div class="coin-item"><i class="fas fa-coins"></i><span class="coin-name">USDT</span><span class="coin-price" id="usdtPrice">$1.00</span><span style="color:#9aa4c9;">stable</span></div>
      <div class="coin-item"><i class="fab fa-solana"></i><span class="coin-name">SOL</span><span class="coin-price" id="solPrice">$173.20</span><span class="coin-change negative" id="solChange">-1.2%</span></div>
    </div>
    <div><i class="fas fa-circle" style="color:#2ecc71; font-size:0.7rem;"></i> live</div>
  </div>

  <!-- INVESTMENT PLAN -->
  <div class="plan-section">
    <div class="plan-title"><i class="fas fa-layer-group"></i> Investment Plan</div>
    <div class="plan-grid">
      <div class="plan-card"><div class="plan-range">$100 – $1,000</div><div class="plan-rate">2% <small>per day</small></div><div class="plan-desc">earnings 2% daily</div></div>
      <div class="plan-card"><div class="plan-range">$1,001 – $10,000</div><div class="plan-rate">3% <small>per day</small></div><div class="plan-desc">earnings 3% daily</div></div>
      <div class="plan-card"><div class="plan-range">$10,001 – $100,000</div><div class="plan-rate">4% <small>per day</small></div><div class="plan-desc">earnings 4% daily</div></div>
      <div class="plan-card"><div class="plan-range">$100,001+</div><div class="plan-rate">5% <small>per day</small></div><div class="plan-desc">earnings 5% daily</div></div>
    </div>
  </div>

  <!-- DEPOSIT / WITHDRAW -->
  <div class="row-cards">
    <div class="card">
      <div class="card-title"><i class="fas fa-arrow-down" style="color:#f7b731;"></i> Deposit USDT (TRC20)</div>
      <div class="card-address" id="depositAddress">TYnaYopuSaMQe3ydHVCWF6EX98JmzTAh27</div>
      <div style="margin-top:0.8rem; font-size:0.8rem; color:#7b84a3;"><i class="fas fa-copy" style="cursor:pointer;" id="copyDeposit"></i> click to copy</div>
    </div>
    <div class="card">
      <div class="card-title"><i class="fas fa-arrow-up" style="color:#2ecc71;"></i> Withdrawal</div>
      <div class="withdraw-row">
        <input type="text" id="withdrawAddressInput" placeholder="TRC20 address" value="TWithdraw123...">
        <button class="btn btn-success" id="bindWithdrawBtn"><i class="fas fa-link"></i> Bind</button>
      </div>
      <div style="margin-top:0.7rem; font-size:0.85rem; color:#9aa4c9;" id="withdrawStatus"><i class="fas fa-check-circle" style="color:#2ecc71;"></i> Address: TWithdraw123... (bound)</div>
    </div>
  </div>

  <!-- TRADE -->
  <div class="trade-section">
    <div class="trade-info">
      <span><i class="fas fa-rocket" style="color:#f7b731;"></i> Auto-trade</span>
      <span><i class="fas fa-clock"></i> 96-day package</span>
      <span class="expiry-badge"><i class="fas fa-hourglass-half"></i> Expires in 96d</span>
    </div>
    <button class="trade-btn" id="tradeBtn"><i class="fas fa-play"></i> TRADE</button>
  </div>

  <div class="status-msg" id="statusMessage">
    <i class="fas fa-info-circle"></i> Click <strong>TRADE</strong> to start 96-day automated trading.
  </div>
  <div style="display:none;" id="userState">loggedOut</div>
</div>

<script>
  (function() {
    // DOM refs
    const authEmail = document.getElementById('authEmail');
    const authPassword = document.getElementById('authPassword');
    const loginBtn = document.getElementById('loginBtn');
    const registerBtn = document.getElementById('registerBtn');
    const logoutBtn = document.getElementById('logoutBtn');
    const userDisplay = document.getElementById('userDisplay');
    const usernameDisplay = document.getElementById('usernameDisplay');
    const userState = document.getElementById('userState');
    const statusMsg = document.getElementById('statusMessage');

    const depositAddr = document.getElementById('depositAddress');
    document.getElementById('copyDeposit').addEventListener('click', function() {
      navigator.clipboard?.writeText(depositAddr.innerText).then(() => {
        statusMsg.innerHTML = `<i class="fas fa-check-circle" style="color:#2ecc71;"></i> Deposit address copied!`;
      }).catch(() => {
        const range = document.createRange();
        range.selectNode(depositAddr);
        window.getSelection().removeAllRanges();
        window.getSelection().addRange(range);
        document.execCommand('copy');
        statusMsg.innerHTML = `<i class="fas fa-check-circle" style="color:#2ecc71;"></i> Address copied!`;
      });
    });

    const withdrawInput = document.getElementById('withdrawAddressInput');
    document.getElementById('bindWithdrawBtn').addEventListener('click', function() {
      const addr = withdrawInput.value.trim();
      if (addr.length > 5) {
        document.getElementById('withdrawStatus').innerHTML = `<i class="fas fa-check-circle" style="color:#2ecc71;"></i> Address: ${addr.substring(0,12)}... (bound)`;
        statusMsg.innerHTML = `<i class="fas fa-check-circle" style="color:#2ecc71;"></i> Withdrawal address updated.`;
      } else {
        statusMsg.innerHTML = `<i class="fas fa-exclamation-triangle" style="color:#f7b731;"></i> Please enter a valid TRC20 address.`;
      }
    });

    // Auth state
    let currentUser = null;
    function updateUIForUser(user) {
      if (user) {
        userDisplay.style.display = 'flex';
        usernameDisplay.textContent = user.username || 'User';
        loginBtn.style.display = 'none';
        registerBtn.style.display = 'none';
        authEmail.style.display = 'none';
        authPassword.style.display = 'none';
        userState.innerText = 'loggedIn';
        statusMsg.innerHTML = `<i class="fas fa-check-circle" style="color:#2ecc71;"></i> Welcome back, ${user.username}!`;
      } else {
        userDisplay.style.display = 'none';
        loginBtn.style.display = 'inline-flex';
        registerBtn.style.display = 'inline-flex';
        authEmail.style.display = 'inline-block';
        authPassword.style.display = 'inline-block';
        userState.innerText = 'loggedOut';
        statusMsg.innerHTML = `<i class="fas fa-info-circle"></i> Please login or register.`;
      }
    }

    let users = JSON.parse(localStorage.getItem('marketcape_users')) || [];
    if (!users.length) {
      users.push({ username: 'investor@mc.io', password: 'pass123' });
      localStorage.setItem('marketcape_users', JSON.stringify(users));
    }

    function findUser(email, password) { return users.find(u => u.username === email && u.password === password); }
    function registerUser(email, password) {
      if (!email || !password) return false;
      if (users.find(u => u.username === email)) return false;
      users.push({ username: email, password });
      localStorage.setItem('marketcape_users', JSON.stringify(users));
      return true;
    }

    loginBtn.addEventListener('click', function() {
      const email = authEmail.value.trim(), pass = authPassword.value.trim();
      const user = findUser(email, pass);
      if (user) { currentUser = user; updateUIForUser(currentUser); statusMsg.innerHTML = `<i class="fas fa-check-circle" style="color:#2ecc71;"></i> Login successful.`; }
      else { statusMsg.innerHTML = `<i class="fas fa-exclamation-triangle" style="color:#e74c3c;"></i> Invalid credentials.`; }
    });

    registerBtn.addEventListener('click', function() {
      const email = authEmail.value.trim(), pass = authPassword.value.trim();
      if (registerUser(email, pass)) {
        const newUser = findUser(email, pass);
        if (newUser) { currentUser = newUser; updateUIForUser(currentUser); statusMsg.innerHTML = `<i class="fas fa-check-circle" style="color:#2ecc71;"></i> Registered & logged in as ${email}`; }
      } else { statusMsg.innerHTML = `<i class="fas fa-exclamation-triangle" style="color:#e74c3c;"></i> Registration failed.`; }
    });

    logoutBtn.addEventListener('click', function() { currentUser = null; updateUIForUser(null); statusMsg.innerHTML = `<i class="fas fa-info-circle"></i> Logged out.`; });

    // TRADE
    const tradeBtn = document.getElementById('tradeBtn');
    let tradeActive = false, tradeTimer = null;
    tradeBtn.addEventListener('click', function() {
      if (!currentUser) { statusMsg.innerHTML = `<i class="fas fa-exclamation-triangle" style="color:#f7b731;"></i> Please login to start trading.`; return; }
      if (tradeActive) { statusMsg.innerHTML = `<i class="fas fa-info-circle" style="color:#f7b731;"></i> Trading already active. 96-day package.`; return; }
      tradeActive = true;
      statusMsg.innerHTML = `<i class="fas fa-play" style="color:#2ecc71;"></i> Trading started! 96-day package active.`;
      tradeBtn.innerHTML = `<i class="fas fa-spinner fa-pulse"></i> Trading...`;
      tradeBtn.style.background = '#2ecc71'; tradeBtn.style.color = '#0b0e1a';
      document.querySelector('.expiry-badge').innerHTML = `<i class="fas fa-hourglass-half"></i> Expires in 96d`;
      if (tradeTimer) clearTimeout(tradeTimer);
      tradeTimer = setTimeout(() => {
        tradeActive = false;
        tradeBtn.innerHTML = `<i class="fas fa-play"></i> TRADE`;
        tradeBtn.style.background = '#f7b731'; tradeBtn.style.color = '#0b0e1a';
        statusMsg.innerHTML = `<i class="fas fa-clock" style="color:#f7b731;"></i> 96-day package expired. Click TRADE to restart.`;
        document.querySelector('.expiry-badge').innerHTML = `<i class="fas fa-hourglass-end"></i> Expired`;
      }, 5000);
    });

    // Live market updates
    function updatePrices() {
      const btc = 67000 + Math.floor(Math.random() * 2000);
      const eth = 3500 + Math.floor(Math.random() * 100);
      const sol = 170 + Math.random() * 8;
      document.getElementById('btcPrice').innerText = `$${btc.toLocaleString()}`;
      document.getElementById('ethPrice').innerText = `$${eth.toLocaleString()}`;
      document.getElementById('solPrice').innerText = `$${sol.toFixed(2)}`;
      ['btc','eth','sol'].forEach(c => {
        const change = (Math.random() * 6 - 2).toFixed(1);
        const el = document.getElementById(c+'Change');
        if (el) { el.innerText = `${change}%`; el.className = `coin-change ${parseFloat(change) >= 0 ? 'positive' : 'negative'}`; }
      });
    }
    setInterval(updatePrices, 3000);

    // auto-login demo
    const demoUser = findUser('investor@mc.io', 'pass123');
    if (demoUser) { currentUser = demoUser; updateUIForUser(currentUser); }
  })();
</script>
</body>
</html>
