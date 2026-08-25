<div align="center">

# 🛡️ Segurança Digital para Você

### Um guia interativo que ensina a reconhecer golpes digitais em menos de 3 minutos

[![Acessar o site](https://img.shields.io/badge/🌐_Acessar_o_site-2C5F5A?style=for-the-badge)](https://marceladrumond.github.io/seguranca-digital-idosos/)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Sem build step](https://img.shields.io/badge/build-nenhum-brightgreen?style=flat-square)
![Custo](https://img.shields.io/badge/custo-R%240-success?style=flat-square)

</div>

---

## 📖 Sobre o projeto

Golpes de Pix, clonagem de WhatsApp e links falsos fazem milhares de vítimas todos os
anos — e idosos são um dos alvos favoritos, muitas vezes por não terem tido contato
próximo com esse tipo de armadilha antes. Este projeto existe pra mudar isso de um
jeito simples: sem cadastro, sem letra miúda, sem jargão técnico.

Pensado pra ser acessado por QR Code em uma sala de espera (o piloto foi feito para uma
clínica de fisioterapia), a pessoa aprende em poucos minutos a reconhecer os 3 golpes
mais comuns hoje no Brasil, testa o que aprendeu num quiz com feedback imediato, e ainda
pode ouvir o conteúdo em voz alta, aumentar o contraste e o tamanho do texto, ou levar
um guia impresso pra casa.

Um **Projeto de Extensão** do curso de Análise e Desenvolvimento de Sistemas (ADS) do
**CEU Anhanguera**, pensado de ponta a ponta com o público idoso em mente.

## ✨ Funcionalidades

**Conteúdo educativo**
- 3 cards explicando os golpes mais comuns: Pix bloqueado, WhatsApp clonado (com alerta
  sobre clonagem de voz por Inteligência Artificial) e links de prêmios falsos
- Quiz de 3 perguntas com feedback específico pra cada resposta errada — sem punir
  quem erra, só explicando o porquê
- Toque em outra alternativa pra tentar de novo, na hora, sem botões extras

**Acessibilidade em primeiro lugar**
- Alto contraste e tipografia grande desde o início — não é um "modo especial", é o
  padrão da página
- Botão de acessibilidade que aumenta o texto e o contraste ainda mais, com a
  preferência salva entre visitas
- Botão "Ouvir" em cada pergunta e explicação, usando a Web Speech API do navegador
- Navegação completa por teclado, com foco bem gerenciado a cada transição de tela

**Pra levar consigo**
- Guia em PDF de 1 página só, com impressão otimizada — sem depender de nenhuma
  biblioteca externa
- Exportação dos resultados do quiz em CSV
- Compartilhamento direto com um familiar pelo WhatsApp

Tudo isso rodando **100% no navegador** — sem servidor, sem banco de dados, sem custo
de hospedagem.

## 🔗 Acesse

**[marceladrumond.github.io/seguranca-digital-idosos](https://marceladrumond.github.io/seguranca-digital-idosos/)**

## 🛠️ Tecnologias

Propositalmente simples — sem framework, sem build step, sem `npm install`:

| | |
|---|---|
| **Estrutura** | HTML5 semântico |
| **Estilo** | CSS puro — variáveis CSS, zero dependência de CDN de framework |
| **Interatividade** | JavaScript puro (vanilla, ES2017+) |
| **Fontes** | Google Fonts (Inter + Manrope) |
| **Voz** | Web Speech API, nativa do navegador |
| **Hospedagem** | GitHub Pages |

## 🚀 Rodando localmente

Não precisa instalar nada:

```bash
git clone https://github.com/MarcelaDrumond/seguranca-digital-idosos.git
cd seguranca-digital-idosos
python -m http.server 8000
```

Acesse `http://localhost:8000` — ou simplesmente abra o `index.html` direto no
navegador.

## 📁 Estrutura do projeto

```
seguranca-digital-idosos/
├── index.html      # conteúdo e estrutura da página
├── style.css       # design tokens, utilitários e CSS de impressão
├── script.js       # lógica do quiz e das funcionalidades extras
├── assets/         # imagens (hero + logo)
└── README.md
```

## ⚙️ Configuração

O formulário de feedback pós-quiz ("Isso te ajudou?", exibido depois do resultado) **já
está configurado e ativo**, usando o Google Forms embutido via iframe.

Pra trocar pelo seu próprio formulário: edite a constante `GOOGLE_FORM_URL` no topo do
`script.js` com o link de incorporação do seu Google Form (Forms → Enviar → aba `<>` →
copiar a URL do `src`). Se o valor ficar vazio, essa seção some automaticamente — nada
quebra.

## 🤖 Construção e desenvolvimento

Este projeto foi construído em parceria com o
**[Claude Code](https://claude.com/claude-code)**, da Anthropic — do design inicial até
os últimos ajustes de acessibilidade. O processo incluiu:

- Levantamento de requisitos e definição de paleta/tipografia antes de escrever
  qualquer linha de código
- Implementação iterativa, com verificação real no navegador a cada mudança
- Uma auditoria de segurança completa antes da publicação — sem chaves ou segredos
  expostos, sem vulnerabilidades de XSS, histórico do Git limpo
- Revisão de acessibilidade em cada etapa: contraste, navegação por teclado, leitura em
  voz alta, tamanho das áreas de toque

A ideia não foi só gerar código, mas usar a IA como parceira real de desenvolvimento —
testando, revisando e refinando até o resultado ficar pronto pra uso de verdade por
pessoas de verdade.

## 👥 Créditos

Projeto de Extensão — **ADS × CEU Anhanguera**

## 📄 Licença

Projeto de uso educativo e gratuito. Sinta-se livre pra adaptar para sua própria
instituição ou iniciativa social.
