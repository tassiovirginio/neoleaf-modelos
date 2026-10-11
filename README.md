# NeoLeaf: modelos

Modelos de LaTeX prontos para o catálogo do [NeoLeaf](https://neoleaf.science). Cada pasta é um modelo completo e
autossuficiente: arquivo principal, bibliografia, estilo bibliográfico, imagens de exemplo e a classe, na versão usada.
Foram compilados com pdfLaTeX (TeX Live 2026) antes de entrarem aqui.

O catálogo do NeoLeaf guarda só o link e a versão (tag) de cada modelo. Os arquivos vêm deste repositório.

## Modelos

| Pasta | Arquivo principal | Para que serve | Origem | Licença |
|---|---|---|---|---|
| `acm-sigconf` | `sigconf.tex` | Artigos de conferências da ACM (formato sigconf) | [acmart](https://github.com/borisveytsman/acmart), v2.21 | LPPL 1.3c |
| `acm-sigplan` | `sigplan.tex` | Conferências ACM SIGPLAN | acmart v2.21 | LPPL 1.3c |
| `acm-acmsmall` | `acmsmall.tex` | Periódicos ACM (formato acmsmall) | acmart v2.21 | LPPL 1.3c |
| `acm-acmtog` | `acmtog.tex` | Periódico ACM Transactions on Graphics | acmart v2.21 | LPPL 1.3c |

## Como os arquivos foram gerados

Os modelos da ACM vêm do repositório oficial `borisveytsman/acmart`, que guarda só os fontes (`.dtx` e `.ins`). Os arquivos
foram gerados com `latex acmart.ins` (a classe `acmart.cls` e o estilo `ACM-Reference-Format.bst`) e `latex samples.ins`
(os documentos de exemplo). Nenhum conteúdo foi alterado: os cabeçalhos de autoria e de licença continuam nos arquivos.

## Licenças

Cada modelo mantém a licença de quem o criou, indicada na tabela. O texto da LPPL 1.3c está em
`LICENSE-ACMART-LPPL.txt`. Este repositório só reúne e organiza os arquivos; os direitos continuam com os autores.
Se você é autor de um modelo e quer que ele saia daqui, abra uma issue.

## Versões

Use sempre uma tag (por exemplo `v1`) para o modelo não mudar sem aviso. O catálogo do NeoLeaf fixa a tag no cadastro.
