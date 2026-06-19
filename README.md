<!-- Pedro Pandolfi — GitHub Profile README -->

<h1 align="center">Pedro Pandolfi</h1>
<h3 align="center">Analista de Sistemas · Espírito Santo, Brasil</h3>

<p align="center">
  Desenvolvimento web e sistemas empresariais — com foco em eletrônica embarcada,<br/>
  engenharia reversa automotiva (VAG/PQ35) e ferramentas para assistentes de código com IA.
</p>

<p align="center">
  <a href="https://pandolfi.tech" target="_blank">
    <img src="https://img.shields.io/badge/Site-pandolfi.tech-0A0A0A?style=for-the-badge" />
  </a>
  <a href="https://linkedin.com/in/pandolfipedro" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://instagram.com/pandolfipedro" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" />
  </a>
</p>

---

## Sobre mim

- 💼 Analista de Sistemas — aplicações web, backends e integrações empresariais
- 🚗 Projetos open source na plataforma **VW PQ35/PQ46** — emulação CAN, long coding MK60EC1 e documentação K-Matrix
- ⚡ Eletrônica embarcada — **ESP32**, **MCP2515**, CAN bus 500 kbps, OBD-II
- 🤖 Ferramentas para IA — **MCP server** local com indexação de código e orçamento de tokens
- 📊 Exploração de dados aplicada ao domínio automotivo (EDA, telemetria, dashboards)

---

## Stack

### Web, Backend & Dados

<p align="left">
  <img src="https://cdn.simpleicons.org/typescript/3178C6" height="30" title="TypeScript" />&nbsp;
  <img src="https://cdn.simpleicons.org/javascript/F7DF1E" height="30" title="JavaScript" />&nbsp;
  <img src="https://cdn.simpleicons.org/react/61DAFB" height="30" title="React" />&nbsp;
  <img src="https://cdn.simpleicons.org/nodedotjs/339933" height="30" title="Node.js" />&nbsp;
  <img src="https://cdn.simpleicons.org/express/000000" height="30" title="Express" />&nbsp;
  <img src="https://cdn.simpleicons.org/php/777BB4" height="30" title="PHP" />&nbsp;
  <img src="https://cdn.simpleicons.org/mysql/4479A1" height="30" title="MySQL" />&nbsp;
  <img src="https://cdn.simpleicons.org/postgresql/4169E1" height="30" title="PostgreSQL" />&nbsp;
  <img src="https://cdn.simpleicons.org/python/3776AB" height="30" title="Python" />&nbsp;
  <img src="https://cdn.simpleicons.org/docker/2496ED" height="30" title="Docker" />&nbsp;
  <img src="https://cdn.simpleicons.org/html5/E34F26" height="30" title="HTML5" />&nbsp;
  <img src="https://cdn.simpleicons.org/sass/CC6699" height="30" title="Sass" />
</p>

### Embarcada, CAN & Sistemas

<p align="left">
  <img src="https://cdn.simpleicons.org/cplusplus/00599C" height="30" title="C++" />&nbsp;
  <img src="https://cdn.simpleicons.org/arduino/00979D" height="30" title="Arduino / ESP32" />&nbsp;
  <img src="https://cdn.simpleicons.org/socketdotio/010101" height="30" title="Socket.io" />&nbsp;
  <img src="https://cdn.simpleicons.org/prisma/2D3748" height="30" title="Prisma" />&nbsp;
  <img src="https://cdn.simpleicons.org/git/F05032" height="30" title="Git" />&nbsp;
  <img src="https://cdn.simpleicons.org/gnubash/4EAA25" height="30" title="Bash / Terminal" />
</p>

---

## Projetos em destaque

### 🤖 [ContextCache MCP](https://github.com/pandolfipedro/contextcache-mcp)

> Servidor **MCP** local e budget-aware que monta **Context Packs** mínimos para assistentes de código — grafo de dependências, SQLite, indexação AST, sem APIs pagas.

**Stack:** `TypeScript` · `MCP` · `SQLite` · `Node.js 20+` · `Cursor` · `Claude Code`  
**Tools:** `get_context_pack` · `get_file_summary` · indexação incremental por `content_hash`

---

### 🚗 [PQ35 ABS Emulator](https://github.com/pandolfipedro/pq35-abs-emulator) · v2.0

> Emulador open source do módulo **Bosch MK60EC1** para **VW PQ35/PQ46** (Jetta MK5, Golf MK5).  
> Lê velocidade via OBD **0x7E1 → 0x7E9 PID 0x0D** (TCU 09G) e transmite frames `Bremse_*` no CAN — restaura **velocímetro** e **hodômetro** sem o módulo ABS original.

> ⚠️ **Não restaura frenagem ABS.** Apenas mensagens CAN. Use por sua conta e risco.

**Stack:** `ESP32` · `MCP2515` · `ACAN2515` · `CAN 500 kbps` · `C++` · DBC [`vw_pq.dbc`](https://github.com/pandolfipedro/pq35-abs-emulator/blob/main/docs/vw_pq.dbc)  
**Frames:** `0x1A0` · `0x4A0` · `0x4A8` · `0x5A0` · `0x3A0` · KMatrix PQ35/46 V5.20.6F

---

### 🔧 [MK60EC1 Long Code](https://github.com/pandolfipedro/mk60ec1-longcode)

> Calculadora offline (HTML estático) — **VIN + módulo ABS** → long code hex para **VCDS**.  
> Foco em Jetta importado BR **2009–2016** · módulos **1K0907379 AD/BL/CC**.

**Recursos:** tamanhos de freio 280/288/312 mm · modo ESP/ASR · helper byte-a-byte · migração entre índices de módulo

---

### 📡 [CAN PQ35 — KMatrix Reference](https://github.com/pandolfipedro/pq35-abs-emulator/blob/main/CAN_PQ35.md)

> Referência de sinais CAN para PQ35/PQ46 baseada na K-Matrix oficial VW (V5.20.6F), com notas de implementação em C++.

**Cobertura:** `mBremse_1 (0x1A0)` · `mBremse_2 (0x5A0)` · `mBremse_3 (0x4A0)` · `mBremse_5 (0x4A8)`

---

### 📊 Outros projetos

| Projeto | Descrição |
|---------|-----------|
| [**telemetry-cloud**](https://github.com/pandolfipedro/telemetry-cloud) | Portal full stack de telemetria OBD-II/CAN — ESP32 → WebSocket → dashboard em tempo real |
| [**eda-veiculos**](https://github.com/pandolfipedro/eda-veiculos) | EDA em Python sobre preços e performance de automóveis (UCI Automobile) |
| [**SEFAZ-ES-QR-Code**](https://github.com/pandolfipedro/SEFAZ-ES-QR-Code) | Leitura de cupons fiscais via QR Code + integração SEFAZ |

---

<p align="center">
  <i>Aberto a colaborações em projetos automotivos, embarcados e ferramentas para desenvolvedores.</i>
</p>
