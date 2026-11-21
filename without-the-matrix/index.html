<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<link rel="icon" type="image/x-icon" href="/images/favicon.ico">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Link Library</title>
<style>
  :root {
    color-scheme: dark;
    --bg: #101214;
    --panel: #191c20;
    --panel-2: #20242a;
    --border: #30363d;
    --text: #edf0f2;
    --muted: #9ba4ad;
    --green: #a8f0b0;
    --visited: #858c94;
    --danger: #ff8585;
  }
  * { box-sizing: border-box; }
  body {
    margin: 0; min-height: 100vh; padding: 8px 18px;
    background: radial-gradient(ellipse at top, #1b2220 0, var(--bg) 52%);
    color: var(--text); font: 16px/1.5 system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  }
  main { width: min(760px, 100%); margin: 0 auto; }
  header { text-align: center; margin-bottom: 28px; }
  h1 { margin: 0 0 8px; font-size: clamp(2rem, 6vw, 2.8rem); letter-spacing: -.04em; }
  header p { margin: 0; color: var(--muted); }
  .panel { background: color-mix(in srgb, var(--panel) 94%, transparent); border: 1px solid var(--border); border-radius: 18px; padding: 20px; box-shadow: 0 18px 60px #0003; }
  label { display: block; margin-bottom: 8px; font-weight: 650; }
  textarea {
    display: block; width: 100%; min-height: 100px; resize: vertical;
    padding: 13px 14px; border: 1px solid var(--border); border-radius: 12px;
    background: #111417; color: var(--text); font: inherit; outline: none;
  }
  textarea:focus, input:focus { border-color: #8cdda0; box-shadow: 0 0 0 3px #8cdda022; }
  .hint { color: var(--muted); font-size: .88rem; margin: 8px 0 14px; }
  .actions { display: flex; flex-wrap: wrap; gap: 10px; }
  button {
    border: 1px solid var(--border); border-radius: 10px; padding: 10px 14px;
    color: var(--text); background: var(--panel-2); font: inherit; font-weight: 650; cursor: pointer;
  }
  button:hover { filter: brightness(1.13); }
  .primary { color: #102014; background: var(--green); border-color: var(--green); }
  .danger { color: var(--danger); }
  .list-head { display: flex; align-items: center; justify-content: space-between; gap: 12px; margin: 28px 2px 12px; }
  .list-head h2 { margin: 0; font-size: 1.15rem; }
  #count { color: var(--muted); font-size: .9rem; }
  #links { display: grid; gap: 10px; }
  .link-row { display: flex; align-items: center; gap: 12px; padding: 13px 14px; background: var(--panel); border: 1px solid var(--border); border-radius: 12px; min-width: 0; }
  .link-main { min-width: 0; flex: 1; }
  .link-main a { display: block; color: var(--green); text-decoration: none; overflow-wrap: anywhere; font-weight: 620; }
  .link-main a:hover { text-decoration: underline; text-underline-offset: 4px; }
  .link-main a.visited { color: var(--visited); }
  .remove { flex: 0 0 auto; padding: 7px 10px; color: var(--muted); }
  .empty { text-align: center; padding: 30px 15px; border: 1px dashed var(--border); border-radius: 12px; color: var(--muted); }
  .footer { color: var(--muted); text-align: center; font-size: .82rem; margin: 22px 0 0; }
  @media (max-width: 520px) { body { padding: 28px 12px; } .panel { padding: 15px; } .link-row { padding: 11px; } .list-head { align-items: flex-start; } }

       .back-btn {
    display: inline-block;
    padding: 12px 30px;
    font-size: 18px;
    font-weight: bold;
    color: #fff;
    text-decoration: none;
    background: #222;
    border: 2px solid #fff;
    border-radius: 8px;
    box-shadow: 0 0 10px #fff33f33;
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
}

.back-btn::before {
    content: '';
    position: absolute;
    top: 50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: rgba(255, 255, 255, 0.2);
    transform: rotate(45deg);
    transition: all 0.5s ease;
}

.back-btn:hover::before {
    left: 100%;
}

.back-btn:hover {
    color: #fff;
    background: #111;
    box-shadow: 0 0 20px #fffa00, 0 0 30px #fffa00, 0 0 40px #fffa00;
    transform: scale(1.05);
}


  /* Matrix screensaver layer */
  #matrix {
    position: fixed; inset: 0; width: 100%; height: 100%;
    opacity: 0; visibility: hidden; pointer-events: none;
    background: #000; z-index: 9999; transition: opacity .45s ease;
  }
  body.matrix-active #matrix { opacity: 1; visibility: visible; }
  @media (prefers-reduced-motion: reduce) { #matrix { transition: none; } }
</style>
</head>
<body>
<main>
  <header>
    <h1>Link Library</h1>
  </header>

  <section class="panel" aria-labelledby="add-heading">
    <label id="add-heading" for="linkInput">Add links</label>
    <textarea id="linkInput" placeholder="https://www.youtube.com/&#10;https://example.com/&#10;Paste one link per line…"></textarea>
    <p class="hint">Paste one URL per line. Existing links stay in place; duplicates are skipped.</p>
    <div class="actions">
      <button class="primary" id="addBtn">Add links</button>
      <button id="sortBtn" title="Sort links alphabetically">Sort A–Z</button>
    </div>
    <p id="status" class="hint" role="status" aria-live="polite"></p>
  </section>

  <div class="list-head">
    <h2>Your saved links</h2>
    <span id="count">0 links</span>
  </div>
  <section id="links" aria-live="polite"></section>
  <div class="actions" style="justify-content:center; margin-top:16px">
    <button class="danger" id="clearBtn">Clear all links</button>
  </div>
  
  <br>
<center>
<a href="../" class="back-btn">Back</a>
<br>


  <p class="footer">Saved in this browser on this device. Green links turn grey after you open them.</p>
</main>

<!-- Matrix screensaver canvas; the Link Library content stays underneath -->
<canvas id="matrix" aria-hidden="true"></canvas>

<script>
(() => {
  const LINKS_KEY='link-library-items-v1';
  const VISITED_KEY='link-library-visited-v1';
  const input=document.getElementById('linkInput');
  const list=document.getElementById('links');
  const count=document.getElementById('count');
  const status=document.getElementById('status');

  function read(key, fallback) {
    try {
      const value=JSON.parse(localStorage.getItem(key));
      return Array.isArray(value) ? value : fallback;
    } catch { return fallback; }
  }
  let links=[...new Set(read(LINKS_KEY, []).map(normalize).filter(Boolean))];
  let visited=new Set(read(VISITED_KEY, []).map(normalize).filter(Boolean));
  function save() {
    try {
      localStorage.setItem(LINKS_KEY, JSON.stringify(links));
      localStorage.setItem(VISITED_KEY, JSON.stringify([...visited]));
    } catch (error) {
      status.textContent='Browser storage is unavailable here. Open this file in a normal browser tab and allow local storage.';
    }
  }
  function normalize(raw) {
    let value=raw.trim();
    if (!value) return null;
    if (!/^[a-zA-Z][a-zA-Z\d+.-]*:/.test(value)) value='https://' + value;
    try {
      const url=new URL(value);
      if (!['http:', 'https:'].includes(url.protocol)) return null;
      return url.href;
    } catch { return null; }
  }
  function labelFor(url) {
    try {
      const parsed=new URL(url);
      return parsed.hostname.replace(/^www\./, '') + (parsed.pathname !== '/' ? parsed.pathname : '') + parsed.search + parsed.hash;
    } catch { return url; }
  }
  function render() {
    list.replaceChildren();
    count.textContent=`${links.length} ${links.length === 1 ? 'link' : 'links'}`;
    if (!links.length) {
      const empty=document.createElement('div');
      empty.className='empty';
      empty.textContent='No links yet — add one above to get started.';
      list.append(empty);
      return;
    }
    links.forEach((url, index) => {
      const row=document.createElement('div');
      row.className='link-row';
      const main=document.createElement('div');
      main.className='link-main';
      const anchor=document.createElement('a');
      anchor.href=url;
      anchor.target='_blank';
      anchor.rel='noopener noreferrer';
      anchor.textContent=labelFor(url);
      anchor.title=url;
      if (visited.has(url)) anchor.classList.add('visited');
      anchor.addEventListener('click', () => {
        visited.add(url);
        anchor.classList.add('visited');
        save();
      });
      main.append(anchor);
      const remove=document.createElement('button');
      remove.className='remove';
      remove.textContent='Remove';
      remove.setAttribute('aria-label', `Remove ${url}`);
      remove.addEventListener('click', () => {
        links.splice(index, 1);
        save(); render();
        status.textContent='Link removed.';
      });
      row.append(main, remove);
      list.append(row);
    });
  }
  document.getElementById('addBtn').addEventListener('click', () => {
    const lines=input.value.split(/\r?\n/).map(s => s.trim()).filter(Boolean);
    if (!lines.length) { status.textContent='Paste at least one link first.'; return; }
    let added=0, duplicates=0, invalid=0;
    for (const line of lines) {
      const url=normalize(line);
      if (!url) { invalid++; continue; }
      if (links.includes(url)) { duplicates++; continue; }
      links.push(url); added++;
    }
    save(); render();
    input.value='';
    status.textContent=`Added ${added}; skipped ${duplicates} duplicate${duplicates === 1 ? '' : 's'}${invalid ? `; ignored ${invalid} invalid line${invalid === 1 ? '' : 's'}` : ''}.`;
  });
  document.getElementById('clearBtn').addEventListener('click', () => {
    if (!links.length) { status.textContent='There are no links to clear.'; return; }
    if (confirm(`Clear all ${links.length} saved links? This cannot be undone.`)) {
      links=[];
      visited=new Set();
      save(); render();
      status.textContent='All links cleared.';
    }
  });
  document.getElementById('sortBtn').addEventListener('click', () => {
    links.sort((a, b) => labelFor(a).localeCompare(labelFor(b)));
    save(); render();
    status.textContent='Links sorted A–Z.';
  });
  render();

  // Matrix screensaver: after 10 seconds without activity, show digital rain.
  const IDLE_DELAY=10000;
  const canvas=document.getElementById('matrix');
  const ctx=canvas.getContext('2d');
  const chars='アカサタナハマヤラワ012345789ABCDEFGHIJKLMNOPQRSTUVWXYZ:・."=*+-<>';
  let width=0, height=0, fontSize=17, drops=[];
  let idleTimer=null, animationFrame=null, active=false, lastActivity=Date.now();

  function resizeMatrix() {
    const dpr=Math.min(window.devicePixelRatio || 1, 2);
    width=window.innerWidth;
    height=window.innerHeight;
    canvas.width=Math.floor(width * dpr);
    canvas.height=Math.floor(height * dpr);
    ctx.setTransform(dpr, 0, 0, dpr, 0, 0);
    fontSize=Math.max(13, Math.min(20, Math.round(width / 90)));
    const columns=Math.ceil(width / fontSize);
    drops=Array.from({ length: columns }, () => Math.random() * -(height / fontSize));
    ctx.fillStyle='#000';
    ctx.fillRect(0, 0, width, height);
  }

  function drawMatrix() {
    if (!active) return;
    ctx.fillStyle='rgba(0, 0, 0, 0.075)';
    ctx.fillRect(0, 0, width, height);
    ctx.font=fontSize + 'px Consolas, monospace';
    for (let i=0; i < drops.length; i++) {
      const char=chars[Math.floor(Math.random() * chars.length)];
      const x=i * fontSize, y=drops[i] * fontSize;
      const bright=Math.random() > .975;
      ctx.fillStyle=bright ? '#d9ffe5' : (Math.random() > .25 ? '#20f56d' : '#078b3b');
      ctx.shadowBlur=bright ? 12 : 3;
      ctx.shadowColor=bright ? '#aaffc4' : '#00ff55';
      ctx.fillText(char, x, y);
      ctx.shadowBlur=0;
      if (y > height && Math.random() > .975) drops[i]=Math.random() * -25;
      else drops[i] += Math.random() > .985 ? 1.8 : .8;
    }
    animationFrame=requestAnimationFrame(drawMatrix);
  }

  function enterMatrix() {
    active=true;
    document.body.classList.add('matrix-active');
    cancelAnimationFrame(animationFrame);
    ctx.fillStyle='#000';
    ctx.fillRect(0, 0, width, height);
    drawMatrix();
  }

  function scheduleMatrix() {
    clearTimeout(idleTimer);
    idleTimer=setTimeout(enterMatrix, Math.max(0, IDLE_DELAY - (Date.now() - lastActivity)));
  }

  function noteActivity() {
    lastActivity=Date.now();
    if (active) {
      active=false;
      document.body.classList.remove('matrix-active');
      cancelAnimationFrame(animationFrame);
    }
    scheduleMatrix();
  }

  window.addEventListener('resize', resizeMatrix);
  window.addEventListener('mousemove', noteActivity, { passive: true });
  window.addEventListener('mousedown', noteActivity, { passive: true });
  window.addEventListener('keydown', noteActivity);
  window.addEventListener('touchstart', noteActivity, { passive: true });
  resizeMatrix();
  scheduleMatrix();
})();
</script>
</body>
</html>

