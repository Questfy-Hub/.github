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
| ---- | ---------- |
|EMAIL: varchar(250) | FULLNAME: varchar(250) |
|CPF: varchar(250) | PASSWORD: varchar(250) |
|ID_COMPANY: long |ROLE: varchar(250) |


## COMPANY:

| ID: long | CompanyName: varchar(50) |
| ---- | ------------- |
|CNPJ: varchar(250) | CompanyCode: varchar(250) |

## TASKS:

| ID: long | TITTLE: varchar(50) |
|---- |-------- |
|ShortDescription: varchar(250) | LongDescription: varchar(250) |
| EndLineDate: varchar(250) | DIFFICULT: integer |
| STATUS: varchar(50) | ID_USER: long |

## GIFTS:

| ID: long | GiftName: varchar(50) |
| ---- | ---------- |
| GiftPrice: float | CATEGORY: varchar(250) |
| ID_COMPANY: long |


Em resumo, a tabela ***User*** são os dados necessários para o cadastro do usuário, a tabela ***Company*** são as empresas que desejam se cadastrar no Site, a tabela ***Tasks*** são as missões/tarefas que os funcionários executarão, e por fim a tabela ***Gifts*** na qual será a lojinha com presentes e recompensas para os funcionários que concluírem suas tarefas em um determinado período de tempo.

## INÍCIO DO DESENVOLVIMENTO FRONT END (PÁGINA INICIAL):

A página inicial do projeto, ou o famoso FRONT END, foi desenvolvido pelo nosso Líder Gabriel, na qual foi utilizado a plataforma `Angular`, que é um Framework de código aberto para criação de aplicativos dinâmicos e interativos na Web. E esta parte do Front End
será explicada de forma mais detalhada em outro Documento. **NÃO PRECISAM SE PREOCUPAR**, podem continuar com a programação normal.

## BACK END (CODAGEM E DESENVOLVIMENTO DE FUNCIONALIDADES):

O Back End ficou sob a responsabilidade do nosso integrante João, na qual todo o desenvolvimento das Tasks, as ligações entre as tabelas, as funcionalidades de cada tabela, ficaram por conta dele. Além do desenvolvimento de um CRUD, para puxar as informações
de todas as tabelas.
Depois foi feito os métodos de Update `Put` e `Patch`, que são métodos de solicitação HTTP usados para atualizar recursos em um servidor. Ambos são usados em APIs RESTful, mas têm diferenças importantes em como eles atualizam os dados.

# MÉTODO PUT:

. PROPÓSITO : O método `PUT` é usado para atualizar ou substituir um recurso completo no servidor.

. IDEMPOTÊNCIA : É idempotente, o que significa que fazer várias solicitações `PUT` com os mesmos dados resultará no mesmo estado do recurso no servidor.

. USO TÍPICO : É comum usar `PUT` quando você tem todos os detalhes do recurso e deseja substituir completamente o recurso existente.

. CORPO DA SOLICITAÇÃO : O corpo da solicitação geralmente contém a representação completa do recurso que deve ser atualizado ou criado.

# MÉTODO PATCH:

. PROPÓSITO : O método `PATCH` é usado para aplicar atualizações parciais a um recurso.

. IDEMPOTÊNCIA : Também é idempotente, mas com uma ressalva: a idempotência se aplica a atualizações que não causam efeitos colaterais diferentes a cada vez que são aplicadas.

. USO TÍPICO : É comum usar `PATCH` quando você deseja atualizar apenas alguns campos de um recurso, sem alterar todo o recurso.

. CORPO DA SOLICITAÇÃO : O corpo da solicitação contém apenas os dados que devem ser atualizados, não a representação completa do recurso.

# GETTASKBYUSERID

Depois nós temos a função `getTaskByUserId`, na qual é uma função comum em sistemas de gerenciamento de tarefas, especialmente em aplicações de software que seguem o paradigma do CRUD (Create, Read, Update, Delete). O propósito geral dessa função é buscar e retornar uma lista de tarefas associadas a um usuário específico, identificando-o pelo seu ID único. Em Java, a função `getTaskByUserId` é geralmente usada em um contexto onde você deseja recuperar uma ou mais tarefas associadas a um determinado usuário, identificando esse usuário por seu ID. A função normalmente faz parte de uma classe de serviço ou de um repositório que interage com um banco de dados ou uma estrutura de dados em memória.

Embora a implementação específica possa variar de acordo com a linguagem de programação e a arquitetura do sistema, o comportamento típico da função `getTaskByUserId` é:

. ENTRADA (Input):

userId: Um identificador único (ID) do usuário para o qual se deseja recuperar as tarefas. Esse ID é geralmente um número inteiro ou uma string.

. PROCESSO (Processing):

. A função consulta a base de dados ou outro repositório de dados onde as tarefas são armazenadas.

. Filtra as tarefas para retornar apenas aquelas que pertencem ao usuário cujo ID foi fornecido.

. SAÍDA (Output):

. Uma lista de tarefas associadas ao userId especificado. Cada tarefa na lista pode ser um objeto ou um dicionário contendo detalhes como o título da tarefa, descrição, data de criação, status, entre outros.

Nós também utilizamos um sistema de criptografia para o nosso projeto. Essa criptografia consiste em uma prática essencial para proteger dados de usuários. A criptografia garante que mesmo que um banco de dados seja comprometido, as senhas não possam ser facilmente lidas ou utilizadas. Em Java, a criptografia de senhas pode ser feita de forma segura usando algoritmos de hashing com salt.
