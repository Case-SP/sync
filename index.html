<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
<meta name="apple-mobile-web-app-title" content="sync">
<meta name="theme-color" content="#0a0a0a">
<meta name="format-detection" content="telephone=no">
<link rel="apple-touch-icon" href="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxODAgMTgwIj48cmVjdCB3aWR0aD0iMTgwIiBoZWlnaHQ9IjE4MCIgcng9IjQwIiBmaWxsPSIjMGEwYTBhIi8+PGNpcmNsZSBjeD0iOTAiIGN5PSI5MCIgcj0iNDgiIGZpbGw9Im5vbmUiIHN0cm9rZT0iI2Q0YTg2YSIgc3Ryb2tlLXdpZHRoPSIzIi8+PGxpbmUgeDE9IjkwIiB5MT0iOTAiIHgyPSI5MCIgeTI9IjU2IiBzdHJva2U9IiNkNGE4NmEiIHN0cm9rZS13aWR0aD0iMyIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIi8+PGxpbmUgeDE9IjkwIiB5MT0iOTAiIHgyPSIxMTYiIHkyPSI5MCIgc3Ryb2tlPSIjZDRhODZhIiBzdHJva2Utd2lkdGg9IjMiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIvPjwvc3ZnPg==">
<title>sync</title>
<style>
  :root {
    --bg: #0a0a0a;
    --panel: #111;
    --line: #1d1d1d;
    --line-soft: #161616;
    --fg: #e8e8e8;
    --dim: #666;
    --dimmer: #2e2e2e;
    --accent: #d4a86a;
    --accent-bg: rgba(212, 168, 106, 0.10);
    --accent-edge: rgba(212, 168, 106, 0.4);
    --now: #6ea8fe;
    --now-bg: rgba(110, 168, 254, 0.08);
    --safe-top: env(safe-area-inset-top, 0px);
    --safe-bot: env(safe-area-inset-bottom, 0px);
  }
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    -webkit-tap-highlight-color: transparent;
    -webkit-touch-callout: none;
  }
  html { height: 100%; }
  body {
    height: 100%;
    background: var(--bg);
    color: var(--fg);
    font-family: 'JetBrains Mono', ui-monospace, 'SF Mono', Menlo, monospace;
    font-size: 14px;
    line-height: 1.4;
    overflow: hidden;
    overscroll-behavior: none;
    -webkit-font-smoothing: antialiased;
    user-select: none;
    -webkit-user-select: none;
  }
  .app {
    display: flex;
    flex-direction: column;
    height: 100vh;
    height: 100dvh;
    padding-top: var(--safe-top);
    padding-bottom: var(--safe-bot);
  }
  .now-bar {
    flex: 0 0 auto;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    background: var(--bg);
    border-bottom: 1px solid var(--line);
    position: relative;
  }
  .now-cell {
    padding: 14px 12px 16px;
    text-align: center;
    border-right: 1px solid var(--line);
    min-width: 0;
  }
  .now-cell:last-child { border-right: none; }
  .now-zone {
    font-size: 9px;
    letter-spacing: 0.22em;
    text-transform: uppercase;
    color: var(--dim);
  }
  .now-time {
    font-size: 22px;
    font-weight: 500;
    color: var(--fg);
    font-variant-numeric: tabular-nums;
    margin-top: 4px;
    letter-spacing: -0.01em;
  }
  .now-time .sec {
    font-size: 11px;
    color: var(--dim);
    font-weight: 400;
    margin-left: 2px;
    letter-spacing: 0;
  }
  .now-meta {
    font-size: 9px;
    color: var(--dim);
    margin-top: 3px;
    letter-spacing: 0.06em;
    font-variant-numeric: tabular-nums;
  }
  .hint-strip {
    flex: 0 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 14px;
    border-bottom: 1px solid var(--line);
    font-size: 10px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--dim);
  }
  .reset-btn {
    color: var(--dim);
    background: transparent;
    border: 1px solid var(--dimmer);
    padding: 5px 10px;
    font: inherit;
    font-size: 9px;
    letter-spacing: 0.15em;
    cursor: pointer;
    border-radius: 2px;
    transition: all 120ms;
  }
  .reset-btn:active { background: var(--line); color: var(--fg); }
  .reset-btn.armed { color: var(--accent); border-color: var(--accent-edge); }
  .grid-wrap {
    flex: 1 1 auto;
    overflow: hidden;
    position: relative;
  }
  .grid {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    height: 100%;
    overflow: hidden;
  }
  .col {
    overflow-y: scroll;
    overflow-x: hidden;
    -webkit-overflow-scrolling: touch;
    scrollbar-width: none;
    border-right: 1px solid var(--line);
    scroll-behavior: smooth;
    background: var(--panel);
  }
  .col:last-child { border-right: none; }
  .col::-webkit-scrollbar { display: none; }
  .row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 14px;
    height: 44px;
    cursor: pointer;
    color: var(--fg);
    font-variant-numeric: tabular-nums;
    border-left: 2px solid transparent;
    border-bottom: 1px solid var(--line-soft);
    transition: background 80ms linear, color 80ms linear;
    font-size: 15px;
  }
  .row:active { background: #181818; }
  .row.active {
    background: var(--accent-bg);
    border-left-color: var(--accent);
    color: var(--accent);
  }
  .row.now-marker { color: var(--now); background: var(--now-bg); }
  .row.now-marker.active {
    background: var(--accent-bg);
    color: var(--accent);
    border-left-color: var(--accent);
  }
  .row .day {
    font-size: 10px;
    color: var(--dim);
    letter-spacing: 0.04em;
  }
  .row.active .day { color: var(--accent); }
  .row.now-marker .day { color: var(--now); }
  .row.now-marker.active .day { color: var(--accent); }
  .grid-wrap::before, .grid-wrap::after {
    content: '';
    position: absolute;
    left: 0; right: 0;
    height: 16px;
    pointer-events: none;
    z-index: 2;
  }
  .grid-wrap::before {
    top: 0;
    background: linear-gradient(180deg, var(--panel), transparent);
  }
  .grid-wrap::after {
    bottom: 0;
    background: linear-gradient(0deg, var(--panel), transparent);
  }
  @media (max-width: 360px) {
    .now-time { font-size: 19px; }
    .row { padding: 0 10px; font-size: 14px; }
    .now-cell { padding: 12px 8px 14px; }
  }
</style>
</head>
<body>
<div class="app">
  <div class="now-bar" id="nowBar">
    <div class="now-cell" data-zone="America/Los_Angeles">
      <div class="now-zone">PT · LA</div>
      <div class="now-time"></div>
      <div class="now-meta"></div>
    </div>
    <div class="now-cell" data-zone="America/New_York">
      <div class="now-zone">ET · NY</div>
      <div class="now-time"></div>
      <div class="now-meta"></div>
    </div>
    <div class="now-cell" data-zone="Asia/Tokyo">
      <div class="now-zone">JST · TYO</div>
      <div class="now-time"></div>
      <div class="now-meta"></div>
    </div>
  </div>
  <div class="hint-strip">
    <span id="status">tap an hour</span>
    <button class="reset-btn" id="reset">RESET</button>
  </div>
  <div class="grid-wrap">
    <div class="grid">
      <div class="col" data-zone="America/Los_Angeles"></div>
      <div class="col" data-zone="America/New_York"></div>
      <div class="col" data-zone="Asia/Tokyo"></div>
    </div>
  </div>
</div>
<script>
  function zoneOffsetMs(zone, date) {
    const dtf = new Intl.DateTimeFormat('en-US', {
      timeZone: zone, hourCycle: 'h23',
      year: 'numeric', month: '2-digit', day: '2-digit',
      hour: '2-digit', minute: '2-digit', second: '2-digit'
    });
    const m = {};
    for (const p of dtf.formatToParts(date)) m[p.type] = p.value;
    const asUTC = Date.UTC(+m.year, +m.month - 1, +m.day, +m.hour, +m.minute, +m.second);
    return asUTC - date.getTime();
  }
  function ymdInZone(zone, date) {
    const dtf = new Intl.DateTimeFormat('en-CA', {
      timeZone: zone, year: 'numeric', month: '2-digit', day: '2-digit'
    });
    const m = {};
    for (const p of dtf.formatToParts(date)) m[p.type] = p.value;
    return { y: +m.year, mo: +m.month, d: +m.day };
  }
  function dateAtHourInZone(zone, hour) {
    const { y, mo, d } = ymdInZone(zone, new Date());
    const tentative = new Date(Date.UTC(y, mo - 1, d, hour, 0, 0));
    const off = zoneOffsetMs(zone, tentative);
    return new Date(tentative.getTime() - off);
  }
  function readInZone(zone, date) {
    const dtf = new Intl.DateTimeFormat('en-CA', {
      timeZone: zone, hourCycle: 'h23',
      year: 'numeric', month: '2-digit', day: '2-digit',
      hour: '2-digit', minute: '2-digit', second: '2-digit', weekday: 'short'
    });
    const m = {};
    for (const p of dtf.formatToParts(date)) m[p.type] = p.value;
    const today = ymdInZone(zone, new Date());
    const t = Date.UTC(today.y, today.mo - 1, today.d);
    const that = Date.UTC(+m.year, +m.month - 1, +m.day);
    return {
      hour: +m.hour % 24, minute: +m.minute, second: +m.second,
      weekday: m.weekday, day: +m.day, month: +m.month,
      dayDiff: Math.round((that - t) / 86400000)
    };
  }
  function pad(n) { return String(n).padStart(2, '0'); }
  function dayLabel(diff) {
    if (diff === 0) return '';
    if (diff > 0) return '+' + diff + 'd';
    return diff + 'd';
  }
  const cols = Array.from(document.querySelectorAll('.col'));
  const nowCells = Array.from(document.querySelectorAll('.now-cell'));
  const statusEl = document.getElementById('status');
  const resetBtn = document.getElementById('reset');
  let selectedTs = null;
  function renderRows() {
    for (const col of cols) {
      const zone = col.dataset.zone;
      const nowRead = readInZone(zone, new Date());
      col.innerHTML = '';
      for (let h = 0; h < 24; h++) {
        const d = dateAtHourInZone(zone, h);
        const row = document.createElement('div');
        row.className = 'row';
        row.dataset.zone = zone;
        row.dataset.hour = h;
        row.dataset.ts = d.getTime();
        const time = document.createElement('span');
        time.textContent = pad(h) + ':00';
        const day = document.createElement('span');
        day.className = 'day';
        row.appendChild(time);
        row.appendChild(day);
        if (h === nowRead.hour) row.classList.add('now-marker');
        row.addEventListener('click', () => select(d.getTime()));
        col.appendChild(row);
      }
    }
    if (selectedTs !== null) applySelection();
  }
  function updateNowBar() {
    const now = new Date();
    nowCells.forEach(cell => {
      const zone = cell.dataset.zone;
      const r = readInZone(zone, now);
      cell.querySelector('.now-time').innerHTML =
        pad(r.hour) + ':' + pad(r.minute) +
        '<span class="sec">:' + pad(r.second) + '</span>';
      cell.querySelector('.now-meta').textContent =
        r.weekday + ' · ' + pad(r.month) + '/' + pad(r.day);
    });
  }
  function applySelection() {
    const date = new Date(selectedTs);
    let summaryParts = [];
    const zoneShort = {
      'America/Los_Angeles': 'PT',
      'America/New_York': 'ET',
      'Asia/Tokyo': 'JST'
    };
    for (const col of cols) {
      const zone = col.dataset.zone;
      const r = readInZone(zone, date);
      summaryParts.push(zoneShort[zone] + ' ' + pad(r.hour) + ':00' +
        (r.dayDiff !== 0 ? dayLabel(r.dayDiff) : ''));
      col.querySelectorAll('.row').forEach(el => {
        const h = +el.dataset.hour;
        const dayEl = el.querySelector('.day');
        if (h === r.hour) {
          el.classList.add('active');
          dayEl.textContent = dayLabel(r.dayDiff);
        } else {
          el.classList.remove('active');
          dayEl.textContent = '';
        }
      });
    }
    statusEl.textContent = summaryParts.join('  →  ');
    resetBtn.classList.add('armed');
  }
  function clearSelection() {
    selectedTs = null;
    document.querySelectorAll('.row').forEach(el => {
      el.classList.remove('active');
      const d = el.querySelector('.day');
      if (d) d.textContent = '';
    });
    statusEl.textContent = 'tap an hour';
    resetBtn.classList.remove('armed');
  }
  function select(ts) {
    if (selectedTs === ts) { clearSelection(); return; }
    selectedTs = ts;
    applySelection();
    if (window.navigator.vibrate) window.navigator.vibrate(8);
  }
  resetBtn.addEventListener('click', clearSelection);
  function scrollToNow(smooth = false) {
    cols.forEach(col => {
      const nowRow = col.querySelector('.row.now-marker');
      if (!nowRow) return;
      const target = nowRow.offsetTop - 44 * 1.5;
      if (smooth) col.scrollTo({ top: target, behavior: 'smooth' });
      else col.scrollTop = target;
    });
  }
  function fullRefresh() {
    renderRows();
    updateNowBar();
    scrollToNow(false);
  }
  renderRows();
  updateNowBar();
  requestAnimationFrame(() => scrollToNow(false));
  setInterval(updateNowBar, 1000);
  setInterval(fullRefresh, 60 * 60 * 1000);
  document.addEventListener('visibilitychange', () => {
    if (!document.hidden) fullRefresh();
  });
  window.addEventListener('pageshow', () => fullRefresh());
</script>
</body>
</html>
