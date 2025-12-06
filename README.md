<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Presentación Laboral — Nombre Apellido</title>
  <meta name="description" content="Presentación profesional / CV breve de Nombre Apellido" />
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --accent:#6ee7b7; --muted:#9aa4b2; --text:#e6eef6;
      --glass: rgba(255,255,255,0.03);
      font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;background:linear-gradient(180deg,#081028 0%, #071427 100%);color:var(--text);}
    .container{max-width:900px;margin:32px auto;padding:28px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:12px;box-shadow:0 6px 30px rgba(2,6,23,0.6);}

    header{display:flex;gap:20px;align-items:center}
    .avatar{width:92px;height:92px;border-radius:12px;background:var(--glass);display:flex;align-items:center;justify-content:center;font-weight:700;color:var(--accent);font-size:30px}
    .identity{flex:1}
    h1{margin:0;font-size:24px}
    .role{color:var(--muted);margin-top:4px}
    .contact{display:flex;gap:12px;flex-wrap:wrap;margin-top:10px}
    .pill{background:rgba(255,255,255,0.02);padding:8px 12px;border-radius:999px;font-size:13px;border:1px solid rgba(255,255,255,0.03)}

    main{display:grid;grid-template-columns:1fr 320px;gap:22px;margin-top:22px}
    section.card{background:linear-gradient(180deg, rgba(255,255,255,0.015), rgba(255,255,255,0.01));padding:18px;border-radius:10px;border:1px solid rgba(255,255,255,0.02)}

    .summary p{margin:0;color:var(--muted);line-height:1.45}
    .skills{display:flex;gap:10px;flex-wrap:wrap;margin-top:10px}
    .skill{background:rgba(255,255,255,0.03);padding:6px 10px;border-radius:8px;font-size:13px}

    .xp{display:flex;flex-direction:column;gap:10px}
    .xp-item{padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.02);background:linear-gradient(180deg, rgba(0,0,0,0.02), rgba(255,255,255,0.005))}
    .xp-item h3{margin:0;font-size:15px}
    .xp-item .meta{font-size:13px;color:var(--muted);margin-top:6px}
    .projects{display:flex;flex-direction:column;gap:8px}
    .project{padding:10px;border-radius:8px;border:1px dashed rgba(255,255,255,0.02)}

    /* Sidebar */
    .side{display:flex;flex-direction:column;gap:12px}
    .side h4{margin:0 0 6px 0}
    .edu, .lang{font-size:14px;color:var(--muted)}

    footer{margin-top:18px;text-align:center;color:var(--muted);font-size:13px}

    /* Responsive */
    @media (max-width:880px){main{grid-template-columns:1fr;}
      .avatar{width:76px;height:76px;font-size:24px}
    }

    /* Print */
    @media print{
      body{background:white;color:black}
      .container{box-shadow:none;margin:0;border-radius:0}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="avatar">GA</div>
      <div class="identity">
        <h1>Nombre Apellido</h1>
        <div class="role">Desarrollador/a Frontend • React | JavaScript | UI</div>
        <div class="contact">
          <div class="pill">📍 Ciudad, País</div>
          <div class="pill">✉️ correo@ejemplo.com</div>
          <div class="pill">🔗 linkedin.com/in/tu-usuario</div>
          <div class="pill">⭐ GitHub: tu-usuario</div>
        </div>
      </div>
      <div style="margin-left:12px">
        <a href="#" onclick="window.print();return false" class="pill" style="text-decoration:none">🖨️ Imprimir / PDF</a>
      </div>
    </header>

    <main>
      <div>
        <section class="card summary">
          <h2 style="margin-top:0">Resumen profesional</h2>
          <p>Desarrollador/a con X años de experiencia construyendo aplicaciones web con React, manejo de estado, consumo de APIs y diseño de interfaces accesibles. Me enfoco en soluciones limpias, pruebas y colaboración en equipo. Busco oportunidades para crecer en equipos que valoren la calidad y el impacto.</p>
        </section>

        <section class="card" style="margin-top:12px">
          <h2>Experiencia</h2>
          <div class="xp">
            <div class="xp-item">
              <h3>Empresa Ejemplo — Desarrollador Frontend</h3>
              <div class="meta">Mar 2022 — Presente · Ciudad, País</div>
              <ul style="margin:8px 0 0 18px;color:var(--muted)">
                <li>Desarrollé módulos de UI reutilizables con React y Tailwind.</li>
                <li>Integré APIs RESTful y optimicé cargas (lazy loading, code-splitting).</li>
                <li>Mejoré la accesibilidad y la performance (Lighthouse).</li>
              </ul>
            </div>

            <div class="xp-item">
              <h3>Startup ABC — Junior Frontend</h3>
              <div class="meta">Ene 2020 — Feb 2022 · Remoto</div>
              <ul style="margin:8px 0 0 18px;color:var(--muted)">
                <li>Implementé diseños pixel-perfect y formularios con validación.</li>
                <li>Colaboré con backend para definir contratos de API y pruebas E2E.</li>
              </ul>
            </div>

          </div>
        </section>

        <section class="card" style="margin-top:12px">
          <h2>Proyectos destacados</h2>
          <div class="projects">
            <div class="project">
              <strong>Proyecto Uno</strong> — SPA para gestión de tareas. <br>
              <small class="meta">Tecnologías: React, Context, Express</small>
            </div>
            <div class="project">
              <strong>Proyecto Dos</strong> — E-commerce demo con carrito persistente.<br>
              <small class="meta">Tecnologías: React, Redux, Node.js, MySQL</small>
            </div>
          </div>
        </section>

      </div>

      <aside class="side">
        <section class="card">
          <h4>Habilidades</h4>
          <div class="skills">
            <div class="skill">React</div>
            <div class="skill">JavaScript (ES6+)</div>
            <div class="skill">HTML & CSS</div>
            <div class="skill">Git</div>
            <div class="skill">Axios / Fetch</div>
            <div class="skill">Testing (Jest)</div>
          </div>
        </section>

        <section class="card edu">
          <h4>Formación</h4>
          <div><strong>Universidad X</strong></div>
          <div class="meta">Lic. en Sistemas — 2016 — 2020</div>
        </section>

        <section class="card lang">
          <h4>Idiomas</h4>
          <div>Español — Nativo</div>
          <div>Inglés — Intermedio/Avanzado</div>
        </section>

        <section class="card">
          <h4>Contacto</h4>
          <div style="color:var(--muted);font-size:14px">Tel: +54 9 11 1234 5678</div>
          <div style="color:var(--muted);font-size:14px">Correo: correo@ejemplo.com</div>
        </section>
      </aside>
    </main>

    <footer>
      <div>Disponible para entrevistas · Referencias a pedido</div>
    </footer>
  </div>
</body>
</html>
