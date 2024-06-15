# 🖥️ QUESTFY HUB: SISTEMA DE GERENCIAMENTO DE TAREFAS GAMEFICADO:

![Trabalho](https://github.com/Questfy-Hub/General_Informations/assets/132410269/f87fd2d4-74dd-4247-875e-77bc4347defb)



## INTRODUÇÃO:

A ideia primordial deste projeto é o desenvolvimento de um site para a organização e gerenciamento de tarefas empresariais. Seu conceito mais voltado para um Level Design Gameficado engloba toda a ideia do projeto, utilizando de Ranqueamento de usuário, Ranqueamento de pontos, Níveis de Dificuldade das Tarefas, para que o Usuário Final(os funcionários das empresas), tenham uma experiência completamente inovadora no seu ambiente profissional. O sistema do site funciona com o consumo de uma API, desenvolvida no Angular. Depois do cadastramento no Site, temos as divisões presentes nele: Distribuição das Tarefas para os usuários (Definido pelos Gestores), Nível de Dificuldade das Tarefas (Definido também pelos Gestores), Distribuição de Pontos das Tarefas (Pontuação Pré-Estabelecida, mas suscetível a mudanças por parte das empresas), Loja de Pontos para os funcionários consumirem seus pontos adquiridos pelas tarefas concluídas. Todo o desenvolvimento do site foi trabalhado na linguagem `Java`, com a implementação de `PostGreSQL` para a conexão dos bancos de dados com o site. A parte visual foi desenvolvida no `Figma`. Utilizamos o algoritmo de ordenação `Quick Sort` para o ranking(Ranqueamento), e também o método de recursividade para as tarefas.



## SITE DO PROJETO:

 - [Questfy Hub](https://questfyhub.netlify.app/login)


## 🛠️ ESTRUTURAS UTILIZADAS:

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

> Utilização de SQL para a criação desses Diagramas.






## CADASTRO:

![Cadastro](https://github.com/Questfy-Hub/General_Informations/assets/132410269/de40e406-ea7a-4af4-a7f1-b7e7e696ce87)

> As informações de cadastro ficam armazenadas no banco de dados criado através do SQL, especificamente na Tabela **User**, e a opção de colocar a foto foi uma peculiaridade que utilizamos para deixar nosso site o mais profissional possível.

## TAREFAS: 

![Tarefas](https://github.com/Questfy-Hub/General_Informations/assets/132410269/a485749a-7cea-4e4f-8ad2-bcd9c6f6e674)

> Quando as tarefas forem geradas para os funcionários, elas possuirão uma data limite para serem executadas, sendo de 1 hora de execução, a 2 meses, para serem concluídas,
dependendo do nível de dificuldade que for imposta para aquela tarefa.

> Outro detalhe são as colunas na qual as tarefas estão presentes, utilizando de uma interface interativa, funcionam como uma medida de progressão, e todas as vezes que ocorrer um avanço da tarefa, ela irá passar de um estado para o outro, não somente isso, como terá uma diminuição de pontos gradativa a medida que o tempo da tarefa se expirar, mas nunca chegará a 0, para que os funcionários sempre sejam incentivados a concluírem no tempo determinado.

> Por exemplo, uma tarefa de nível x, que demora cerca de 1 semana para ser finalizada, quando o prazo dela acabar, os pontos dela progressivamente diminuirão, equivalente a quantidade de dias que ela estava atribuída, até que chegue em 1 ponto, e não passará disso.

## RANQUEAMENTO:

![Ranqueamento](https://github.com/Questfy-Hub/General_Informations/assets/132410269/5a862cd5-c27f-47bd-9b18-2e67e633d7e0)

> Esta aba apresenta as informações do funcionário, similar aos "Status" do personagem de um jogo, contendo seus pontos, o ranking dos melhores funcionários a completar o maior número de tarefas, acessso a um item especial, na qual é necessário uma elevada pontuação para adquirí-la, e principalmente ficam as novas tarefas e as que ainda precisam ser finalizadas, para que o funcionário tenha um controle sobre o que ele necessariamente precisa priorizar em finalizar.

## LOJA DE PONTOS:


![Loja de Pontos](https://github.com/Questfy-Hub/General_Informations/assets/132410269/e0b02b44-f82a-435e-ba6a-6aef77120ceb)

> A Loja De Pontos foi pensada como uma bonificação para os usuários adquirirem recompensas por suas tarefas concluídas, podendo resgatar brindes variados, na qual fica a parte da empresa o que ela irá adicionar a loja.



## BACK END (DESENVOLVIMENTO DE FUNCIONALIDADES):

O Back End teve todo o desenvolvimento das Tasks, as ligações entre as tabelas, as funcionalidades presentes nelas . Além do desenvolvimento de um CRUD (Create, Read, Update, Delete) para puxar todas as informações
do [Diagrama](https://github.com/Questfy-Hub/General_Informations/assets/132410269/0f5f99ed-3c72-48de-adc6-fb63df01c830).
Logo depois, foi utilizado os métodos de Update `Put` and `Patch`, que são métodos de solicitação HTTP usados para atualizar recursos em um servidor.

# MÉTODO PUT:

- PROPÓSITO : O método `PUT` foi utilizado para fazer a atualização geral das Tasks, alterando seu status, pontuação, dificuldade.

# MÉTODO PATCH:

- PROPÓSITO : O método `PATCH` foi utlizado para alterações parciais nas Tasks, sendo mais para troca de status, por exemplo: De Pendente, para Aprovado.


# getTaskByUserId:

Depois temos a função `getTaskByUserId`, na qual é uma função comum em sistemas de gerenciamento de tarefas, especialmente em aplicações de software que seguem o paradigma do CRUD. O propósito geral dessa função neste projeto é buscar e retornar uma lista de tarefas associadas a um usuário específico, identificando-o pelo seu ID único.


# CRIPTOGRAFIA:

Utilizamos também  um sistema de criptografia para o embaralhamento das informações sensíveis do usuário. Essa criptografia consiste em uma prática essencial para proteger dados de usuários.
