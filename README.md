# Trabalho-01---CSS-Grid-Layout

Projeto prático de um site responsivo aplicando conceitos avançados de CSS Grid Layout, integrado ao contexto de um **Sistema de Gestão de Eventos de Queima (Flaring)**.

## 🏢 O Contexto (Problema e Solução)
Desenvolvido para o cenário da **Petrobras** (Escola SENAI Santos Dumont), o sistema visa substituir processos manuais e planilhas descentralizadas no registro de queima de gás natural em plataformas offshore. 
O objetivo é garantir a conformidade ambiental (ESG) perante órgãos como IBAMA e ANP, evitando multas milionárias através de auditoria inteligente, padronização de entradas e respeito à hierarquia de aprovação de dados.

## 🛠️ Requisitos Técnicos Obrigatórios (CSS Grid)

1. **Estrutura Semântica:** Uso rigoroso das tags HTML5 (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, e `<footer>`).
2. **Layout Principal:** Gerenciado inteiramente via `grid-template-areas`.
3. **Responsividade:** O site deve se adaptar sem "quebras", utilizando no mínimo 3 breakpoints (Mobile, Tablet e Desktop).
4. **Navegação (Nav):** O menu deve se transformar de uma lista vertical (mobile) para uma grade horizontal complexa (desktop).
5. **Destaque Premium (Span):** Pelo menos um card de serviço/funcionalidade (ex: "Auditoria e Inteligência ESG") deve ocupar 2 colunas ou 2 linhas (`grid-column/row: span 2`).
6. **Organização Densa:** Uso de `grid-auto-flow: dense` para organizar elementos de tamanhos variados sem deixar espaços vazios na seção de Diferenciais.

## 📂 Estrutura Atual
- `index.html`: Página inicial contendo o Dashboard/Apresentação do FlareControl ESG, já estruturada com todas as tags semânticas obrigatórias.


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