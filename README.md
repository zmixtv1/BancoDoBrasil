# 🚀 StudyFlow: Plataforma Gamificada para Concursos de TI

> Uma aplicação web focada em produtividade e organização para o concurso do **Banco do Brasil (Agente de Tecnologia)** e TCU. Desenvolvida para contornar desafios de foco (TDAH) através de gamificação e feedback visual imediato.

![Status do Projeto](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow)
![Tecnologia](https://img.shields.io/badge/Tech-HTML%20%7C%20TailwindCSS%20%7C%20JavaScript-blue)

## 🎯 O Problema
Estudar para concursos de alto nível exige consistência e organização. Para perfis com TDAH, métodos tradicionais (planilhas estáticas) geram atrito e falta de motivação. Eu precisava de uma ferramenta que oferecesse:
- **Feedback Visual:** Barras de progresso para "sentir" o avanço.
- **Decisão Automatizada:** O sistema decide o que estudar hoje (fim da paralisia de escolha).
- **Recompensa Imediata:** Gamificação ao concluir tarefas.

## 💡 A Solução
Desenvolvi uma **Single Page Application (SPA)** leve e responsiva que gerencia todo o meu ciclo de estudos. O sistema combina cronogramas dinâmicos, simulados interativos e técnicas de foco (Pomodoro), tudo persistindo dados localmente no navegador.

### Funcionalidades Principais

* **📅 Cronograma Dinâmico & Cíclico:** O sistema gera automaticamente a pauta do dia (ex: *Manhã: Python / Tarde: Estatística*) baseado em listas cíclicas de tópicos, garantindo que todas as matérias do edital sejam cobertas.
* **🍅 Timer Pomodoro Integrado:** Modos de Foco (40min), Pausa Curta e Pausa Longa com alertas sonoros, integrados na sidebar para evitar distrações externas.
* **💾 Persistência de Dados (LocalStorage):** Todo o progresso (dias concluídos, questões respondidas) é salvo no navegador. O usuário pode fechar a aba e voltar sem perder nada.
* **📝 Simulados Interativos:**
    * **Modo Cesgranrio (BB):** Cálculo de nota percentual e feedback imediato de Certo/Errado.
    * **Modo Cebraspe (TCU):** Cálculo de nota líquida (Certo anula Errado).
* **🎨 UI Moderna (Glassmorphism):** Interface limpa e agradável com TailwindCSS para reduzir a fadiga visual durante longas sessões.

## 🛠️ Tecnologias Utilizadas

* **HTML5 Semantic:** Estrutura e acessibilidade.
* **CSS3 & TailwindCSS:** Estilização responsiva e efeitos visuais (Glassmorphism).
* **JavaScript (ES6+):**
    * Manipulação avançada do DOM.
    * Lógica de datas para geração do cronograma.
    * Manipulação de Arrays/Objetos para banco de questões.
    * `localStorage` API para salvar o estado da aplicação.

## 📂 Estrutura do Projeto

```bash
/
├── index.html          # Dashboard TCU
├── index2.html         # Dashboard Banco do Brasil (Foco Principal)
├── questoes2.html      # Simulado Interativo BB (Prova 2023)
├── GuiaEstudosTCU/     # Assets e arquivos complementares
└── README.md           # Documentação