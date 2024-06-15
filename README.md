# 🖥️ QUESTFY HUB

A plataforma _**QuestfyHub**_ consiste em um gerenciador de tarefas com elementos de gamificação para utilização empresarial. O projeto foi criado como um projeto semestral da UC "Estrutura de Dados e Análise de Algoritmos".

## :rocket: Pré-requisitos
Antes de começar, certifique-se de que todos os pré-requisitos abaixo sejam atendidos, para que seja possivel a utilização local do projeto:
- Java 17
- Banco de dados local **PostgreSQL**
- _(Opcional)_ Angular 17

> Observação: O terceiro requisito se tornou opcional pois agora o Front-End do projeto está sendo hospedado na plataforma Netlify.
>
> Link de acesso para o projeto: [QuestfyHub](https://questfyhub.netlify.app)
>
> Para visualização utilize o login de teste:
> - wwonka@gmail.com | 1234


## :wrench: Utilização
Após realizada a cópia do repositório, algumas coisas devem ser feitas antes. Como o projeto foi inicialmente desenvolvido para rodar em ambiente local, algumas configurações devem ser feitas antes de rodar o programa:
<details>
    <summary>Postgresql</summary><!--TODO: Colocar imagens-->
    <p>
        <ol>
            <li>
                <p>Crie um novo banco de dados dentro do postgresql;</p>
                <img src="https://github.com/Questfy-Hub/General_Informations/assets/146457912/7d812f68-5571-48b0-989e-636a09814b8d">
            </li>
            <br>
            <li>Baixe o banco modelo em <a>Links Uteis</a>;</li>
            <br>
            <li>
                <p>Importe o banco modelo para seu banco de dados.</p>
                <img src="https://github.com/Questfy-Hub/General_Informations/assets/146457912/562c45b2-d519-4cf8-8cbd-4ce5daf04272">
                <img src="https://github.com/Questfy-Hub/General_Informations/assets/146457912/e003b94a-c4ff-4a05-8ee6-9dd667cd4da9">
            </li>
        </ol>
    </p>
</details>

<details>
    <summary>Back-End</summary>
    <p>
        <ol>
            <li>Vá ao arquivo application.proprieties;</li>
            <br>
            <li>
                Altere as informações dentro de [ ];
                <img src="https://github.com/Questfy-Hub/General_Informations/assets/146457912/03a73727-a598-4b8a-8ae3-fc9bc8478d4b">
            </li>
        </ol>
    </p>
</details>

## :globe_with_meridians: Sobre o Projeto

Conforme informado anteriormente, a ideia primordial deste projeto é o desenvolvimento de um site para a organização e gerenciamento de tarefas empresariais que adotam metodologias ágeis. As principais funcionalidades presentes dentro do projeto são:
- Criação e distribuição das tarefas
- Distribuição de pontos por tarefas
- Loja de Pontos
- Visualização de relatorios mensais por funcionario (Gestor)
  

 Todo o desenvolvimento do site foi trabalhado na linguagem `Java`, utilizando o algoritmo de ordenação `Quick Sort` para o rankeamendo de usuários. Foi implementado o banco de dados `PostGreSQL` para a conexão dos bancos de dados com o site. A parte visual foi desenvolvida no `Figma`. 


- FRONT END: `ANGULAR`
- BACK END: `JAVA`, `SPRING BOOT`, `JPA`
- BANCO DE DADOS: `POSTGRESQL`
- DESIGN: `FIGMA`

## Levantamento de Requisitos
| Requisitos Funcionais      | Requisitos não Funcionais          |
|:-------------------------- |----------------------------------: |
| Gerenciamento de Tarefas   | Criptografia de dados              |
| Visualização Kanban        | Autenticação de Usuário            |
| Cadastro de Usuário        | Interface intuitiva e Interativa   |
| Loja de Pontos             |                                    |



## BANCO DE DADOS (DIAGRAMA):

![Diagrama1](https://github.com/Questfy-Hub/General_Informations/assets/146457912/2ba59dd9-06ab-41b9-9b2f-2cfd28f732a5)

> Para criar o diagrama do banco de dados foi utilizado a ferramenta SQL WorkBench


## ✏️ Colaboradores
- Gabriel Evaristo
- Vinicius Madureira
- João Paulo
- Israel Fonseca




