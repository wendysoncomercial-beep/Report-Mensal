# Dashboard Customer

Dashboard web em **HTML, CSS e JavaScript** para acompanhamento semanal de indicadores de Customer Experience e performance por produto.

## Visão geral

Este projeto consome dados diretamente de planilhas do **Google Sheets** e monta um dashboard com:

- visão geral da carteira de clientes;
- indicadores de entrada e recorrência;
- contact rate;
- funil semanal por produto;
- evolução semanal de clientes entrantes;
- indicadores de experiência como **CSAT**, **Reclame Aqui**, **Play Store** e **BACEN**;
- análise de dores por produto.

## Funcionalidades

- filtros por **ano** e **mês**;
- abas separadas para **FGTS**, **INSS**, **PRIVADO** e **Experiência**;
- leitura automática da **última atualização**;
- gráficos com **Chart.js**;
- layout responsivo e leve;
- consumo de dados sem backend.

## Estrutura do projeto

```bash
.
├── index.html
└── README.md
```

## Fonte de dados

O dashboard lê os dados destas planilhas:

- **Dashboard principal**: `1Qk4LzvKDr8q1VYxhB5Gx4tKd3QtaFL7Qp9A_GliiAKE`
- **Última atualização**: `1aTaua3I0MHJrvObrhVXfJV7MsLcp-ai6NItKSQ6b25M`

Abas utilizadas:

- `visao_mes_produto`
- `visao_semanal_produto`
- `evolucao_experiencia`
- `experiencia_resumo`
- `dores_produto`
- `ultima_atualizacao`

## Como usar

### 1. Clonar ou baixar o projeto

```bash
git clone <URL_DO_SEU_REPOSITORIO>
cd dashboard-customer
```

### 2. Abrir localmente

Basta abrir o arquivo `index.html` no navegador.

### 3. Publicar no GitHub Pages

Se quiser deixar online pelo GitHub Pages:

1. suba os arquivos para o repositório;
2. vá em **Settings**;
3. abra a seção **Pages**;
4. em **Source**, selecione a branch principal;
5. salve e aguarde a publicação.

## Observações importantes

- As planilhas precisam estar com acesso compatível para leitura no navegador.
- Como os dados são carregados diretamente do Google Sheets, qualquer alteração na estrutura das abas pode impactar o funcionamento.
- Os IDs das planilhas estão definidos diretamente no arquivo `index.html`.

## Pontos de personalização

Você pode ajustar facilmente:

- cores do layout no bloco `:root` do CSS;
- nomes das abas no objeto `SHEETS`;
- lógica de filtros por ano e mês;
- títulos e cards do dashboard;
- gráficos renderizados com Chart.js.

## Melhorias futuras sugeridas

- separar o CSS e o JavaScript em arquivos próprios (`style.css` e `script.js`);
- adicionar tratamento visual para erro de carregamento das planilhas;
- incluir loading state durante a busca dos dados;
- criar versão com backend para maior controle de segurança e performance.

## Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript (Vanilla JS)
- Chart.js
- Google Sheets GViz API

## Autor

Projeto estruturado para publicação no GitHub com foco em visualização de indicadores de Customer.
