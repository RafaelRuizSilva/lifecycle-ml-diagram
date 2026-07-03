# Ciclo de Vida de ML na AWS — Diagrama Interativo

Aula interativa sobre o ciclo de vida de um modelo de machine learning, baseada no diagrama de arquitetura oficial do [AWS Well-Architected — Machine Learning Lens](https://docs.aws.amazon.com/pt_br/wellarchitected/latest/machine-learning-lens/architecture-diagram.html).

O diagrama da AWS foi recriado como uma interface clicável: cada componente (fases, Feature Stores, Model Registry, Lineage Tracker, loops de feedback) abre um painel explicando o que acontece naquela etapa, como ela se conecta às demais e quais serviços AWS a implementam.

## Funcionalidades

- **Diagrama fiel ao original da AWS** — banner de fases em chevrons, caixas coloridas, cilindros das stores, setas tracejadas com rótulos e loops de feedback.
- **15 componentes clicáveis** — ao selecionar um, as conexões dele ficam destacadas e o restante do diagrama esmaece.
- **Painel lateral de detalhes** — "o que acontece aqui", conexões no diagrama e serviços AWS com ícones no estilo das categorias oficiais.
- **Modo aula** — botão que percorre as 15 etapas na ordem lógica do ciclo (navegável também pelas setas ← → do teclado).
- **Quiz** — 8 perguntas com feedback imediato ao final da página.

## Como executar

É um único arquivo estático, sem dependências nem build:

```
# basta abrir no navegador
index.html
```

Ou sirva localmente:

```
python -m http.server 8000
# http://localhost:8000
```

## Publicar no GitHub Pages

Em **Settings → Pages** do repositório, selecione a branch `main` e a pasta `/ (root)`. A página ficará disponível em `https://<seu-usuario>.github.io/<nome-do-repo>/`.

## Estrutura

| Arquivo | Descrição |
|---|---|
| `index.html` | Toda a aplicação: HTML, CSS e JavaScript em um único arquivo autocontido |

## Créditos

- Conteúdo baseado no [AWS Well-Architected Machine Learning Lens](https://docs.aws.amazon.com/wellarchitected/latest/machine-learning-lens/machine-learning-lens.html).
- Ícones inspirados no estilo dos [AWS Architecture Icons](https://aws.amazon.com/architecture/icons/) (recriados em SVG, não são os oficiais).
