# Primeiros passos em Python

Material introdutório de Python com slides em Reveal.js e notebooks Jupyter. A primeira aula aplica os fundamentos ao cálculo de consumo e custo de energia; a segunda pratica sorteios, repetição e decisões com jogos.

**Autor:** Waldsson Sacramento dos Santos.

## Proposta da aula

O material foi preparado para quem está começando a programar. A apresentação explica os conceitos antes de demonstrá-los em código, com saídas de terminal e um diagrama de decisão. O notebook complementa a aula com exemplos executáveis, exercícios e um projeto guiado.

A sequência sugerida é apresentar os fundamentos nos slides e, em seguida, executar os exemplos no notebook. Os exercícios também podem ser usados para estudo posterior.

## Aula 1 — Python para entender o consumo de energia

- Introdução à programação, ao Python e ao Jupyter Notebook.
- Saída de informações com `print()`.
- Variáveis, atribuição e tipos de dados.
- Operadores aritméticos.
- F-strings e formatação decimal.
- Entrada de dados e conversão de tipos.
- Comparações, valores booleanos e decisões com `if` e `else`.
- Projeto: estimador de consumo de energia e comparação de custo com um orçamento.

## Aula 2 — Aprendendo Python com jogos

Aula de **duas horas** que retoma os fundamentos da primeira e os aplica em seis jogos. Cada conceito novo é apresentado quando o jogo precisa dele. Apenas Python básico e o módulo `random` são usados.

- Revisão: entrada, conversão, comparação e repetição.
- Jogo de adivinhação: `random.randint`, `for`, `range`, `elif` e `break`.
- Duelo de dados: sorteio, comparação e empate.
- Par ou ímpar: soma e resto da divisão com `%`.
- Pedra, papel e tesoura: vários `elif` e condições combinadas com `and`.
- Aventura de decisões: textos e condições aninhadas.
- Quiz de multiplicação: sorteio, repetição e contador de pontos.

A aula prioriza o raciocínio antes do código. Em cada jogo, depois das regras, um slide **Pense antes de programar** traz perguntas para responder em português; as respostas aparecem uma a uma quando a apresentação avança. Só então os conceitos e a implementação em Python são apresentados.

No notebook, a adivinhação é resolvida em etapas. Cada jogo traz regras, um exemplo de partida, as mesmas perguntas para pensar e uma célula para a solução. As respostas, os passos para programar e a solução ficam em blocos expansíveis.

## Abrir a apresentação

Com Python 3 instalado, execute na pasta do repositório:

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

Abra [http://localhost:8000](http://localhost:8000) no navegador. A página inicial direciona para a [aula 1](http://localhost:8000/aula_01/) e para a [aula 2](http://localhost:8000/aula_02/). Use as setas para navegar; nos exemplos de código, cada avanço destaca o próximo trecho ou revela a saída. Para encerrar o servidor, pressione **Ctrl+C** no terminal.

Os slides carregam o Reveal.js e seu plugin de destaque de código pela CDN, portanto precisam de conexão com a internet. A página é estática e não exige uma etapa de build.

## Executar o notebook

Use Python 3 e o Jupyter Notebook. Se ainda não tiver o Jupyter, consulte as [instruções oficiais de instalação](https://jupyter.org/install).

Na pasta do repositório, execute:

```bash
jupyter notebook aula_01/aula_01_energia_python.ipynb
jupyter notebook aula_02/aula_02_jogos_python.ipynb
```

Use o primeiro comando para a aula 1 e o segundo para a aula 2.

No navegador, execute as células de cima para baixo com **Shift + Enter**. As variáveis ficam disponíveis durante a sessão, por isso a ordem de execução importa. Os exemplos usam recursos básicos de Python, sem bibliotecas adicionais. Na aula 2, os jogos usam sorteios, então os resultados mudam a cada execução.

### Exemplo do projeto

Para um aparelho de **100 W**, utilizado **5 horas por dia** durante **30 dias**, com tarifa de **R$ 0,80/kWh**:

- Consumo estimado: **15 kWh**.
- Custo estimado: **R$ 12,00**.
- Com orçamento de **R$ 10,00**, o custo fica acima do limite.

Experimente alterar o orçamento para **R$ 15,00** e observe a nova mensagem. Nas entradas de Python, use ponto decimal, como `0.80`.

## Publicar no GitHub Pages

1. Envie `index.html` e as pastas `assets/`, `aula_01/` e `aula_02/` para o repositório no GitHub, mantendo a estrutura abaixo.
2. Acesse **Settings → Pages**.
3. Em **Build and deployment → Source**, selecione **Deploy from a branch**.
4. Selecione a branch que contém os arquivos (`main` ou `master`) e a pasta **/ (root)**.
5. Clique em **Save** e aguarde a publicação. O endereço aparecerá nessa mesma página.

No GitHub Free, use um repositório público. Novos commits na branch selecionada atualizam o site. Veja a [documentação do GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

O endereço do site abre a página inicial, que leva às aulas em `aula_01/` e `aula_02/`. Cada apresentação oferece seu notebook para download no último slide. A execução do notebook acontece em um ambiente Jupyter.

## Arquivos

```text
.
├── index.html                              # Página inicial com links para as aulas
├── assets/
│   └── python-logo.svg                     # Logotipo oficial do Python
├── aula_01/
│   ├── index.html                          # Apresentação da aula 1
│   └── aula_01_energia_python.ipynb        # Exemplos, exercícios e projeto guiado
├── aula_02/
│   ├── index.html                          # Apresentação da aula 2
│   └── aula_02_jogos_python.ipynb          # Jogos guiados e atividades
└── README.md
```

## Referências

- Edsger W. Dijkstra — [Notes on Structured Programming, EWD 249 (1969)](https://www.cs.utexas.edu/~EWD/transcriptions/EWD02xx/EWD249/EWD249.html).
- Python Software Foundation — [O que é Python?](https://www.python.org/doc/essays/blurb/) e [logotipo oficial](https://www.python.org/community/logos/).
- [Project Jupyter](https://jupyter.org/).
- [Reveal.js — apresentação de código](https://revealjs.com/code/).
