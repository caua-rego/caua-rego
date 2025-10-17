# Olá — eu sou Cauã Rego 👋

<!-- Hero SVG animado embutido: não precisa de assets externos -->
<div align="center">
  <svg width="100%" height="260" viewBox="0 0 1200 260" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Hero animado">
    <defs>
      <linearGradient id="g" x1="0" x2="1" y1="0" y2="1">
        <stop offset="0%" stop-color="#0f1724"/>
        <stop offset="50%" stop-color="#08101a"/>
        <stop offset="100%" stop-color="#071018"/>
      </linearGradient>
      <linearGradient id="grad" x1="0" x2="1">
        <stop offset="0%" stop-color="#7c3aed">
          <animate attributeName="offset" values="0;1;0" dur="8s" repeatCount="indefinite"/>
        </stop>
        <stop offset="100%" stop-color="#06b6d4">
          <animate attributeName="offset" values="1;0;1" dur="8s" repeatCount="indefinite"/>
        </stop>
      </linearGradient>
      <filter id="blur">
        <feGaussianBlur stdDeviation="30" />
      </filter>
    </defs>

    <!-- Fundo -->
    <rect width="1200" height="260" fill="url(#g)"/>

    <!-- Gradiente animado em forma orgânica -->
    <g opacity="0.6">
      <path d="M0 140 C200 50 400 250 600 160 C800 70 1000 210 1200 140 L1200 260 L0 260 Z"
            fill="url(#grad)" filter="url(#blur)">
        <animate attributeName="d" dur="12s" repeatCount="indefinite"
          values="
            M0 140 C200 50 400 250 600 160 C800 70 1000 210 1200 140 L1200 260 L0 260 Z;
            M0 150 C220 80 420 230 600 140 C780 50 980 240 1200 150 L1200 260 L0 260 Z;
            M0 135 C170 60 380 260 600 170 C820 80 1030 200 1200 135 L1200 260 L0 260 Z;
            M0 140 C200 50 400 250 600 160 C800 70 1000 210 1200 140 L1200 260 L0 260 Z"/>
      </path>
    </g>

    <!-- Partículas flutuantes -->
    <g fill="#58a6ff" opacity="0.08">
      <circle cx="180" cy="60" r="40">
        <animate attributeName="cy" values="60;40;60" dur="6s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0.08;0.18;0.08" dur="6s" repeatCount="indefinite"/>
      </circle>
      <circle cx="420" cy="30" r="28">
        <animate attributeName="cy" values="30;18;30" dur="5s" repeatCount="indefinite"/>
      </circle>
      <circle cx="860" cy="90" r="52">
        <animate attributeName="cy" values="90;70;90" dur="7s" repeatCount="indefinite"/>
      </circle>
      <circle cx="1050" cy="40" r="24">
        <animate attributeName="cy" values="40;20;40" dur="4s" repeatCount="indefinite"/>
      </circle>
    </g>

    <!-- Texto no hero -->
    <g fill="#cbd5e1" font-family="Inter, Roboto, sans-serif" text-anchor="middle">
      <text x="600" y="110" font-size="28" font-weight="700" fill="#e6eef8">Cauã Rego</text>
      <text x="600" y="145" font-size="16" fill="#9aa4b2">Desenvolvedor | UX consciente • Lógica de negócios robusta • Segurança</text>
    </g>
  </svg>
</div>

<p align="center">
  <a href="https://github.com/caua-rego"><img alt="Seguir" src="https://img.shields.io/github/followers/caua-rego?label=Seguir&style=for-the-badge&color=111827&logo=github"></a>
  <a href="https://github.com/caua-rego?tab=repositories"><img alt="Projetos" src="https://img.shields.io/badge/Projetos-🔭&style=for-the-badge&color=111827"></a>
  <a href="mailto:seu.email@exemplo.com"><img alt="Contato" src="https://img.shields.io/badge/Contato-✉️&style=for-the-badge&color=111827"></a>
</p>

---

## Sobre
Sou Cauã Rego — desenvolvedor focado em transformar requisitos complexos em interfaces e APIs claras, com atenção à experiência do usuário, segurança e consistência dos dados.

- Local: [Sua cidade, País]  
- Pronome: [ele/ela/they]  
- Aberto a: [Emprego / Freelance / Mentoria]

---

## Tecnologias (sugestão)
<p align="center">
  <img alt="TypeScript" src="https://img.shields.io/badge/-TypeScript-111827?style=flat-square&logo=typescript&logoColor=3178c6"/>
  <img alt="JavaScript" src="https://img.shields.io/badge/-JavaScript-111827?style=flat-square&logo=javascript&logoColor=f7df1e"/>
  <img alt="React" src="https://img.shields.io/badge/-React-111827?style=flat-square&logo=react&logoColor=61dafb"/>
  <img alt="Node.js" src="https://img.shields.io/badge/-Node.js-111827?style=flat-square&logo=node.js&logoColor=339933"/>
  <img alt="Postgres" src="https://img.shields.io/badge/-Postgres-111827?style=flat-square&logo=postgresql&logoColor=336791"/>
  <img alt="Docker" src="https://img.shields.io/badge/-Docker-111827?style=flat-square&logo=docker&logoColor=2496ed"/>
</p>

---

## Projetos em Destaque

<div align="center">
  <table role="presentation" cellspacing="12" cellpadding="8">
    <tr>
      <td align="left" valign="top" width="420" style="background:#071017;border-radius:12px;padding:18px;">
        <h3 style="margin:0 0 6px 0;color:#e6eef8">🔎 Focal App</h3>
        <p style="margin:0 0 10px 0;color:#9aa4b2">
          App focado em experiência do usuário e lógica de negócios.
        </p>
        <p style="margin:0 0 10px 0;color:#cbd5e1">
          Tech (detectado): <strong>TypeScript</strong><br/>
          Link: <a href="https://github.com/caua-rego/focal-app" style="color:#58a6ff">github.com/caua-rego/focal-app</a>
        </p>
      </td>

      <td align="left" valign="top" width="420" style="background:#071017;border-radius:12px;padding:18px;">
        <h3 style="margin:0 0 6px 0;color:#e6eef8">🏦 Bank Áurea</h3>
        <p style="margin:0 0 10px 0;color:#9aa4b2">
          Projeto bancário com ênfase em segurança, transações e consistência de dados.
        </p>
        <p style="margin:0 0 10px 0;color:#cbd5e1">
          Tech (detectado): <strong>CSS, Python, HTML</strong><br/>
          Link: <a href="https://github.com/caua-rego/bank-aurea" style="color:#58a6ff">github.com/caua-rego/bank-aurea</a>
        </p>
      </td>
    </tr>

    <tr>
      <td align="left" valign="top" colspan="2" width="860" style="background:#071017;border-radius:12px;padding:18px;">
        <h3 style="margin:0 0 6px 0;color:#e6eef8">📚 System Bank Education</h3>
        <p style="margin:0 0 10px 0;color:#9aa4b2">
          Repositório educativo para aprender CRUDs e lógica de programação.
        </p>
        <p style="margin:0 0 10px 0;color:#cbd5e1">
          Tech (detectado): <strong>Python</strong><br/>
          Link: <a href="https://github.com/caua-rego/system-bank-education" style="color:#58a6ff">github.com/caua-rego/system-bank-education</a>
        </p>
      </td>
    </tr>
  </table>
</div>

---

## Estatísticas
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=caua-rego&show_icons=true&theme=dark&hide_border=true" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=caua-rego&layout=compact&theme=dark&hide_border=true" alt="Top Languages" />
</p>
