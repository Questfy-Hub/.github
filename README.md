# QUESTFY HUB: SISTEMA DE GERENCIAMENTO DE TAREFAS GAMEFICADO:

![Trabalho](https://github.com/Questfy-Hub/General_Informations/assets/132410269/f87fd2d4-74dd-4247-875e-77bc4347defb)



## INTRODUÇÃO:

A ideia primordial do nosso projeto é o desenvolvimento de um site para a organização e gerenciamento de tarefas empresariais. Seu conceito mais voltado para um Level Design Gameficado engloba toda a ideia do projeto, utilizando de Ranqueamento de usuário, Ranqueamento de pontos, Níveis de dificuldade das Tarefas, para que o usuário final(os funcionários das empresas), tenham uma experiência completamente inovadora no seu ambiente profissional. O sistema do site funciona com: A distribuição das Tarefas para os usuários (Definido pelos Gestores), Nível de dificuldade das Tarefas (Definido também pelos Gestores), Distribuição de Pontos das Tarefas (Pontuação Pré-Estabelecida, mas suscetível a mudanças por parte das empresas). Todo o desenvolvimento do site foi trabalhado na linguagem `Java`, com a implementação de `PostGreSQL` para a conexão dos bancos de dados com o site. O visual do site foi criado no `Figma`


## ESTRUTURAS UTILIZADAS:

- FRONT END: `ANGULAR`
- BACK END: `JAVA`, `SPRING BOOT`
- BANCO DE DADOS: `POSTGRESQL`
- DESIGN: `FIGMA`


## DISTRIBUIÇÃO DOS REQUISITOS:


## REQUISITOS FUNCIONAIS:

![Requisitos Funcionais](https://github.com/Questfy-Hub/General_Informations/assets/132410269/573e87eb-816a-4de4-982f-9a3cff539a82)

## REQUISITOS NÃO FUNCIONAIS:

![Requisitos Não Funcionais](https://github.com/Questfy-Hub/General_Informations/assets/132410269/a96b7fe0-adc8-4651-a4fd-6fa5b89f2e6f)


## SITE DO PROJETO:

 - (https://questfyhub.netlify.app/login)





## INÍCIO DO DESENVOLVIMENTO FRONT END (PÁGINA INICIAL):

A página inicial do projeto, ou o famoso FRONT END, foi desenvolvido pelo nosso Líder Gabriel, na qual foi utilizado a plataforma `Angular`, que é um Framework de código aberto para criação de aplicativos dinâmicos e interativos na Web. E esta parte do Front End
será explicada de forma mais detalhada em outro Documento.

## BACK END (CODAGEM E DESENVOLVIMENTO DE FUNCIONALIDADES):

O Back End ficou sob a responsabilidade do nosso integrante João, na qual todo o desenvolvimento das Tasks, as ligações entre as tabelas, as funcionalidades de cada tabela, ficaram por conta dele. Além do desenvolvimento de um CRUD, para puxar as informações
de todas as tabelas.
Depois foi feito os métodos de Update `Put` e `Patch`, que são métodos de solicitação HTTP usados para atualizar recursos em um servidor. Ambos são usados em APIs RESTful, mas têm diferenças importantes em como eles atualizam os dados.

# MÉTODO PUT:

- PROPÓSITO : O método `PUT` é usado para atualizar ou substituir um recurso completo no servidor.

- IDEMPOTÊNCIA : É idempotente, o que significa que fazer várias solicitações `PUT` com os mesmos dados resultará no mesmo estado do recurso no servidor.

- USO TÍPICO : É comum usar `PUT` quando você tem todos os detalhes do recurso e deseja substituir completamente o recurso existente.

- CORPO DA SOLICITAÇÃO : O corpo da solicitação geralmente contém a representação completa do recurso que deve ser atualizado ou criado.

# MÉTODO PATCH:

- PROPÓSITO : O método `PATCH` é usado para aplicar atualizações parciais a um recurso.

- IDEMPOTÊNCIA : Também é idempotente, mas com uma ressalva: a idempotência se aplica a atualizações que não causam efeitos colaterais diferentes a cada vez que são aplicadas.

- USO TÍPICO : É comum usar `PATCH` quando você deseja atualizar apenas alguns campos de um recurso, sem alterar todo o recurso.

- CORPO DA SOLICITAÇÃO : O corpo da solicitação contém apenas os dados que devem ser atualizados, não a representação completa do recurso.

# getTaskByUserId:

Depois nós temos a função `getTaskByUserId`, na qual é uma função comum em sistemas de gerenciamento de tarefas, especialmente em aplicações de software que seguem o paradigma do CRUD (Create, Read, Update, Delete). O propósito geral dessa função é buscar e retornar uma lista de tarefas associadas a um usuário específico, identificando-o pelo seu ID único. Em Java, a função `getTaskByUserId` é geralmente usada em um contexto onde você deseja recuperar uma ou mais tarefas associadas a um determinado usuário, identificando esse usuário por seu ID. A função normalmente faz parte de uma classe de serviço ou de um repositório que interage com um banco de dados ou uma estrutura de dados em memória.

Embora a implementação específica possa variar de acordo com a linguagem de programação e a arquitetura do sistema, o comportamento típico da função `getTaskByUserId` é:

- ENTRADA (Input):

 - UserId: Um identificador único (ID) do usuário para o qual se deseja recuperar as tarefas. Esse ID é geralmente um número inteiro ou uma string.

- PROCESSO (Processing):

- A função consulta a base de dados ou outro repositório de dados onde as tarefas são armazenadas.

- Filtra as tarefas para retornar apenas aquelas que pertencem ao usuário cujo ID foi fornecido.


- SAÍDA (Output):

- Uma lista de tarefas associadas ao userId especificado. Cada tarefa na lista pode ser um objeto ou um dicionário contendo detalhes como o título da tarefa, descrição, data de criação, status, entre outros.

# CRIPTOGRAFIA:

Nós também utilizamos um sistema de criptografia para o nosso projeto. Essa criptografia consiste em uma prática essencial para proteger dados de usuários. A criptografia garante que mesmo que um banco de dados seja comprometido, as senhas não possam ser facilmente lidas ou utilizadas. Em Java, a criptografia de senhas pode ser feita de forma segura usando algoritmos de hashing com salt.
