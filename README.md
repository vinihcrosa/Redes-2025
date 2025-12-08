# Redes_2025

Pequeno guia para compilar o PDF do projeto LaTeX.

## Requisitos
- LaTeX com `latexmk`, `pdflatex` e `biber` instalados (TeX Live completo costuma ser o suficiente).

## Como compilar
No diretório do projeto:
```bash
latexmk -pdf main.tex
```
O `latexmk` chama o `biber` automaticamente para processar `refs.bib`. O PDF final é gerado em `main.pdf`.

## Limpeza de artefatos
Para remover arquivos temporários gerados na compilação:
```bash
latexmk -c
```
