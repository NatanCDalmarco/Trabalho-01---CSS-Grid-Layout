# Trabalho-01---CSS-Grid-Layout

Projeto prático de um site responsivo aplicando conceitos avançados de CSS Grid Layout, integrado ao contexto de um Sistema de Gestão de Eventos de Queima (Flaring).

 🏢 O Contexto (Problema e Solução)
Desenvolvido para o cenário da Petrobras (Escola SENAI Santos Dumont), o sistema visa substituir processos manuais e planilhas descentralizadas no registro de queima de gás natural em plataformas offshore. 
O objetivo é garantir a conformidade ambiental (ESG) perante órgãos como IBAMA e ANP, evitando multas milionárias através de auditoria inteligente, padronização de entradas e respeito à hierarquia de aprovação de dados.

 🛠️ Requisitos Técnicos Obrigatórios (CSS Grid)

1. Estrutura Semântica: Uso rigoroso das tags HTML5 (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, e `<footer>`).
2. Layout Principal: Gerenciado inteiramente via `grid-template-areas`.
3. Responsividade: O site deve se adaptar sem "quebras", utilizando no mínimo 3 breakpoints (Mobile, Tablet e Desktop).
4. Navegação (Nav): O menu deve se transformar de uma lista vertical (mobile) para uma grade horizontal complexa (desktop).
5. Destaque Premium (Span): Pelo menos um card de serviço/funcionalidade (ex: "Auditoria e Inteligência ESG") deve ocupar 2 colunas ou 2 linhas (`grid-column/row: span 2`).
6. Organização Densa: Uso de `grid-auto-flow: dense` para organizar elementos de tamanhos variados sem deixar espaços vazios na seção de Diferenciais.


/Trabalho-01---CSS-Grid-Layout
│
├── index.html                 # Página inicial (Apresentação, Contexto do problema e Soluções ESG)
├── registro.html              # Página interna (Ex: Formulário de Novo Registro de Queima ou Relatório)
├── README.md                  # Documentação do projeto
│
└── assets/                    # Pasta principal de recursos estáticos
    │
    ├── css/                   # Arquivos de estilo separados por responsabilidade
    │   ├── reset.css          # Zera margens, paddings e define box-sizing
    │   ├── globais.css        # Variáveis de cores, tipografia e estilos gerais
    │   ├── layout.css         # O coração do projeto: 'grid-template-areas' e Media Queries (Mobile/Tablet/Desktop)
    │   └── componentes.css    # Estilos específicos (ex: `.card-funcionalidade`, `.alerta-auditoria`, menu)
    │
    ├── img/                   # Imagens gerais do projeto
    │   ├── logo-flarecontrol.svg
    │   └── bg-plataforma-offshore.jpg
    │
    └── icons/                 # Ícones utilizados nos cards e botões
        ├── icon-dashboard.svg
        ├── icon-alerta.svg
        └── icon-relatorio.svg



        resposta quetionarios


        Com certeza. Abaixo, organizei o conteúdo de forma limpa, direta e estruturada, ideal para você copiar e colar em um bloco de notas (.txt) ou usar como guia de estudo rápido.

---

 1. O QUE É CSS GRID?
* Definição: É um sistema de layout "quadriculado" (grade) para a web.
* Diferença do Flexbox: O Flexbox trabalha em uma direção (ou linha ou coluna). O Grid trabalha nas duas direções ao mesmo tempo (linhas E colunas).
* Histórico: Surgiu para acabar com a bagunça de usar "floats" e tabelas para montar sites.

 2. POR QUE USAR?
* Menos código: Você monta um site inteiro com poucas linhas de CSS.
* Responsivo: É muito fácil fazer o site se ajustar de celular para PC.
* Organização: Você decide exatamente onde cada elemento (menu, banner, rodapé) vai ficar.

 3. ANATOMIA (CONCEITOS CHAVE)
* Grid Container: O elemento pai (a caixa que segura tudo).
* Grid Item: Os elementos filhos (o que vai dentro da caixa).
* Grid Line: As linhas que dividem a grade (como as linhas de um caderno).
* Grid Track: O espaço entre duas linhas (é a coluna ou a linha inteira).
* Grid Cell: Um único "quadradinho" da grade (como uma célula de Excel).
* Grid Area: Um conjunto de vários quadradinhos formando um bloco maior.
* Gap: O espaço (respiro) entre as colunas e linhas.

 4. COMANDOS ESSENCIAIS
* `display: grid;` -> Ativa a grade no elemento pai.
* `grid-template-columns` -> Define quantas colunas e qual o tamanho delas.
* `grid-template-rows` -> Define as linhas.
* `grid-template-areas` -> Dá nome aos espaços (ex: "topo", "conteudo", "rodape").
* `gap` -> Define a distância entre os itens.

 5. DIMENSIONAMENTO ESPERTO
* fr (Fração): Unidade que ocupa o espaço que sobra. `1fr 1fr` cria duas colunas iguais.
* minmax(min, max): Define um tamanho que nunca fica menor que o mínimo, nem maior que o máximo.
* repeat(auto-fit, ...): Comando mágico que faz o site se ajustar sozinho ao tamanho da tela sem precisar de código extra para celular.

 6. GRIDS ANINHADAS E SUBGRID
* Nested Grid: É colocar um grid dentro de outro grid.
* Subgrid: Faz o grid "filho" usar as mesmas linhas do grid "pai" para tudo ficar perfeitamente alinhado.

 7. ESTRATÉGIA RESPONSIVA
* Mobile-First: Comece desenhando o site para celular (geralmente tudo em 1 coluna).
* Media Queries: Use apenas para mudar o número de colunas quando a tela crescer (ex: de 1 coluna no celular para 3 colunas no PC).
