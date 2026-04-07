# 🩸 PerkLab — Dead by Daylight Build Tool

> Ferramenta web completa para montar e gerenciar builds de Dead by Daylight — ideal para campeonatos, análise de meta e uso competitivo.

![Dead by Daylight](https://img.shields.io/badge/Dead%20by%20Daylight-Build%20Tool-red?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0iI2ZmZiIgZD0iTTEyIDJMMiAyMmgyMEwxMiAyeiIvPjwvc3ZnPg==)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![LocalStorage](https://img.shields.io/badge/Persistência-LocalStorage-green?style=for-the-badge)

---

## 📸 Preview

| Dark Mode | Light Mode |
|-----------|------------|
| Builder com perks de Killer/Survivor | Sistema de perfis salvos |
| Tier List completa | Modo Campeonato |

---

## ✨ Funcionalidades

### 🔨 Builder de Builds
- **200+ perks** catalogados — todos os Killers e Survivors até 2024
- Filtros por **personagem**, **tier (S/A/B/C/D)** e **busca por texto**
- Slots visuais com **tooltip detalhado** (descrição completa, origem, tier)
- Build **aleatório** com 1 clique
- **Exportar build** para clipboard formatado

### 👤 Sistema de Perfis
- Salva builds com nome personalizado via **LocalStorage** (persiste entre sessões)
- Visualização com mini-preview dos perks e badge de role
- **Editar** e **deletar** perfis salvos
- Suporte a múltiplos perfis de Killer e Survivor

### 📊 Tier List
- Todos os perks classificados em tiers **S / A / B / C / D**
- Alternância entre Killer e Survivor
- Filtro de busca em tempo real

### 🏆 Modo Campeonato
- Setup completo de **1 Killer + 4 Survivors**
- Campo de nome por jogador
- Seletor de perks via modal para cada slot
- **Exportar lineup completo** para clipboard (ideal para organização de torneios)

### 🌗 Dark / Light Mode
- Toggle instantâneo com memória salva
- Paleta temática fiel ao universo do jogo

---

## 🚀 Como Usar

Este projeto é 100% **client-side** — sem backend, sem dependências, sem instalação.

### Opção 1 — Abrir diretamente
```bash
# Clone o repositório
git clone https://github.com/seu-usuario/perklab.git

# Abra o arquivo no navegador
open index.html
```

### Opção 2 — Deploy estático
Faça upload do `index.html` em qualquer serviço de hospedagem estática:

- **GitHub Pages** — vá em `Settings > Pages > Deploy from branch`
- **Netlify** — arraste o arquivo para [app.netlify.com/drop](https://app.netlify.com/drop)
- **Vercel** — `vercel --prod`

---

## 🗂️ Estrutura do Projeto

```
PerkLab/
└── index.html       # Aplicação completa em arquivo único
```

O projeto foi desenvolvido como **single-file app** para máxima portabilidade — basta compartilhar o arquivo.

---

## 🧠 Perks Incluídos

### Killers (116 perks)
| Personagem | Perks Notáveis |
|------------|----------------|
| The Nurse | Save The Best For Last, A Nurse's Call |
| The Hag | Hex: Ruin, Hex: Devour Hope |
| The Cannibal | Barbecue & Chili (BBQ), Knock Out |
| The Plague | Corrupt Intervention, Infectious Fright |
| The Deathslinger | Dead Man's Switch, Gearhead |
| The Pinhead | Deadlock, Hex: Plaything |
| The Artist | Scourge Hook: Pain Resonance, Grim Embrace |
| Xenomorph | Ultimate Weapon |
| Dracula | Hex: Undying |
| ...e muito mais | Todos os killers do lançamento até 2024 |

### Survivors (107 perks)
| Personagem | Perks Notáveis |
|------------|----------------|
| Meg Thomas | Sprint Burst, Adrenaline |
| Laurie Strode | Decisive Strike, Sole Survivor |
| Bill Overbeck | Borrowed Time, Unbreakable |
| David King | Dead Hard |
| Feng Min | Lithe |
| Jeff Johansen | Distortion, Head On |
| Kate Denson | Windows of Opportunity |
| Nicolas Cage | Dramaturgy, Scene Partner |
| Gabriel Soma | Made For This |
| Sable Ward | Weave Attunement |
| ...e muito mais | Todos os survivors do lançamento até 2024 |

---

## 🏆 Uso em Campeonatos

O **Modo Campeonato** foi pensado para:

- **Organisers** registrarem builds de cada equipe antes da partida
- **Comentaristas** consultarem os perks durante a transmissão
- **Jogadores** documentarem suas estratégias de torneio
- **Exportar** o setup completo para Discord, Google Sheets ou sheets de meta

### Fluxo sugerido para torneios:
1. Abra a aba **🏆 Campeonato**
2. Insira os nomes dos jogadores
3. Selecione os perks de cada um via modal
4. Clique em **📋 Exportar** para copiar o lineup formatado
5. Cole no canal do torneio ou na planilha de acompanhamento

---

## 💾 Persistência de Dados

Todos os dados são salvos localmente via `localStorage`:

| Chave | Conteúdo |
|-------|----------|
| `dbdProfiles` | Array de builds salvos |
| `dbdChamp` | Setup atual do campeonato |
| `dbdTheme` | Preferência de tema (dark/light) |

> **Atenção:** Os dados ficam no navegador. Limpar o cache apaga os perfis. Para backup, use a função **Exportar**.

---

## 🛠️ Tecnologias

- **HTML5** puro — sem frameworks
- **CSS3** com variáveis customizadas para theming
- **Vanilla JavaScript** — sem dependências externas
- **Google Fonts** — Bebas Neue, Rajdhani, Share Tech Mono
- **localStorage API** — persistência de dados

---

## 📋 Roadmap

- [ ] Importar build via código compartilhável (URL params)
- [ ] Sistema de votação de tier list colaborativo
- [ ] Comparador de builds (A vs B)
- [ ] Histórico de partidas em campeonatos
- [ ] PWA (Progressive Web App) para uso offline
- [ ] Suporte a add-ons e offerings
- [ ] Integração com DBD API (quando disponível)

---

## 🤝 Contribuindo

Pull requests são bem-vindos! Para mudanças maiores, abra uma issue primeiro para discutirmos.

```bash
# Fork o projeto
# Crie sua feature branch
git checkout -b feature/nova-funcionalidade

# Commit suas mudanças
git commit -m 'feat: adiciona nova funcionalidade X'

# Push para a branch
git push origin feature/nova-funcionalidade

# Abra um Pull Request
```

---

## ⚖️ Aviso Legal

Este projeto é um **fan-made tool** não oficial. Dead by Daylight é propriedade da **Behaviour Interactive**. Todos os nomes de personagens e perks pertencem aos seus respectivos detentores. Este projeto não possui afiliação com a Behaviour Interactive.

---

## 📄 Licença

[MIT](LICENSE) — use, modifique e distribua livremente.

---

<div align="center">
  Feito com 🩸 para a comunidade de Dead by Daylight
  <br><br>
  <b>⭐ Se este projeto te ajudou, deixa uma estrela!</b>
</div>
