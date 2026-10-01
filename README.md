# Primeiros passos em Python

Material introdutório de Python com slides em Reveal.js e notebook Jupyter, aplicado ao cálculo de consumo e custo de energia.

**Autor:** Waldsson Sacramento dos Santos.

## Proposta da aula

O material foi preparado para quem está começando a programar. A apresentação explica os conceitos antes de demonstrá-los em código, com saídas de terminal e um diagrama de decisão. O notebook complementa a aula com exemplos executáveis, exercícios e um projeto guiado.

A sequência sugerida é apresentar os fundamentos nos slides e, em seguida, executar os exemplos no notebook. Os exercícios também podem ser usados para estudo posterior.

## Conteúdo

- Introdução à programação, ao Python e ao Jupyter Notebook.
- Saída de informações com `print()`.
- Variáveis, atribuição e tipos de dados.
- Operadores aritméticos.
- F-strings e formatação decimal.
- Entrada de dados e conversão de tipos.
- Comparações, valores booleanos e decisões com `if` e `else`.
- Projeto: estimador de consumo de energia e comparação de custo com um orçamento.

## Abrir a apresentação

Com Python 3 instalado, execute na pasta do repositório:

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

Abra [http://localhost:8000](http://localhost:8000) no navegador. Use as setas para navegar; nos exemplos de código, cada avanço destaca o próximo trecho ou revela a saída. Para encerrar o servidor, pressione **Ctrl+C** no terminal.

Os slides carregam o Reveal.js e seu plugin de destaque de código pela CDN, portanto precisam de conexão com a internet. A página é estática e não exige uma etapa de build.

## Executar o notebook

Use Python 3 e o Jupyter Notebook. Se ainda não tiver o Jupyter, consulte as [instruções oficiais de instalação](https://jupyter.org/install).

Na pasta do repositório, execute:

```bash
jupyter notebook aula_python_engenharia_eletrica.ipynb
```

No navegador, execute as células de cima para baixo com **Shift + Enter**. As variáveis ficam disponíveis durante a sessão, por isso a ordem de execução importa. Os exemplos usam recursos básicos de Python, sem bibliotecas adicionais de cálculo.

### Exemplo do projeto

Para um aparelho de **100 W**, utilizado **5 horas por dia** durante **30 dias**, com tarifa de **R$ 0,80/kWh**:

- Consumo estimado: **15 kWh**.
- Custo estimado: **R$ 12,00**.
- Com orçamento de **R$ 10,00**, o custo fica acima do limite.

Experimente alterar o orçamento para **R$ 15,00** e observe a nova mensagem. Nas entradas de Python, use ponto decimal, como `0.80`.

## Publicar no GitHub Pages

1. Envie `index.html`, a pasta `assets/` e o notebook para o repositório no GitHub, mantendo a estrutura abaixo.
2. Acesse **Settings → Pages**.
3. Em **Build and deployment → Source**, selecione **Deploy from a branch**.
4. Selecione a branch que contém os arquivos (`main` ou `master`) e a pasta **/ (root)**.
5. Clique em **Save** e aguarde a publicação. O endereço aparecerá nessa mesma página.

No GitHub Free, use um repositório público. Novos commits na branch selecionada atualizam o site. Veja a [documentação do GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

O site apresenta os slides e oferece o notebook para download. A execução do notebook acontece em um ambiente Jupyter.

## Arquivos

```text
.
├── index.html                              # Apresentação Reveal.js
├── assets/
│   └── python-logo.svg                     # Logotipo oficial do Python
├── aula_python_engenharia_eletrica.ipynb    # Exemplos e exercícios
└── README.md
```

## Referências

- Edsger W. Dijkstra — [Notes on Structured Programming, EWD 249 (1969)](https://www.cs.utexas.edu/~EWD/transcriptions/EWD02xx/EWD249/EWD249.html).
- Python Software Foundation — [O que é Python?](https://www.python.org/doc/essays/blurb/) e [logotipo oficial](https://www.python.org/community/logos/).
- [Project Jupyter](https://jupyter.org/).
- [Reveal.js — apresentação de código](https://revealjs.com/code/).
