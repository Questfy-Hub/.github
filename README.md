# QUESTFY HUB: SISTEMA DE GERENCIAMENTO DE TAREFAS GAMEFICADO:

![Trabalho](https://github.com/Questfy-Hub/General_Informations/assets/132410269/f87fd2d4-74dd-4247-875e-77bc4347defb)



## INTRODUÇÃO:

A ideia primordial deste projeto é o desenvolvimento de um site para a organização e gerenciamento de tarefas empresariais. Seu conceito mais voltado para um Level Design Gameficado engloba toda a ideia do projeto, utilizando de Ranqueamento de usuário, Ranqueamento de pontos, Níveis de dificuldade das Tarefas, para que o usuário final(os funcionários das empresas), tenham uma experiência completamente inovadora no seu ambiente profissional. O sistema do site funciona com o consumo de uma API, desenvolvida no Angular, depois da entrada no Site, temos as divisões: A distribuição das Tarefas para os usuários (Definido pelos Gestores), Nível de dificuldade das Tarefas (Definido também pelos Gestores), Distribuição de Pontos das Tarefas (Pontuação Pré-Estabelecida, mas suscetível a mudanças por parte das empresas). Todo o desenvolvimento do site foi trabalhado na linguagem `Java`, com a implementação de `PostGreSQL` para a conexão dos bancos de dados com o site. A parte visual foi desenvolvida no `Figma`. Utilizamos algoritmos de ordenação (Quick Sort) para a 



## SITE DO PROJETO:

 - [Questfy Hub](https://questfyhub.netlify.app/login)


## ESTRUTURAS UTILIZADAS:

- FRONT END: `ANGULAR`
- BACK END: `JAVA`, `SPRING BOOT`
- BANCO DE DADOS: `POSTGRESQL`
- DESIGN: `FIGMA`


## DISTRIBUIÇÃO DOS REQUISITOS:


## REQUISITOS FUNCIONAIS:

![Requisitos Funcionais](https://github.com/Questfy-Hub/General_Informations/assets/132410269/573e87eb-816a-4de4-982f-9a3cff539a82)

## REQUISITOS NÃO FUNCIONAIS:

![Requisitos Não Funcionais](https://github.com/Questfy-Hub/General_Informations/assets/132410269/aa213d69-d34f-4f7d-991d-6eeb535fdede)

## BANCO DE DADOS (DIAGRAMA):

![Diagrama](https://github.com/Questfy-Hub/General_Informations/assets/132410269/0f5f99ed-3c72-48de-adc6-fb63df01c830)

- Utilização de SQL para a criação desses Diagramas 






## CADASTRO:

![Cadastro](https://github.com/Questfy-Hub/General_Informations/assets/132410269/de40e406-ea7a-4af4-a7f1-b7e7e696ce87)

> As informações do usuário estão armazenadas 

## TAREFAS: 

![Tarefas](https://github.com/Questfy-Hub/General_Informations/assets/132410269/a485749a-7cea-4e4f-8ad2-bcd9c6f6e674)

- Quando as tarefas forem geradas para os funcionários, elas possuirão um tempo limite para serem executadas, sendo de 1 hora de execução, a praticamente 2 meses, para serem concluídas,
dependendo do nível de dificuldade que for imposta para aquela tarefa.

- Outro detalhe são as colunas na qual as tarefas estão presentes, onde elas funcionam como uma medida de progressão, e todas as vezes que ocorrer um avanço da tarefa, ela irá passar de um estado para o outro, não somente isso, como terá uma diminuição de pontos progressiva, a medida que o tempo da tarefa se expira, mas nunca chegará a 0, para que os funcionários sejam incentivados a concluírem no tempo determinado.

- Por exemplo, uma tarefa de nível x, que demora cerca de 1 semana para ser finalizada, quando o prazo dela acabar, os pontos dela progressivamente diminuirão, equivalente a quantidade de dias que ela estava atribuída, até que chegue em 1 ponto, e não passará disso.

## RANQUEAMENTO:

![Ranqueamento](https://github.com/Questfy-Hub/General_Informations/assets/132410269/5a862cd5-c27f-47bd-9b18-2e67e633d7e0)

- 

## LOJA DE PONTOS:


![Loja de Pontos](https://github.com/Questfy-Hub/General_Informations/assets/132410269/e0b02b44-f82a-435e-ba6a-6aef77120ceb)

- A Loja De Pontos foi pensada como uma bonificação para os usuários adquirirem recompensas por suas tarefas concluídas, podendo resgatar brindes variados, na qual fica a parte da empresa o que ela irá adicionar a loja.



## BACK END (CODAGEM E DESENVOLVIMENTO DE FUNCIONALIDADES):

O Back End teve todo o desenvolvimento das Tasks, as ligações entre as tabelas, as funcionalidades presentes nelas . Além do desenvolvimento de um CRUD (Create, Read, Update, Delete) para puxar as informações
de todas as tabelas.
Depois, foi utilizado os métodos de Update `Put` and `Patch`, que são métodos de solicitação HTTP usados para atualizar recursos em um servidor. Ambos são usados em APIs RESTful.

# MÉTODO PUT:

- PROPÓSITO : O método `PUT` é usado para atualizar ou substituir um recurso completo no servidor.

# MÉTODO PATCH:

- PROPÓSITO : O método `PATCH` é usado para aplicar atualizações parciais a um recurso.


# getTaskByUserId:

Depois temos a função `getTaskByUserId`, na qual é uma função comum em sistemas de gerenciamento de tarefas, especialmente em aplicações de software que seguem o paradigma do CRUD. O propósito geral dessa função no nosso projeto é buscar e retornar uma lista de tarefas associadas a um usuário específico, identificando-o pelo seu ID único.


# CRIPTOGRAFIA:

Utilizamos também  um sistema de criptografia para o embaralhamento das informações sensíveis do usuário. Essa criptografia consiste em uma prática essencial para proteger dados de usuários.
