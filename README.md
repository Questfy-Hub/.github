# PROJETO A3: SISTEMA DE GERENCIAMENTO DE TAREFAS GAMEFICADO:

**OBJETIVOS PRINCIPAIS**:

[X] REUNIÕES CONSTANTES PARA A SEPARAÇÃO E AVALIAÇÃO DE IDEIAS PARA O PROJETO;
 
[X] FINALIZAÇÃO DA AVALIAÇÃO, E INÍCIO DA DIVISÃO DE FUNÇÕES PARA OS MEMBROS DO GRUPO;

[X] INÍCIO DO PROJETO, MUITAS E MUITAS PESQUISAS REALIZADAS PARA A IDEIA COMEÇAR A SER TRABALHADA;

[X] REUNIÕES SEMANAIS PARA ANALISARMOS O DESENVOLVIMENTO DO SITE, E VERMOS ONDE PODÍAMOS MELHORAR, E ACRESCENTAR OU RETIRAR DETALHES;

[X] SITE FINALIZADO, TODOS OS INTEGRANTES TRABALHARAM ARDUAMENTE PARA DESENVOLVEREM ESSE SITE, PARA CONSEGUIR AJUDAR ÀS GRANDES E MICRO EMPRESAS;

[ ] APRESENTAÇÃO DO SITE...

## INÍCIO DO PROJETO:

A ideia primordial do nosso projeto é o desenvolvimento de um site para a organização e gerenciamento de tarefas empresariais.
Esse site não será limitado apenas para empresas de grande porte, pois micro empresas, empresas autônomas também se beneficiarão do nosso site.
O conceito de gameficar esse projeto partiu da afeição que o nosso grupo possui por jogos, principalmente jogos de RPG.
Ao longo do projeto, nós iremos especificar com mais detalhes como esse "jogo" irá funcionar.

## ESTRUTURAS UTILIZADAS:

- FRONT END: `ANGULAR`
- BACK END: `JAVA`, `SPRING BOOT`
- BANCO DE DADOS: `POSTGRESQL`
- DESIGN: `FIGMA`

## REQUISITOS FUNCIONAIS:

- CADASTRO DE USUÁRIO
- CADASTRO DA EMPRESA
- CADASTRO DE PRÊMIOS
- GERENCIAMENTO DE TAREFAS
- GERENCIAMENTO DE PREMIAÇÕES
- VISUALIZAÇÃO KANBAN
- VISUALIZAÇÃO EM CALENDÁRIO
- LOJA DE PONTOS

## REQUISITOS NÃO FUNCIONAIS:

- AUTENTIFICAÇÃO DE USUÁRIO
- CRIPTOGRAFIA DE DADOS
- DESIGN REATIVO
- INTERFACE INTUITIVA E INTERATIVA
- SISTEMA DE HIERARQUIA
- SISTEMA DE SQUADS

## DIAGRAMA UML

Nosso Site, como descrito anteriormente, a parte do desing foi feita no Figma, que é um editor gráfico de vetor e prototipagem, e projetos de design. Dito isso, aqui estão nossas tabelas desenvolvidas neste software:

## USER:

| ID: long | USERNAME: varchar(50) |
|----: |----------: |
|EMAIL: varchar(250) | FULLNAME: varchar(250) |
|CPF: varchar(250) | PASSWORD: varchar(250) |
|ID_COMPANY: longo |ROLE: varchar(250) |


## COMPANY:

| ID: long | CompanyName: varchar(50) |
|----: |-------------: |
|CNPJ: varchar(250) | CompanyCode: varchar(250) |

## TASKS:

| ID | TITTLE |
|----|--------|
|ShortDescription | LongDescription |
| EndLineDate | DIFFICULT |
| STATUS | ID_USER |

## GIFTS:

| ID | GiftName |
|----|----------|
| GiftPrice| CATEGORY |
| ID_COMPANY |


Em resumo, a tabela **User** são os dados necessários para o cadastro do usuário, a tabela **Company** são as empresas que desejam se cadastrar no Site, a tabela **Tasks** são as missões/tarefas que os funcionários executarão, e por fim a tabela **Gifts** na qual será a lojinha com presentes e recompensas para os funcionários que concluírem suas tarefas em um determinado período de tempo.

## INÍCIO DO DESENVOLVIMENTO FRONT END (PÁGINA INICIAL):

A página inicial do projeto, ou o famoso FRONT END, foi desenvolvido pelo nosso Líder Gabriel, na qual foi utilizado a plataforma `Angular`, que é um Framework de código aberto para criação de aplicativos dinâmicos e interativos na Web.
