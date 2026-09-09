<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Perfil — Data Analyst</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Inter:wght@400;500;600&display=swap');

  :root{
    --bg: #0B1220;
    --panel: #121B2E;
    --panel-line: #223049;
    --text: #E7ECF5;
    --muted: #90A0B7;
    --grid-line: rgba(231,236,245,0.05);
  }

  *{ box-sizing: border-box; }

  body{
    margin: 0;
    background: var(--bg);
    color: var(--text);
    font-family: 'Inter', sans-serif;
    line-height: 1.5;
  }

  a{ color: inherit; }

  .wrap{
    max-width: 860px;
    margin: 0 auto;
    padding: 0 24px;
  }

  /* HERO */
  .hero{
    position: relative;
    padding: 96px 0 64px;
    background-image:
      linear-gradient(var(--grid-line) 1px, transparent 1px),
      linear-gradient(90deg, var(--grid-line) 1px, transparent 1px);
    background-size: 40px 40px;
    border-bottom: 1px solid var(--panel-line);
    overflow: hidden;
  }

  .hero::after{
    content: "";
    position: absolute;
    right: -120px;
    top: -80px;
    width: 420px;
    height: 420px;
    background: radial-gradient(circle, rgba(56,189,248,0.14) 0%, rgba(56,189,248,0) 70%);
  }

  .eyebrow{
    color: #38BDF8;
    font-size: 14px;
    font-weight: 600;
    margin: 0 0 14px;
  }

  h1{
    font-family: 'Space Grotesk', sans-serif;
    font-size: clamp(36px, 6vw, 56px);
    font-weight: 700;
    margin: 0 0 16px;
    letter-spacing: -0.5px;
    max-width: 12ch;
  }

  .lede{
    color: var(--muted);
    font-size: 18px;
    max-width: 56ch;
    margin: 0;
  }

  /* SECTION HEADS */
  section{ padding: 64px 0; }
  section + section{ border-top: 1px solid var(--panel-line); }

  h2{
    font-family: 'Space Grotesk', sans-serif;
    font-size: 24px;
    font-weight: 600;
    margin: 0 0 8px;
  }

  .section-note{
    color: var(--muted);
    font-size: 15px;
    max-width: 60ch;
    margin: 0 0 36px;
  }

  /* SKILLS */
  .skills{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1px;
    background: var(--panel-line);
    border: 1px solid var(--panel-line);
  }

  .skill{
    background: var(--panel);
    padding: 24px 20px;
    position: relative;
  }

  .skill::before{
    content: "";
    position: absolute;
    top: 0; left: 0;
    width: 100%;
    height: 3px;
    background: var(--accent);
  }

  .skill-icon{
    width: 30px;
    height: 30px;
    margin-bottom: 14px;
    color: var(--accent);
  }

  .skill-icon svg{
    width: 100%;
    height: 100%;
    display: block;
  }

  .skill-name{
    font-family: 'Space Grotesk', sans-serif;
    font-weight: 600;
    font-size: 16px;
    margin: 0 0 6px;
  }

  .skill-role{
    color: var(--muted);
    font-size: 13px;
    margin: 0;
  }

  .skill[data-c="excel"]{ --accent: #22A65A; }
  .skill[data-c="sql"]{ --accent: #38BDF8; }
  .skill[data-c="python"]{ --accent: #F2C744; }
  .skill[data-c="databricks"]{ --accent: #FF6B4A; }
  .skill[data-c="powerbi"]{ --accent: #F2B90D; }
  .skill[data-c="ai"]{ --accent: #B084F5; }

  /* GOAL */
  .goal p{
    max-width: 62ch;
    color: var(--text);
    font-size: 16px;
    margin: 0 0 16px;
  }
  .goal p:last-child{ margin-bottom: 0; }

  /* CONTACT */
  .contact-list{
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .contact-list a{
    display: inline-block;
    padding: 10px 18px;
    border: 1px solid var(--panel-line);
    border-radius: 4px;
    text-decoration: none;
    font-size: 14px;
    font-weight: 500;
    transition: border-color .15s ease, background .15s ease;
  }

  .contact-list a:hover{
    border-color: #38BDF8;
    background: rgba(56,189,248,0.08);
  }

  footer{
    padding: 32px 0 56px;
    color: var(--muted);
    font-size: 13px;
  }

  @media (max-width: 640px){
    .skills{ grid-template-columns: 1fr; }
    .hero{ padding: 64px 0 48px; }
  }
</style>
</head>
<body>

<div class="hero">
  <div class="wrap">
    <p class="eyebrow">Data Analyst · Em transição de carreira</p>
    <h1>Transformando dados em decisões melhores</h1>
    <p class="lede">
      Junior Data Analyst apaixonado por tecnologia, dados e resolução de problemas.
      Desenvolvendo habilidades em Data Analytics, Business Intelligence e Inteligência Artificial.
    </p>
  </div>
</div>

<section>
  <div class="wrap">
    <h2>Skills &amp; Technologies</h2>
    <p class="section-note">Ferramentas que uso no dia a dia para analisar, tratar e visualizar dados.</p>

    <div class="skills">
      <div class="skill" data-c="excel">
        <div class="skill-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round">
            <rect x="3" y="3.5" width="18" height="17" rx="1.5"/>
            <line x1="3" y1="9" x2="21" y2="9"/>
            <line x1="3" y1="14.5" x2="21" y2="14.5"/>
            <line x1="9" y1="3.5" x2="9" y2="20.5"/>
            <line x1="15" y1="3.5" x2="15" y2="20.5"/>
          </svg>
        </div>
        <p class="skill-name">Excel</p>
        <p class="skill-role">Análise, limpeza e visualização de dados</p>
      </div>
      <div class="skill" data-c="sql">
        <div class="skill-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round">
            <ellipse cx="12" cy="5.5" rx="8" ry="3"/>
            <path d="M4 5.5v13c0 1.7 3.6 3 8 3s8-1.3 8-3v-13"/>
            <path d="M4 12c0 1.7 3.6 3 8 3s8-1.3 8-3"/>
          </svg>
        </div>
        <p class="skill-name">SQL</p>
        <p class="skill-role">Consultas, manipulação e análise de dados</p>
      </div>
      <div class="skill" data-c="python">
        <div class="skill-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round">
            <path d="M12 3c-2.8 0-5 .8-5 3v3h5"/>
            <path d="M12 3c2.8 0 5 .8 5 3v3"/>
            <rect x="4" y="6" width="10" height="6" rx="2"/>
            <path d="M12 21c2.8 0 5-.8 5-3v-3h-5"/>
            <path d="M12 21c-2.8 0-5-.8-5-3v-3"/>
            <rect x="10" y="12" width="10" height="6" rx="2"/>
            <circle cx="9" cy="8.4" r=".4" fill="currentColor" stroke="none"/>
            <circle cx="15" cy="15.6" r=".4" fill="currentColor" stroke="none"/>
          </svg>
        </div>
        <p class="skill-name">Python</p>
        <p class="skill-role">Análise de dados e automação</p>
      </div>
      <div class="skill" data-c="databricks">
        <div class="skill-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round">
            <path d="M12 3.5 3 8l9 4.5 9-4.5-9-4.5Z"/>
            <path d="M3 12.5 12 17l9-4.5"/>
            <path d="M3 16.5 12 21l9-4.5"/>
          </svg>
        </div>
        <p class="skill-name">Databricks</p>
        <p class="skill-role">Processamento e exploração de dados</p>
      </div>
      <div class="skill" data-c="powerbi">
        <div class="skill-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round">
            <line x1="4" y1="20" x2="4" y2="10"/>
            <line x1="10" y1="20" x2="10" y2="4"/>
            <line x1="16" y1="20" x2="16" y2="13"/>
            <line x1="20.5" y1="20" x2="20.5" y2="8"/>
          </svg>
        </div>
        <p class="skill-name">Power BI</p>
        <p class="skill-role">Dashboards, KPIs e visualização de dados</p>
      </div>
      <div class="skill" data-c="ai">
        <div class="skill-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round">
            <circle cx="12" cy="12" r="3"/>
            <path d="M12 3v2.5M12 18.5V21M21 12h-2.5M5.5 12H3M18.4 5.6l-1.8 1.8M7.4 16.6l-1.8 1.8M18.4 18.4l-1.8-1.8M7.4 7.4 5.6 5.6"/>
          </svg>
        </div>
        <p class="skill-name">Inteligência Artificial</p>
        <p class="skill-role">Ferramentas de IA para produtividade e análise</p>
      </div>
    </div>
  </div>
</section>

<section class="goal">
  <div class="wrap">
    <h2>Objetivo de carreira</h2>
    <p>
      Estou em busca de oportunidades para crescer profissionalmente na área de dados,
      aplicar meus conhecimentos em projetos reais e aprender continuamente novas
      tecnologias e boas práticas.
    </p>
    <p>
      Neste GitHub, compartilho projetos, estudos e experimentos relacionados a análise
      de dados, programação, business intelligence e inteligência artificial.
    </p>
    <p>Sempre aprendendo, construindo e transformando dados em insights.</p>
  </div>
</section>

<section>
  <div class="wrap">
    <h2>Contato</h2>
    <ul class="contact-list">
      <li><a href="https://www.linkedin.com/in/SEU_LINKEDIN" target="_blank">LinkedIn</a></li>
      <li><a href="mailto:SEU_EMAIL@email.com">Email</a></li>
    </ul>
  </div>
</section>

<footer>
  <div class="wrap">
    Feito com dados, curiosidade e um pouco de café. ☕
  </div>
</footer>

</body>
</html>
