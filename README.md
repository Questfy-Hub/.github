# 🖥️ QUESTFY HUB

A plataforma _**QuestfyHub**_ consiste em um gerenciador de tarefas com elementos de gamificação para utilização empresarial. O sistema é ideal para instituições que buscam formas inovadoras e personalizáveis de beneficiar os colaboradores, permitindo a compra de diferentes recompensas com pontos adquiridos na conclusão de atividades escolhidas pela própria empresa. 

O projeto foi criado como requisito obrigatório da UC "Estrutura de Dados e Análise de Algoritmos", parte da grade do curso de Ciência da computação na UNA. Inicialmente, o software não foi desenvolvido com propósitos comerciais.
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
> - Usuário: wwonka@gmail.com | Senha: 1234


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
            <li>Baixe o banco modelo em <a href="#links">Links Uteis</a>;</li>
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
                Preencha as informações necessárias (sinalizadas nos colchetes);
                <img src="https://github.com/Questfy-Hub/General_Informations/assets/146457912/03a73727-a598-4b8a-8ae3-fc9bc8478d4b">
            </li>
        </ol>
    </p>
</details>

Assim que todas as configurações estiverem feitas, abra e execute a classe _**AppApplication**_, depois entre no site do projeto.

## :globe_with_meridians: Sobre o Projeto

Conforme informado anteriormente, a ideia primordial deste projeto é o desenvolvimento de um site para a organização e gerenciamento de tarefas empresariais que adotam metodologias ágeis. As principais funcionalidades presentes dentro do projeto são:
- Criação e distribuição das tarefas
- Distribuição de pontos por tarefas
- Loja de Pontos
- Visualização de relatorios mensais por funcionario (Gestor)
  

 Todo o desenvolvimento do site foi trabalhado na linguagem `Java`, utilizando o algoritmo de ordenação `Quick Sort` para o rankeamento de usuários. Foi implementado o banco de dados `PostGreSQL` para a conexão dos bancos de dados com o site. A parte visual foi desenvolvida no `Figma`. 


- FRONT END: `ANGULAR`
- BACK END: `JAVA`, `SPRING BOOT`, `JPA`
- BANCO DE DADOS: `POSTGRESQL`
- DESIGN: `FIGMA`

## Levantamento de Requisitos

### Requisitos Funcionais
**Requisitos do Administrador**

| Prioridade | Requisito |
| :------ | ----------- |
| Alta | Registrar, visualizar, editar, e apagar a organização |
| Alta | Criar, visualizar, editar, apagar, adicionar informações, atribuir usuário e aprovar tarefas |
| Alta | Criar, visualizar, editar, e apagar usuário |
| Alta | Criar, visualizar, editar, e apagar produtos da loja de ponto |
| Média | Gerar relatórios de produtividade da equipe | 


**Requisitos do Funcionário**
| Prioridade | Requisito |
| :------ | ----------- |
| Alta | Visualizar, editar, adicionar informações, receber pontos na conclusão e enviar para aprovação as tarefas |
| Alta | Efetuar a compra dos produtos  |
| Média | Visualizar e editar informações da sua conta | 

### Requisitos não Funcionais

| Prioridade | Requisito |
| :------ | ----------- |
| Alta | Autenticação de Usuário |
| Alta | Privacidade dos dados armazenados |
| Média |  Criptografia de dados |
| Média | Bom funcionamento no maior número de dispositivos |
| Média | Interface simples e intuitiva |
| Média | Alta disponibilidade |
| Média | Baixo tempo de resposta |
## BANCO DE DADOS (DIAGRAMA):

![Diagrama1](https://github.com/Questfy-Hub/General_Informations/assets/146457912/2ba59dd9-06ab-41b9-9b2f-2cfd28f732a5)

> Para criar o diagrama do banco de dados foi utilizado a ferramenta SQL WorkBench


## ✏️ Colaboradores
<table>
  <tr>
    <td align="center">
      <a href="https://github.com/gabsevamac" title="defina o titulo do link">
        <img src="https://github.com/Questfy-Hub/General_Informations/assets/146457912/f77485f5-ec3c-41b4-a0b0-2bc03215a379" width="100px;" alt="Gabriel Evaristo"/><br>
        <sub>
          <b>Gabriel Evaristo</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/ViniciusMGodinho" title="defina o titulo do link">
        <img src="https://github.com/Questfy-Hub/General_Informations/assets/146457912/39ef40d6-6122-494e-8fdf-a6e6e4af0e33" width="100px;" alt="Vinicius Madureira"/><br>
        <sub>
          <b>Vinicius Madureira</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/JoaoPaulo-66" title="defina o titulo do link">
        <img src="https://github.com/Questfy-Hub/General_Informations/assets/146457912/f7ed62f9-dc12-4c04-b3d6-c361b9cbfc03" width="100px;" alt="João Paulo"/><br>
        <sub>
          <b>João Paulo</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/IsraPrime16" title="defina o titulo do link">
        <img src="https://github.com/Questfy-Hub/General_Informations/assets/146457912/84ed49e7-6aa8-4a99-8f78-6c02df36c3c8" width="100px;" alt="Israel Silva"/><br>
        <sub>
          <b>Israel Silva</b>
        </sub>
      </a>
    </td>
  </tr>
</table>



## <a name="links"></a> Links Úteis

- [Codigo do Back-End](https://github.com/Questfy-Hub/Back-End)
- [Codigo do Front-End](https://github.com/Questfy-Hub/Front-End)
- [Diagrama do Banco de Dados](https://github.com/Questfy-Hub/General_Informations/blob/main/A3.mwb)
- [Modelo do Banco de Dados](https://github.com/Questfy-Hub/General_Informations/blob/main/QuestfyHub_DB.sql)
- [Slides da apresentação](ExpoUna_EDAA_QuestfyHub.pptx)

