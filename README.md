<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>NotMobin Profile</title>
  <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      background: #0f0f0f;
      font-family: 'JetBrains Mono', monospace;
      color: #eee;
      padding: 2rem;
      margin: 0;
    }
    .card {
      max-width: 1000px;
      margin: auto;
      background: #1c1c1c;
      border-radius: 16px;
      padding: 2rem;
      box-shadow: 0 0 25px rgba(255,0,0,0.2);
      position: relative;
      overflow: hidden;
    }
    .heading {
      display: flex;
      align-items: center;
      gap: 1.5rem;
    }
    .pfp {
      border-radius: 50%;
      border: 2px solid crimson;
      width: 120px;
      height: 120px;
    }
    h1 {
      font-size: 2rem;
      margin: 0;
      color: crimson;
    }
    .roles {
      margin-top: 0.3rem;
      font-size: 0.9rem;
      color: #aaa;
    }
    .section {
      margin-top: 2rem;
    }
    .section h2 {
      color: #ff5555;
      font-size: 1.2rem;
      margin-bottom: 0.5rem;
    }
    ul {
      list-style: '✦ ';
      padding-left: 1.2rem;
    }
    .discord-btn {
      margin-top: 1.5rem;
      background: #5865F2;
      padding: 0.8rem 1.2rem;
      border-radius: 12px;
      display: inline-block;
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
    }
    .discord-btn:hover {
      background: #404eed;
    }
    .board-slide {
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      background: crimson;
      color: white;
      font-weight: bold;
      text-align: center;
      padding: 0.5rem 0;
      animation: slidein 3s ease-in-out infinite alternate;
    }

    @keyframes slidein {
      0% { transform: translateX(-100%); }
      100% { transform: translateX(0%); }
    }

    .flex-col {
      display: flex;
      flex-direction: column;
      gap: 1.2rem;
    }

    .flex-row {
      display: flex;
      gap: 2rem;
      flex-wrap: wrap;
    }

    .badge {
      background: #222;
      border: 1px solid crimson;
      border-radius: 8px;
      padding: 0.5rem 1rem;
      color: crimson;
    }
  </style>
</head>
<body>
  <div class="card">
    <div class="heading">
      <img src="https://cdn.discordapp.com/avatars/1176208389475082292/bc95e08c07f3bdc69ab36583bb0d7a0a.png?size=1024" class="pfp" alt="pfp">
      <div>
        <h1>NotMobin</h1>
        <div class="roles">🧠 System Programmer • 🧩 Reverse Engineer • 🛡️ Cyber Security Specialist</div>
        <div class="flex-row" style="margin-top: 0.5rem;">
          <span class="badge">C++</span>
          <span class="badge">x86 ASM</span>
          <span class="badge">Kernel</span>
          <span class="badge">Minecraft Plugin Dev</span>
          <span class="badge">Server Config</span>
        </div>
      </div>
    </div>

    <div class="section">
      <h2>👁️‍🗨️ About Me</h2>
      <ul>
        <li>🔬 Medium-level hacker mind with a love for reversing protocols</li>
        <li>🌱 Exploring kernel-level exploit dev, eBPF, and malware analysis</li>
        <li>🛡️ Certified: CEH v11 / v13</li>
        <li>🔧 Tools: IDA, Ghidra, Wireshark, x64dbg, Burp, Metasploit</li>
      </ul>
    </div>

    <div class="section">
      <h2>📦 Projects & Interests</h2>
      <ul>
        <li>🎮 Game Security: Anti-Cheat</li>
        <li>🔐 Hacking Tools: Custom payloads, scanners, & bypasses</li>
        <li>🕸️ Networking: Packet crafting, MITM tools, raw sockets</li>
        <li>🧬 Systems Dev: C++, C, Assembly, Static/Dynamic analysis</li>
      </ul>
    </div>

    <div class="section">
      <h2>⚡ Contact & More</h2>
      <ul>
        <li>📫 Email: mobin.abasbo@gmail.com</li>
        <li>💬 Discord: <strong>mobinnot</strong></li>
        <li>📡 Telegram: <a href="https://t.me/mobinnot" target="_blank">@mobinnot</a></li>
        <li>🧔 Pronouns: He/Him</li>
      </ul>
      <a href="https://discord.com/users/1176208389475082292" class="discord-btn" target="_blank">Join Me on Discord</a>
    </div>

    <div class="board-slide">The Board of Hermes: My Name</div>
  </div>
</body>
</html>