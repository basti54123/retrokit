<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>RetroKit Chile — Juega Retro en 10 Minutos</title>
  <meta name="description" content="Instalación y configuración de emuladores lista en 10 minutos. Legal, simple y con soporte por WhatsApp. Android y PC.">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0b0f1a; --card:#12182a; --muted:#9aa4b2; --text:#eaf0ff; --brand:#5eff9c; --brand2:#6ae2ff; --danger:#ff5e7a;
      --shadow:0 10px 30px rgba(0,0,0,.35);
    }
    *{box-sizing:border-box}
    body{margin:0;background:radial-gradient(1200px 800px at 10% 0%,#111a2f 0%,#0b0f1a 40%,#0b0f1a 100%);color:var(--text);font-family:Outfit,system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;line-height:1.5}
    a{color:inherit;text-decoration:none}
    .wrap{max-width:1100px;margin:auto;padding:24px}
    .btn{display:inline-flex;gap:10px;align-items:center;border:0;padding:14px 20px;border-radius:14px;background:linear-gradient(135deg,var(--brand),var(--brand2));color:#05131a;font-weight:800;box-shadow:var(--shadow);cursor:pointer}
    .btn--ghost{background:transparent;border:1px solid #23324d;color:var(--text)}
    header{position:sticky;top:0;backdrop-filter:saturate(140%) blur(6px);background:rgba(7,11,20,.6);border-bottom:1px solid #1c2540;z-index:20}
    nav{display:flex;align-items:center;justify-content:space-between;gap:16px}
    nav .logo{display:flex;align-items:center;gap:10px;font-weight:800}
    nav .logo i{display:inline-flex;width:28px;height:28px;border-radius:8px;background:linear-gradient(135deg,var(--brand),var(--brand2));box-shadow:0 0 18px rgba(90,255,156,.3)}
    nav .links a{opacity:.8;margin:0 8px}
    .hero{display:grid;grid-template-columns:1.15fr 1fr;gap:40px;align-items:center;padding:56px 0}
    .hero h1{font-size:clamp(34px,5vw,54px);line-height:1.05;margin:0 0 14px;font-weight:800}
    .sub{color:var(--muted);font-size:18px}
    .card{background:linear-gradient(180deg,#111936,#0c1224);border:1px solid #1c2540;border-radius:20px;box-shadow:var(--shadow)}
    .hero .screen{aspect-ratio:16/10;border-radius:18px;position:relative;overflow:hidden;border:1px solid #1c2540}
    .scanline::after{content:"";position:absolute;inset:0;background:repeating-linear-gradient(to bottom,rgba(255,255,255,.04),rgba(255,255,255,.04) 1px,transparent 1px,transparent 4px);mix-blend-mode:overlay;pointer-events:none}
    .hero .glow{position:absolute;inset:auto 0 0 0;height:70px;background:radial-gradient(80% 80% at 50% 100%,rgba(106,226,255,.25),transparent 60%)}
    .badges{display:flex;flex-wrap:wrap;gap:10px;margin-top:16px}
    .badge{background:#0e1730;border:1px solid #1f2b4a;padding:6px 10px;border-radius:999px;font-size:13px;color:#cfe5ff}
    .grid{display:grid;gap:20px}
    .grid.cols-3{grid-template-columns:repeat(3,1fr)}
    .grid.cols-2{grid-template-columns:repeat(2,1fr)}
    section{padding:52px 0}
    h2{font-size:clamp(26px,3.4vw,36px);margin:0 0 10px}
    .feat{padding:18px;border-radius:16px;border:1px solid #1c2540;background:linear-gradient(180deg,#0f162d,#0c1224)}
    .feat b{display:block;font-size:18px;margin:8px 0}
    .feat i{font-style:normal;font-size:26px}
    .steps .step{display:flex;gap:14px;padding:16px 14px;border-left:3px solid #253257}
    .steps .step b{font-size:16px}
    .pricing{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .price{padding:22px;border-radius:18px;border:1px solid #1c2540;background:linear-gradient(180deg,#0f1630,#0b1122)}
    .price h3{margin:0 0 8px}
    .price ul{padding:0;margin:14px 0 18px;list-style:none}
    .price li{padding:6px 0;display:flex;gap:8px;align-items:center}
    .kicker{letter-spacing:.14em;color:#8bc7ff;font-weight:800;text-transform:uppercase;font-size:12px}
    .faq details{background:#0d142a;border:1px solid #1c2540;border-radius:14px;padding:14px}
    .faq summary{cursor:pointer;font-weight:600}
    footer{padding:40px 0;color:#8aa0bf}
    @media (max-width:960px){.hero{grid-template-columns:1fr}.pricing{grid-template-columns:1fr}.grid.cols-3{grid-template-columns:1fr}.grid.cols-2{grid-template-columns:1fr}}
  </style>
</head>
<body>
<header>
  <div class="wrap">
    <nav>
      <a class="logo" href="#top"><i></i> RetroKit <span style="opacity:.6">Chile</span></a>
      <div class="links">
        <a href="#como">Cómo funciona</a>
        <a href="#planes">Planes</a>
        <a href="#faq">FAQ</a>
      </div>
      <a class="btn" href="#comprar" aria-label="Ir a comprar">
        <span>Comprar ahora</span>
        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M5 12h14M13 5l7 7-7 7" stroke="#061118" stroke-width="2" stroke-linecap="round"/></svg>
      </a>
    </nav>
  </div>
</header>

<main id="top">
  <div class="wrap hero">
    <div>
      <span class="kicker">Android & PC</span>
      <h1>Tu infancia, lista en <span style="background:linear-gradient(135deg,var(--brand),var(--brand2));-webkit-background-clip:text;background-clip:text;color:transparent">10 minutos</span></h1>
      <p class="sub">Instalación y configuración de emuladores <b>legal</b>, simple y con soporte. Menú bonito por consolas, guías claras y actualización gratuita trimestral. Sí, <i>sin</i> tutoriales eternos.</p>
      <div class="badges">
        <span class="badge">⚡ Instalación rápida</span>
        <span class="badge">🎮 Soporta controles BT</span>
        <span class="badge">✅ Pack inicial libre/legal</span>
        <span class="badge">🛟 Soporte por WhatsApp</span>
      </div>
      <div style="display:flex;gap:12px;margin-top:22px">
        <a class="btn" href="#comprar">Quiero mi RetroKit</a>
        <a class="btn btn--ghost" href="https://wa.me/56900000000?text=Hola%20vengo%20por%20RetroKit" target="_blank" rel="noopener">Hablar por WhatsApp</a>
      </div>
      <p style="margin-top:10px;color:var(--muted);font-size:13px">*Trabajamos con juegos <b>homebrew/domínio público</b> y te guiamos para importar tus propios respaldos.</p>
    </div>

    <div class="card screen scanline" aria-label="Vista previa del menú">
      <div style="position:absolute;inset:0;display:grid;grid-template-columns:repeat(3,1fr);gap:2px;padding:8px">
        <!-- Retro grid thumbnails (SVGs as placeholders) -->
        <div style="background:#0b142a;border:1px solid #1c2540;border-radius:10px;display:flex;align-items:center;justify-content:center">🎮 SNES</div>
        <div style="background:#0b142a;border:1px solid #1c2540;border-radius:10px;display:flex;align-items:center;justify-content:center">🕹️ Arcade</div>
        <div style="background:#0b142a;border:1px solid #1c2540;border-radius:10px;display:flex;align-items:center;justify-content:center">🟨 GB/GBA</div>
        <div style="background:#0b142a;border:1px solid #1c2540;border-radius:10px;display:flex;align-items:center;justify-content:center">🌀 Mega</div>
        <div style="background:#0b142a;border:1px solid #1c2540;border-radius:10px;display:flex;align-items:center;justify-content:center">🔵 PSX</div>
        <div style="background:#0b142a;border:1px solid #1c2540;border-radius:10px;display:flex;align-items:center;justify-content:center">📼 DOS</div>
      </div>
      <div class="glow"></div>
    </div>
  </div>

  <section class="wrap" id="como">
    <h2>Cómo funciona</h2>
    <p class="sub">En 4 pasos. Fácil, chilensis y sin dramas.</p>
    <div class="grid cols-2 steps">
      <div class="step card"><div>1️⃣</div><div><b>Descarga</b><br/>Pagas online y recibes tu link al instante.</div></div>
      <div class="step card"><div>2️⃣</div><div><b>Instala</b><br/>Abres el instalador (Android o Windows) y listo. Menú bonito incluido.</div></div>
      <div class="step card"><div>3️⃣</div><div><b>Juega</b><br/>Incluye pack inicial <b>libre/legal</b>. Puedes agregar tus respaldos a la carpeta <code>Mis-Juegos</code>.</div></div>
      <div class="step card"><div>4️⃣</div><div><b>Soporte</b><br/>Video‑guías + WhatsApp. Si no corre en tu equipo, <span style="color:var(--brand)">te devolvemos el dinero</span>.</div></div>
    </div>
  </section>

  <section class="wrap" id="beneficios">
    <h2>Por qué RetroKit</h2>
    <div class="grid cols-3">
      <div class="feat"><i>✨</i><b>Legal & claro</b><span class="sub">Sin dramas: homebrew/dominio público + guía para importar tus copias.</span></div>
      <div class="feat"><i>🎯</i><b>Cero fricción</b><span class="sub">Todo configurado. Entras y juegas. Ni una línea de tutorial raro.</span></div>
      <div class="feat"><i>🎛️</i><b>Interfaz preciosa</b><span class="sub">Colecciones por consola, año y género. Portadas y videos opcionales.</span></div>
    </div>
  </section>

  <section class="wrap" id="planes">
    <h2>Planes y precios</h2>
    <p class="sub">Paga una vez, juega siempre. Actualización trimestral incluida.</p>
    <div class="pricing">
      <div class="price card">
        <h3>Lite (1 plataforma)</h3>
        <div style="font-size:30px;font-weight:800;color:var(--brand)">$2.990</div>
        <ul>
          <li>✅ Android <b>o</b> PC</li>
          <li>✅ Menú por consolas</li>
          <li>✅ Pack inicial legal</li>
          <li>— Soporte 3 días</li>
        </ul>
        <a class="btn" href="#comprar" data-plan="Lite">Elegir Lite</a>
      </div>
      <div class="price card" style="border:2px solid var(--brand)">
        <h3>Full (Android + PC)</h3>
        <div style="font-size:30px;font-weight:800;color:var(--brand)">$4.990</div>
        <ul>
          <li>✅ Android y PC</li>
          <li>✅ Portadas + listas</li>
          <li>✅ Pack inicial legal</li>
          <li>✅ Soporte 7 días</li>
        </ul>
        <a class="btn" href="#comprar" data-plan="Full">Elegir Full</a>
      </div>
      <div class="price card">
        <h3>Pro (Pendrive 128GB)</h3>
        <div style="font-size:30px;font-weight:800;color:var(--brand)">$24.990</div>
        <ul>
          <li>✅ RetroKit preinstalado</li>
          <li>✅ Espacio para respaldos</li>
          <li>✅ Soporte 15 días</li>
          <li>🚚 Retiro en Concepción</li>
        </ul>
        <a class="btn" href="https://wa.me/56900000000?text=Quiero%20RetroKit%20Pro" target="_blank" rel="noopener">Pedir Pro</a>
      </div>
    </div>
  </section>

  <section class="wrap" id="demo">
    <h2>Mini demo</h2>
    <div class="card" style="padding:14px">
      <div style="aspect-ratio:16/9;border-radius:14px;border:1px solid #1c2540;display:grid;place-items:center;color:#8fb8ff">
        <div>
          <div style="font-weight:800;font-size:20px">Aquí va tu video (YouTube no listado)</div>
          <div class="sub">Instalación en 60 segundos + gameplay</div>
        </div>
      </div>
    </div>
  </section>

  <section class="wrap faq" id="faq">
    <h2>Preguntas frecuentes</h2>
    <div class="grid cols-2">
      <details open><summary>¿Incluye juegos?</summary><div class="sub">Incluye un <b>pack inicial libre/legal</b>. Te guiamos para importar tus propios respaldos (copias personales).</div></details>
      <details><summary>¿Es compatible con controles?</summary><div class="sub">Sí, funciona con controles Bluetooth y USB. Incluimos guía paso a paso.</div></details>
      <details><summary>¿Puedo pedir devolución?</summary><div class="sub">Si no corre en tu equipo, te devolvemos el dinero dentro de 7 días. Cero drama.</div></details>
      <details><summary>¿Es legal?</summary><div class="sub">Trabajamos con software de emulación y juegos de dominio público/homebrew. No distribuimos contenidos protegidos. Te enseñamos a usar tus propias copias.</div></details>
    </div>
  </section>

  <section class="wrap card" id="comprar" style="padding:22px">
    <div class="grid cols-2">
      <div>
        <h2>Compra en 30 segundos</h2>
        <p class="sub">Paga online y recibe tu link de descarga al instante.</p>
        <form id="pay" class="grid" style="gap:12px">
          <label>Elige tu plan
            <select id="plan" style="width:100%;margin-top:6px;padding:12px;border-radius:12px;border:1px solid #1c2540;background:#0b1224;color:var(--text)">
              <option value="Lite">Lite — $2.990</option>
              <option value="Full" selected>Full — $4.990</option>
            </select>
          </label>
          <label>Tu correo para envío automático
            <input id="email" type="email" required placeholder="tucorreo@email.com" style="width:100%;margin-top:6px;padding:12px;border-radius:12px;border:1px solid #1c2540;background:#0b1224;color:var(--text)" />
          </label>
          <button type="submit" class="btn">Pagar con Flow / Webpay</button>
          <p class="sub" style="margin:0">Simulado para demo: verás un mensaje de confirmación.</p>
        </form>
      </div>
      <div>
        <h3 style="margin:0 0 8px">¿Prefieres WhatsApp?</h3>
        <p class="sub">Te atendemos al tiro. Envíanos la palabra <b>RETRO</b> y te mandamos el demo.</p>
        <a class="btn" href="https://wa.me/56900000000?text=RETRO" target="_blank" rel="noopener">Abrir WhatsApp</a>
        <div style="margin-top:16px;font-size:12px;color:#9fb3d9">Al comprar aceptas nuestros términos. No distribuimos contenidos con copyright. RetroKit es solo configuración + interfaz + soporte.</div>
      </div>
    </div>
  </section>
</main>

<footer>
  <div class="wrap">
    <div style="display:flex;gap:10px;align-items:center"><span class="logo"><i></i> RetroKit <span style="opacity:.6">Chile</span></span></div>
    <div style="margin-top:8px">© <span id="year"></span> RetroKit Chile. Hecho con ❤️ en Concepción.</div>
  </div>
</footer>

<script>
  // Año dinámico
  document.getElementById('year').textContent = new Date().getFullYear();
  // Rellenar plan desde botones
  document.querySelectorAll('[data-plan]').forEach(btn=>{
    btn.addEventListener('click',()=>{
      document.getElementById('plan').value = btn.getAttribute('data-plan');
      document.getElementById('pay').scrollIntoView({behavior:'smooth'});
    })
  })
  // Simulación de pago (reemplazar por Flow / Webpay)
  document.getElementById('pay').addEventListener('submit', (e)=>{
    e.preventDefault();
    const email = document.getElementById('email').value;
    const plan = document.getElementById('plan').value;
    alert(`✅ Pago simulado: ${plan}. Enviar link de descarga a: ${email}`);
  });
</script>
</body>
</html>
