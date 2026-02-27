*[Read in English](README.md)*

# Bossa — Experimento de UI Design com Prompts Estruturados

Um experimento em geração de interfaces mobile de alta fidelidade usando apenas prompts estruturados alimentados em modelos de geração de imagem. Sem ferramentas de design. Sem Figma. Sem trabalho manual de pixel.

O objeto é uma corretora de investimentos brasileira fictícia chamada **Bossa** — um nome que remete à sofisticação discreta da Bossa Nova e à atitude de quem constrói.

---

## O que é isto

Este repositório contém os prompts, outputs e a metodologia por trás de um experimento: é possível sair do zero e chegar a uma UI de fintech mobile crível usando apenas linguagem natural e design tokens estruturados?

O objetivo não é substituir designers. É testar até onde o prompt engineering consegue empurrar a qualidade visual dos modelos de geração de imagem atuais, e documentar o processo com honestidade — o que funciona, o que quebra, e onde o julgamento humano continua sendo insubstituível.

---

## O briefing

Um app mobile-first de investimentos para um público brasileiro digitalmente nativo. Produtos principais: Tesouro Direto, Renda Fixa e Fundos. A identidade visual mistura a elegância cultural da Bossa Nova com a estética moderna de wealth management, com inspiração solta na linguagem limpa da Wealthfront sem copiar nenhum player diretamente.

Restrições principais:
- Dark theme, paleta baseada em índigo
- Não pode remeter visualmente a XP, Nubank, BTG, Rico ou Inter
- Frame de iPhone 15 (393 x 852px)
- Três telas: Home, Investimentos, Movimentações

---

## Estrutura do repositório

```
bossa-experiment/
  home-single-screen/
    prompt.md                       # Prompt de tela única (Home)
    home-single-screen.png          # Output gerado
  three-tabs-screens/
    prompt.md                       # Prompt com três telas lado a lado
    three-tabs-screens.png          # Output gerado
  README.md
  README-pt.md
```

---

## Resultados

### Tela Única — Home

A tela home concentra saldo, alocação do portfólio e transações recentes em uma única view com scroll.

[Ver prompt](home-single-screen/prompt.md)

<img src="home-single-screen/home-single-screen.png" alt="Home Tela Única" width="400">

### Três Abas — Home, Investimentos, Movimentações

Três telas apresentadas lado a lado, cada uma com sua aba correspondente ativa na navegação inferior.

[Ver prompt](three-tabs-screens/prompt.md)

![Três Abas](three-tabs-screens/three-tabs-screens.png)

---

## Metodologia

1. **Definir o contexto do produto.** Uma corretora fictícia mas plausível, com categorias de produto reais e dados realistas. A ficção precisa ser específica o suficiente para que o modelo não tenha desculpa para entregar algo genérico.

2. **Construir o prompt como uma spec de design.** Não uma descrição vaga — um documento estruturado com hierarquia de layout, definições de componentes, tokens de cor, escala tipográfica e regras de espaçamento. Quanto mais o prompt se parece com o que um desenvolvedor receberia de um designer, melhor o output.

3. **Estabelecer uma paleta de cores com intenção.** Cada escolha de cor foi feita para evitar associação direta com corretoras brasileiras existentes, mantendo credibilidade de fintech. A paleta foi derivada cruzando referências de concorrentes e deliberadamente desviando de seus identificadores primários.

4. **Gerar e avaliar.** Rodar o prompt no modelo, avaliar o output contra a spec, identificar lacunas e refinar. Cada iteração é preservada para comparação.

5. **Documentar com honestidade.** O ponto não é selecionar o melhor resultado. É mostrar a trajetória completa do prompt ao output, incluindo as falhas.

---

## Modelo

Os outputs foram gerados usando **Google Gemini** (capacidades de geração de imagem). Os prompts são agnósticos de modelo em sua estrutura, mas foram otimizados para a interpretação deste modelo específico de requisitos de design estruturados.

---

## Racional da paleta de cores

| Token            | Hex       | Papel                                     |
|------------------|-----------|-------------------------------------------|
| background       | #0C1222   | Índigo profundo — sofisticação noturna     |
| surfaceCard      | #141C2E   | Camada de cards — elevação sutil           |
| primaryAccent    | #4A7CFF   | Azul elétrico — confiança, tecnologia      |
| secondaryAccent  | #D4956A   | Terracota — calor, identidade brasileira   |
| success          | #34D399   | Verde menta — retornos positivos           |
| danger           | #F87171   | Vermelho coral — perdas, alertas           |

Deliberadamente evitados: preto/amarelo (XP), roxo (Nubank), azul escuro/branco (BTG), laranja (Rico, Inter).

---

## O que isto não é

- Isto não é um produto. A Bossa não existe.
- Isto não é um design system. Os tokens fazem parte do prompt, não de uma spec mantida.
- Isto não é uma afirmação de que IA substitui trabalho de design. É uma observação de onde a fronteira está hoje.

---

## Contexto

Este experimento faz parte de uma exploração mais ampla sobre fluxos de trabalho assistidos por IA para líderes de produto e tecnologia. O foco é prático: o que de fato dá pra prototipar ou entregar mais rápido com essas ferramentas, e onde você ainda precisa de craft humano?

---

## Autor

**Felipe Bossolani** — CPTO na Warren, ex-founder, 20+ anos em fintech.

Escrevendo sobre ferramentas de IA, product engineering e a intersecção entre liderança de tecnologia e craft prático em [bossolani.com](https://bossolani.com) e [LinkedIn](https://www.linkedin.com/in/bossolani/).

---

## Licença

Prompts e metodologia são abertos sob MIT. Faça o que quiser com eles. Se rodar o experimento por conta própria e obtiver resultados interessantes, compartilhe.