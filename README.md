<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>FIREAC - Anti Cheat</title>
  <style>
    body {
      font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
      background-color: #121212;
      color: #e0e0e0;
      margin: 2rem;
      line-height: 1.6;
    }
    h2, h3, h4 {
      color: #ffa500;
      margin-top: 2rem;
      margin-bottom: 1rem;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-bottom: 2rem;
    }
    table.center {
      margin-left: auto;
      margin-right: auto;
      width: auto;
    }
    th, td {
      border: 1px solid #333;
      padding: 12px 15px;
      text-align: center;
    }
    a {
      color: #ffa500;
      text-decoration: none;
      font-weight: 600;
    }
    a:hover {
      text-decoration: underline;
    }
    pre {
      background: #222;
      padding: 15px;
      border-radius: 6px;
      overflow-x: auto;
      font-size: 0.9rem;
    }
    hr {
      border: 1px solid #333;
      margin: 2rem 0;
    }
    .code-block {
      background-color: #222;
      padding: 1rem;
      border-radius: 6px;
      margin: 1rem 0 2rem;
      font-family: monospace;
      font-size: 0.9rem;
    }
    .commands td {
      padding: 20px;
      font-weight: 600;
      color: #ffd700;
      background-color: #222;
    }
  </style>
</head>
<body>

  <h2>FIREAC - Anti Cheat</h2>

  <h3>Requirements</h3>
  <table class="center">
    <tr>
      <td>
        <a href="https://github.com/ThymonA/menuv/releases" target="_blank" rel="noopener noreferrer">menuv</a><br />
        For admin menu
      </td>
      <td>
        <a href="https://github.com/jaimeadf/discord-screenshot/releases" target="_blank" rel="noopener noreferrer">discord-screenshot</a><br />
        For taking screenshots
      </td>
      <td>
        <a href="https://github.com/overextended/oxmysql/releases" target="_blank" rel="noopener noreferrer">oxmysql</a><br />
        For saving SQL data
      </td>
    </tr>
  </table>

  <hr />

  <h3>Features</h3>

  <h4>Client Side Protect</h4>
  <ul>
    <li>Anti Track Players</li>
    <li>Anti Health Hack</li>
    <li>Anti Armor Hack</li>
    <li>Anti Infinity Ammo</li>
    <li>Anti Spectate</li>
    <li>Anti Ragdoll</li>
    <li>Anti Menyoo</li>
    <li>Anti Aim Assist</li>
    <li>Anti Infinite Stamina</li>
    <li>Anti Aim Bot</li>
    <li>Anti Black List Weapon</li>
    <li>Anti Add Weapon</li>
    <li>Anti Remove Weapon</li>
    <li>Anti God Mode</li>
    <li>Anti Noclip</li>
    <li>Anti Rainbow Vehicle</li>
    <li>Anti Teleport Vehicle</li>
    <li>Anti Teleport Ped</li>
    <li>Anti Invisible</li>
    <li>Anti Change Speed</li>
    <li>Anti Free Camera</li>
    <li>Anti Plate Changer</li>
    <li>Anti Night Vision</li>
    <li>Anti Thermal Vision</li>
    <li>Anti Super Jump</li>
    <li>Anti Suicide</li>
  </ul>

  <h4>Server Side Protect</h4>
  <ul>
    <li>Anti Spam Chat</li>
    <li>Anti Black List Commands</li>
    <li>Anti Weapon Damage Changer</li>
    <li>Anti Vehicle Damage Changer</li>
    <li>Anti Black List Word</li>
    <li>Anti Bring All</li>
    <li>Anti Black List Trigger</li>
    <li>Anti Spam Trigger</li>
    <li>Anti Clear Ped Tasks</li>
    <li>Anti Taze Players</li>
    <li>Anti Inject</li>
    <li>Anti Black List Explosion</li>
    <li>Anti Explosion Spam</li>
    <li>Anti Black List Object</li>
    <li>Anti Black List Ped</li>
    <li>Anti Black List Vehicle</li>
    <li>Anti Spam Vehicle</li>
    <li>Anti Spam Ped</li>
    <li>Anti Spam Object</li>
    <li>Anti Change Perm</li>
    <li>Anti Play Sound</li>
  </ul>

  <hr />

  <h3>Inject Protect</h3>
  <ul>
    <li>Anti Resource Start / Stop / Restart</li>
    <li>Anti Add Command</li>
  </ul>

  <hr />

  <h3>Connection Protect</h3>
  <ul>
    <li>Anti VPN</li>
    <li>Anti Hosting</li>
    <li>Anti Black List Name</li>
  </ul>

  <hr />

  <h3>Ban Method</h3>
  <ul>
    <li>FiveM License</li>
    <li>Steam Identifier</li>
    <li>IP Address</li>
    <li>Microsoft ID (LIVE ID)</li>
    <li>Xbox Live ID (XBL ID)</li>
    <li>Discord ID</li>
    <li>FiveM Player Token(s)</li>
  </ul>

  <hr />

  <h3>Logs</h3>
  <ul>
    <li>Console</li>
    <li>Discord</li>
    <li>Chat</li>
    <li>Screenshot</li>
  </ul>

  <hr />

  <h3>Installation</h3>
  <p>Add this to your <code>server.cfg</code>:</p>
  <pre>
ensure FIREAC
ensure menuv
ensure screenshot-basic
ensure discord-screenshot
  </pre>

  <hr />

  <h3>Whitelist</h3>
  <p>You can add your users' identifiers via the admin menu.</p>

  <hr />

  <h3>Exports</h3>

  <h4>Server Side</h4>
  <p><code>FIREAC_CHANGE_TEMP_WHITELIST</code>: Add or remove player from Temporary whitelist.</p>
  <pre class="code-block">
// Add player to temp whitelist
exports['FIREAC']:FIREAC_CHANGE_TEMP_WHITELIST(source, true)

// Remove player from temp whitelist
exports['FIREAC']:FIREAC_CHANGE_TEMP_WHITELIST(source, false)
  </pre>

  <p><code>FIREAC_CHECK_TEMP_WHITELIST</code>: Check if player is in Temporary whitelist.</p>
  <pre class="code-block">
local isWhitelisted = exports['FIREAC']:FIREAC_CHECK_TEMP_WHITELIST(source)
  </pre>

  <p><code>FIREAC_ACTION</code>: Perform BAN, KICK or WARN on a player.</p>
  <pre class="code-block">
// Ban player
exports['FIREAC']:FIREAC_ACTION(source, "BAN", reason, details)

// Kick player
exports['FIREAC']:FIREAC_ACTION(source, "KICK", reason, details)

// Warn player
exports['FIREAC']:FIREAC_ACTION(source, "WARN", reason, details)
  </pre>

  <h4>Client Side</h4>
  <p><code>FIREAC_CHANGE_TEMP_WHITELIST</code>: Add or remove self from Temporary whitelist.</p>
  <pre class="code-block">
// Add self to temp whitelist
exports['FIREAC']:FIREAC_CHANGE_TEMP_WHITELIST(true)

// Remove self from temp whitelist
exports['FIREAC']:FIREAC_CHANGE_TEMP_WHITELIST(false)
  </pre>

  <p><code>FIREAC_CHECK_TEMP_WHITELIST</code>: Check if self is in Temporary whitelist.</p>
  <pre class="code-block">
local isWhitelisted = exports['FIREAC']:FIREAC_CHECK_TEMP_WHITELIST()
  </pre>

  <p><code>FIREAC_ACTION</code>: Perform BAN, KICK or WARN on self.</p>
  <pre class="code-block">
// Ban self
exports['FIREAC']:FIREAC_ACTION("BAN", reason, details)

// Kick self
exports['FIREAC']:FIREAC_ACTION("KICK", reason, details)

// Warn self
exports['FIREAC']:FIREAC_ACTION("WARN", reason, details)
  </pre>

  <hr />

  <h3>Commands</h3>
  <table class="center commands">
    <tr>
      <td><code>/funban [Ban ID]</code><br />Unban user from database (Admin/Console)</td>
      <td><code>/addadmin [ID]</code><br />Add admin and allow access to admin menu (Admin/Console)</td>
    </tr>
    <tr>
      <td colspan="2"><code>/addwhitelist [ID]</code><br />Add user to whitelist with full permissions (Admin/Console)</td>
    </tr>
  </table>

  <hr />

  <h3>Tutorial</h3>
  <p>Full installation guide available at: <a href="https://amirrezajaberi.ir/fireac" target="_blank" rel="noopener noreferrer">https://amirrezajaberi.ir/fireac</a></p>

  <hr />

  <h3>License</h3>
  <p style="text-align:center;">© notmobin</p>

</body>
</html>
