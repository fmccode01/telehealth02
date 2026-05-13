# Ecossistema Digital de Cuidado em Obesidade

Protótipos clicáveis do programa B2C de telehealth para obesidade · Lilly Brazil · Medical Affairs Obesidade.

## 🎯 Como usar

Acesse o link do GitHub Pages (Settings → Pages → ative · em ~1 min seu link aparece).

Ou baixe os arquivos e abra `index.html` direto no browser.

## 📁 Arquivos

- **`index.html`** · landing page com links para os dois protótipos
- **`patient-view.html`** · experiência do paciente em 5 modos
- **`control-center.html`** · centro de comando do clínico

## 🌱 Patient View · o que o paciente vê e sente

5 modos navegáveis pelo topo:

| Modo | Conteúdo |
|---|---|
| Primeira vez | Onboarding com sex-gating, fertilidade, gestação, comorbidades |
| Pré-consulta | Snapshot pra clínico, com SentimentMap pré-consulta |
| Em acompanhamento | Microcheck, FNQ, peso, momentos da vida |
| Árvore de decisão | Como o sistema decide alertar/escalonar |
| Entender pra cuidar | Biblioteca educacional sobre obesidade |

## 🎯 Control Center · torre de comando do pool

6 views via sidebar e topbar:

| View | Conteúdo |
|---|---|
| 🎯 Ação | Pacientes que precisam intervenção agora (críticos + atenção) |
| 👥 Todos | Lista alfabética completa, busca, filtros |
| 📊 Coorte | **13 análises macro com tooltips clínicos interativos** + glossário de 37 siglas |
| ⚡ Triggers | 4 dimensões: volume · recorrência · clusters · predição |
| 📅 Hoje | Timeline cronológica do dia · pool compartilhado |
| 🌳 Decisões | Alertas compostos · combinações de triggers · árvore de decisão |

**Recursos chave:**
- Sistema **Endereçar** · check de tarefa que move pacientes de crítico/atenção → fluxo
- **Tooltips em todos os gráficos** das 13 análises macro (passe o mouse · veja contexto clínico)
- **Modais funcionais** pra cada ação (vídeo · ligar · prescrever · prescrever exames · etc)
- **Exportador de 4 etapas:**
  1. Selecionar análises (6 presets · 34 análises individuais)
  2. Cenários (8 filtros · 5 comparações)
  3. Preview com marca d'água
  4. Email + agendamento

## 🛠 Stack

- React 18 (via CDN unpkg.com)
- Babel standalone (transpilação no browser)
- CSS puro com variables (CSS custom properties)
- Google Fonts (Cormorant Garamond · Source Sans 3 · JetBrains Mono)
- **Zero build step · zero npm install · zero servidor**

## 🚀 Deploy no GitHub Pages

1. Settings (engrenagem) → Pages
2. Source: **Deploy from a branch**
3. Branch: **main** · Folder: **/ (root)**
4. Save
5. Em ~1 minuto seu link aparece em verde no topo da página

Acesse `https://SEUUSUARIO.github.io/NOME-DO-REPO/` (vai cair na index.html que tem os botões pra cada protótipo).

## ⚠️ Disclaimers

- Conteúdo de uso interno · não para distribuição pública
- Instrumentos validados (PHQ-9, GAD-7, STOP-BANG) são domínio público
- FNQ, SentimentMap e ECAP são paráfrases conceituais · não substituem instrumentos originais para uso regulatório
- IWQOL-Lite (proprietário Kolotkin et al.) · apenas domínios são listados
- Dados de pacientes nos protótipos são mockados · sem informação real

## 📐 Para engenharia

A view "Decisões" do Control Center tem **painel preto com pseudocódigo** explicando a lógica de alertas compostos · base pra implementação real do backend.

Tooltips em "Triggers" mostram regras técnicas (`IF condition THEN trigger`), cooldowns e atores responsáveis · documentação inline pra dev.

## 📞 Contato

Lilly Brazil · Medical Affairs · Programa de Obesidade

---

*"Decisão final é sempre clínica."*
