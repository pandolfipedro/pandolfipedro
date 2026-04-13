<!-- Pedro Pandolfi — GitHub Profile README -->

<h1 align="center">Pedro Pandolfi</h1>
<h3 align="center">Analista de Sistemas · Espírito Santo, Brasil</h3>

<p align="center">
  Desenvolvimento de sistemas e aplicações web — com experiência em eletrônica embarcada,<br/>
  engenharia reversa automotiva e integração de hardware com software.
</p>

<p align="center">
  <a href="https://linkedin.com/in/pandolfipedro" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://instagram.com/pandolfipedro" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" />
  </a>
</p>

---

## Sobre mim

- 💼 Analista de Sistemas com atuação em desenvolvimento web e sistemas empresariais
- ⚡ Entusiasta de eletrônica embarcada — ESP32, CAN bus, protocolos automotivos
- 🔬 Curioso por engenharia reversa e protocolos industriais (VAG KMatrix, OBD2, CAN ISO 11898)
- 🚗 Criador do **PQ35 ABS Emulator** — projeto open source de emulação de módulo ABS para VW

---

## Stack Web & Backend

<p align="left">
  <img src="https://cdn.simpleicons.org/html5/E34F26" height="30" title="HTML5" />&nbsp;
  <img src="https://cdn.simpleicons.org/sass/CC6699" height="30" title="Sass" />&nbsp;
  <img src="https://cdn.simpleicons.org/javascript/F7DF1E" height="30" title="JavaScript" />&nbsp;
  <img src="https://cdn.simpleicons.org/react/61DAFB" height="30" title="React" />&nbsp;
  <img src="https://cdn.simpleicons.org/nodedotjs/339933" height="30" title="Node.js" />&nbsp;
  <img src="https://cdn.simpleicons.org/php/777BB4" height="30" title="PHP" />&nbsp;
  <img src="https://cdn.simpleicons.org/mysql/4479A1" height="30" title="MySQL" />
</p>

## Stack Embarcada & Sistemas

<p align="left">
  <img src="https://cdn.simpleicons.org/cplusplus/00599C" height="30" title="C++" />&nbsp;
  <img src="https://cdn.simpleicons.org/arduino/00979D" height="30" title="Arduino / ESP32" />&nbsp;
  <img src="https://cdn.simpleicons.org/swift/F05138" height="30" title="Objective-C / iOS" />&nbsp;
  <img src="https://cdn.simpleicons.org/git/F05032" height="30" title="Git" />&nbsp;
  <img src="https://cdn.simpleicons.org/gnubash/4EAA25" height="30" title="Bash / Terminal" />&nbsp;
</p>

---

## Projetos em destaque

### 🚗 [PQ35 ABS Emulator](https://github.com/pandolfipedro/pq35-abs-emulator)

> Emulador open source de módulo ABS/ESP para a plataforma **VW PQ35/PQ46** (Jetta MK5, Golf MK5, Beetle TSI).  
> Substitui o módulo Bosch MK60EC1 no barramento CAN, restaurando velocímetro, hodômetro e Cruise Control  
> sem o módulo ABS original instalado.

**Stack:** `ESP32` · `MCP2515 + TJA1050` · `ACAN2515` · `CAN bus 500kbps` · `C++` · `OBD2 PID 0x0D`  
**Protocolo:** KMatrix PQ35/46 V5.20.6F · Mensagens `0x1A0` `0x4A0` `0x4A8` `0x5A0` `0xDA0`

---

### 📡 [CAN PQ35 — KMatrix Reference](https://github.com/pandolfipedro/pq35-abs-emulator/blob/main/CAN_PQ35.md)

> Tabela de referência de sinais CAN para a plataforma PQ35/PQ46, baseada no PDF oficial da K-Matrix da VW  
> (V5.20.6F). Documenta todos os sinais relevantes para emulação de ABS/ESP com comentários de implementação em C++.

**Cobertura:** `mBremse_1 (0x1A0)` · `mBremse_2 (0x5A0)` · `mBremse_3 (0x4A0)` · `mBremse_5 (0x4A8)`  
**Utilidade:** Referência para projetos de emulação CAN na plataforma VAG

---

