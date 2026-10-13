# NeoLeaf: modelos

Modelos de LaTeX prontos para o catálogo do [NeoLeaf](https://neoleaf.science). Cada pasta é um modelo completo e
autossuficiente: arquivo principal, bibliografia ou estilo bibliográfico, imagens de exemplo e a classe, na versão usada.
Todos foram compilados com pdfLaTeX (TeX Live 2026) numa cópia só com os arquivos da pasta antes de entrarem aqui.

O catálogo do NeoLeaf guarda só o link e a versão (tag) de cada modelo. Os arquivos vêm deste repositório.

## Modelos

| Pasta | Arquivo principal | Para que serve | Origem | Licença declarada |
|---|---|---|---|---|
| `acm-sigconf` | `sigconf.tex` | Conferências da ACM (sigconf) | [acmart](https://github.com/borisveytsman/acmart) v2.21 | LPPL 1.3c |
| `acm-sigplan` | `sigplan.tex` | Conferências ACM SIGPLAN | acmart v2.21 | LPPL 1.3c |
| `acm-acmsmall` | `acmsmall.tex` | Periódicos ACM (acmsmall) | acmart v2.21 | LPPL 1.3c |
| `acm-acmtog` | `acmtog.tex` | ACM Transactions on Graphics | acmart v2.21 | LPPL 1.3c |
| `ieee-conferencia` | `bare_conf.tex` | Conferências IEEE | [IEEEtran](https://ctan.org/pkg/ieeetran) v1.8b (CTAN) | LPPL 1.3 |
| `ieee-periodico` | `bare_jrnl.tex` | Periódicos IEEE | IEEEtran v1.8b (CTAN) | LPPL 1.3 |
| `elsevier-numerico` | `elsarticle-template-num.tex` | Elsevier, citações numéricas | [elsarticle](https://ctan.org/pkg/elsarticle) v3.5 (CTAN) | LPPL 1.3 |
| `elsevier-autor-ano` | `elsarticle-template-harv.tex` | Elsevier, citações autor-ano | elsarticle v3.5 (CTAN) | LPPL 1.3 |
| `springer-lncs` | `main.tex` | Springer LNCS (modelo mínimo escrito para o NeoLeaf) | [llncs](https://ctan.org/pkg/llncs) v2.26 (CTAN) | CC BY 4.0, segundo o CTAN |

Arquivo de apoio que acompanha alguns modelos: `example-image-a.pdf` (pacote `mwe`, LPPL 1.3, em `elsevier-*`).
O `aliascnt.sty` deixou de ser incluído em `springer-lncs` (v3): a cópia do CTAN exigia um LaTeX mais novo que o do navegador;
o NeoLeaf instala a versão compatível sozinho.

## Como os arquivos foram obtidos

- **ACM:** o repositório oficial guarda só os fontes (`.dtx` e `.ins`). Os arquivos foram gerados com `latex acmart.ins` e
  `latex samples.ins`, sem alterar o conteúdo.
- **IEEE e Elsevier:** copiados do pacote oficial no CTAN. Em `elsevier-*`, a classe `elsarticle.cls` foi gerada com
  `latex elsarticle.ins`.
- **Springer LNCS:** a classe `llncs.cls` e o estilo `splncs04.bst` vêm do CTAN. O `main.tex` e o `referencias.bib` são
  um exemplo mínimo escrito para o NeoLeaf, porque o pacote do CTAN não traz um documento de modelo.

**Alteração na v3:** nos modelos `elsevier-*` e `springer-lncs` foi acrescentada a linha `\usepackage{lmodern}` (marcada com
comentário), para os símbolos de texto (©, °) terem fonte vetorial na compilação no navegador. Nada mais foi alterado.

Os cabeçalhos de autoria e de licença originais continuam nos arquivos. O texto da LPPL 1.3c está em
`LICENSE-LPPL-1.3c.txt`.

## Licenças

Cada modelo mantém a licença de quem o criou, indicada na tabela. A coluna mostra a licença **declarada** pela origem
(nos arquivos ou no CTAN); este repositório não é uma análise jurídica. Ele só reúne e organiza os arquivos, e os direitos
continuam com os autores. Se você é autor de algum modelo e quer que ele saia daqui, abra uma issue.

## Versões

Use sempre uma tag (`v1`, `v2`...) para o modelo não mudar sem aviso. O catálogo do NeoLeaf fixa a tag no cadastro.
