<div align="center">

<img src="assets/banner.svg?v=2" width="100%" alt="Cauã Rêgo — Software Architect · Sistemas distribuídos · Event-driven · iGaming"/>

<img src="https://readme-typing-svg.demolab.com/?font=Cormorant+Garamond&weight=600&size=26&duration=3400&pause=1100&color=A3341F&center=true&vCenter=true&width=760&lines=Software+Architect;Sistemas+distribu%C3%ADdos+%C2%B7+Event-driven+%C2%B7+Performance;S%C3%B3cio+%26+Tech+Lead+%40+RVC;Co-founder+%26+CTO+%40+Operah;Autor+do+ATLAS+%E2%80%94+runtime+C%2B%2B23+escrito+do+zero" alt="typing"/>

<a href="https://www.linkedin.com/in/caua-dev/"><img src="https://img.shields.io/badge/LinkedIn-2b1d0e?style=for-the-badge&logo=linkedin&logoColor=d8b46a" alt="LinkedIn"/></a>
<a href="https://site-caua.vercel.app/"><img src="https://img.shields.io/badge/Portf%C3%B3lio_jog%C3%A1vel-2b1d0e?style=for-the-badge&logo=vercel&logoColor=d8b46a" alt="Portfólio"/></a>
<a href="mailto:cauaregoo12@gmail.com"><img src="https://img.shields.io/badge/E--mail-2b1d0e?style=for-the-badge&logo=gmail&logoColor=d8b46a" alt="E-mail"/></a>
<img src="https://komarev.com/ghpvc/?username=caua-rego&color=a3341f&style=for-the-badge&label=VISITANTES%20DO%20ATELI%C3%8A" alt="views"/>

</div>

<br/>

> *Software, como catedral, se mede pelo que sustenta — não pelo que enfeita.*

---

## I · Proêmio

Sou **arquiteto de software** em Recife. Desenho sistemas distribuídos orientados a eventos, com obsessão por previsibilidade: latência de cauda, consistência transacional e uma trilha auditável de cada real que entra e sai.

- 🏛️ **Sócio & Tech Lead @ RVC** — rede social gamificada de iGaming, com usuários reais e infraestrutura em produção
- 📐 **Co-founder & CTO @ Operah** — tecnologia sob medida para transformar complexidade operacional em clareza
- ⚙️ **Autor do [ATLAS](https://github.com/caua-rego/ATLAS)** — runtime em C++23 escrito do zero, P99.9 de scheduling **29× menor**
- 🎓 **CESAR School** — Análise e Desenvolvimento de Sistemas (2025 → 2027)

Antes disso, engenharia nas plataformas do **Grupo F12** (F12.bet · Luva.bet): clube VIP integrado à Smartico, cashback, instrumentação de funil e KPIs.

---

## II · De Architectura

Vitrúvio dizia que toda obra precisa de três virtudes. Eu traduzo assim:

| | Virtude | No software |
|---|---|---|
| 🧱 | ***Firmitas*** — solidez | Ação vira evento, crédito é idempotente, saldo vive em ledger. O sistema reconstrói o próprio estado a partir do histórico. |
| 📏 | ***Utilitas*** — utilidade | Arquitetura é decisão de negócio. Recompensa calibrada sobre NGR, não sobre volume apostado. Build vs. buy com custo na mesa. |
| ✨ | ***Venustas*** — beleza | Gamificação não é enfeite em cima do produto: é a estrutura que decide o que a pessoa faz primeiro. |

<div align="center">
<img src="assets/facade.svg?v=2" width="88%" alt="Fachada: produto sustentado por eventos, idempotência, ledger, observabilidade e compliance"/>
</div>

**Cânones da casa**

1. **Estrangule, não demola.** Strangler Fig em vez de reescrita total — o legado é conhecimento cristalizado.
2. **Regra em configuração.** Missão nova é uma entrada nova, não um `if` em cinco arquivos.
3. **Uma torneira, um ralo.** Toda economia de pontos tem fonte e escoamento explícitos — e um teto amarrado ao resultado.
4. **Documente o porquê.** ADR para cada decisão que alguém vai querer desfazer daqui a seis meses.
5. **Meça a cauda, não a média.** P99 conta a verdade que a média esconde.

---

## III · Opera Magna

### ⚙️ [ATLAS](https://github.com/caua-rego/ATLAS) — *Adaptive Telemetry & Learning Allocation System*

Runtime **C++23** que mantém a latência de cauda estável quando workloads disputam CPU e memória. Sem patch de kernel, sem JIT, sem dependências externas.

| Métrica | Threads do SO | ATLAS | Ganho |
|---|---:|---:|---:|
| Scheduling P99.9 | 4.291 µs | 148 µs | **29×** |
| Alocação de memória P99 | 1.847 µs | 39 µs | **47×** |
| Context switch P99 | 156 µs | 42 µs | **3,7×** |

```
 Control Plane  │ Q-learning híbrido · policy versioning com rollback · governance hooks
 Scheduler      │ fibers com context switch em assembly (x86_64 + AArch64) · Chase-Lev work-stealing
 Memory         │ arena lock-free · buddy com bitmap · slab · NUMA-aware lendo /sys
 Telemetry      │ causal tracer em ring buffer lock-free · crash handler
```

<sub>64 testes · CI com GCC 14, Clang 18 e macOS · ASan + TSan · Docker multi-stage · MIT</sub>

### Outras obras do ateliê

| Obra | O que é | Materiais |
|---|---|---|
| 🎲 **[Portfólio jogável](https://site-caua.vercel.app/)** | Um currículo que se explora: missões, terminal real, 26 registros escondidos e uma economia de fichas 50/50, sem margem da casa. Progresso derivado de eventos. | React · TypeScript · Vite |
| 🤖 **[Aura Copilot](https://github.com/caua-rego/aura-ai)** | Copiloto de código com LLMs locais — privacidade, baixa latência e arquitetura com dois modelos (conversa + código). Base para pesquisa científica. | Python · Tauri (Rust) · React 19 |
| 🏦 **[Bank Áurea](https://github.com/caua-rego/bank-aurea)** | Plataforma bancária em camadas: autenticação, transferências e rate limiting. | TypeScript |
| 🏥 **[FluiSaúde](https://github.com/caua-rego/fluisaude)** | Gestão para Unidades Básicas de Saúde. Squad vencedor na CESAR School. | TypeScript |
| 🍸 **The Boolean Bar** | Jogo multiplayer de lógica e blefe: engine em C11, gateway Node.js via IPC, anti-cheat por filtragem por cliente. | C11 · Node.js · React 19 |

---

## IV · La Bottega — *as ferramentas do ateliê*

<div align="center">

**Linguagens**

<img src="https://img.shields.io/badge/C%23-2b1d0e?style=for-the-badge&logo=dotnet&logoColor=d8b46a"/> <img src="https://img.shields.io/badge/C%2B%2B23-2b1d0e?style=for-the-badge&logo=cplusplus&logoColor=d8b46a"/> <img src="https://img.shields.io/badge/TypeScript-2b1d0e?style=for-the-badge&logo=typescript&logoColor=d8b46a"/> <img src="https://img.shields.io/badge/Python-2b1d0e?style=for-the-badge&logo=python&logoColor=d8b46a"/> <img src="https://img.shields.io/badge/SQL-2b1d0e?style=for-the-badge&logo=postgresql&logoColor=d8b46a"/>

**Plataforma & Infra**

<img src="https://img.shields.io/badge/.NET-2b1d0e?style=for-the-badge&logo=dotnet&logoColor=d8b46a"/> <img src="https://img.shields.io/badge/Node.js-2b1d0e?style=for-the-badge&logo=nodedotjs&logoColor=d8b46a"/> <img src="https://img.shields.io/badge/Azure-2b1d0e?style=for-the-badge&logo=microsoftazure&logoColor=d8b46a"/> <img src="https://img.shields.io/badge/Docker-2b1d0e?style=for-the-badge&logo=docker&logoColor=d8b46a"/> <img src="https://img.shields.io/badge/CMake-2b1d0e?style=for-the-badge&logo=cmake&logoColor=d8b46a"/>

**Interface**

<img src="https://img.shields.io/badge/React-2b1d0e?style=for-the-badge&logo=react&logoColor=d8b46a"/> <img src="https://img.shields.io/badge/React_Native-2b1d0e?style=for-the-badge&logo=react&logoColor=d8b46a"/> <img src="https://img.shields.io/badge/.NET_MAUI-2b1d0e?style=for-the-badge&logo=dotnet&logoColor=d8b46a"/> <img src="https://img.shields.io/badge/Tauri-2b1d0e?style=for-the-badge&logo=tauri&logoColor=d8b46a"/>

</div>

**Domínio — iGaming:** gamificação (níveis, missões, streaks, economia de pontos) · CRM e cashback · GGR, NGR, hold, LTV · Pix, KYC, antifraude, LGPD · wallet com consistência transacional.

---

## V · Cronaca

| | Casa | Ofício | Período |
|---|---|---|---|
| 🏛️ | **RVC** | Sócio & Tech Lead | jun/2026 → hoje |
| 📐 | **Operah** | Co-founder & CTO | fev/2026 → hoje |
| 🎰 | **F12 do Brasil** · F12.bet · Luva.bet | Especialista em Desenvolvimento de Software | abr/2026 → out/2026 |
| 🧭 | **Daus** | Software Engineer | out/2025 → abr/2026 |
| 🪶 | **Autônomo** | Desenvolvedor — projetos próprios e sob demanda | 2019 → 2025 |

---

## VI · Registro do ateliê

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=caua-rego&show_icons=true&include_all_commits=true&count_private=true&hide_border=false&bg_color=f6ecd6&title_color=a3341f&icon_color=1f3a6b&text_color=3d2814&border_color=b8893b&custom_title=Registro%20do%20Ateli%C3%AA"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=caua-rego&layout=compact&bg_color=f6ecd6&title_color=a3341f&text_color=3d2814&border_color=b8893b&custom_title=Pigmentos"/>

<img src="https://streak-stats.demolab.com?user=caua-rego&background=f6ecd6&border=b8893b&stroke=b8893b&ring=a3341f&fire=a3341f&currStreakNum=2b1d0e&sideNums=2b1d0e&currStreakLabel=a3341f&sideLabels=3d2814&dates=7a5230&locale=pt_BR" alt="streak"/>

</div>

---

<div align="center">

*Firmitas · Utilitas · Venustas*

<sub>Recife, Pernambuco — Brasil</sub>

</div>
