# Atividade-ponderada-2_Arquitetura-em-Esboso-do-MVC-em-Sails

- Nome do Projeto: Projeto Sistema Web (nome ainda a definir);
- Descrição: 
A plataforma proposta tem o intuito de apoiar os jogadores do Business Game da CESIM, promovendo uma melhor interação entre eles. Nosso objetivo é facilitar a compreensão mútua, especialmente entre membros de diferentes culturas, visando resolver a falta de entendimento evidenciada no início do jogo. Para isso, vamos desenvolver uma plataforma com funcionalidades como organização de tarefas, comunicação, relatórios semanais e perfis dos membros. Além disso, implementaremos um sistema de autoavaliação e avaliação entre os membros, visando promover a consciência individual e a compreensão mútua dentro dos grupos;
- Arquitetura: MVC (Model-View-Controller);
- Ferramenta de Diagramação: draw.io.

### Modelos (Models):
- Indivíduos: Model no qual serão armazenadas informações pessoais relacionadas aos indivíduos que utilizarão a aplicação web. Atributos: Nome, Tags, Mensagens, Notas.
- Tempo: model no qual será armazenado um parâtro que armazena o tempo, para saber qual é o momento da simulação que os jogadores estarão, isso será relevante principalmente para criar a periodicidade das avaliações. Atributo: Período de Tempo;
- Avaliações: Armazenará os dados essenciais para o funcionamento das avaliações. Atributos: Opções de Escolha, Combinações de Escolha;
- Cadastros: Irá armazenar os cadastros de cada usuário da aplicação, tais cadastros estarão armazenados no site e serão fornecidos pela Zuyd; Atributos: E-mail, Senha.

### Controladores (Controllers):
- Usuário: Esse controlador tem contato com partes do site que contém informações mais voltadas ao usuário e seus dados pessoais, assim como os busca em seus respectivos models.
Ações: Buscar/Selecionar, Adicionar, Ordenar;
- Sistema: Esse controlador tem acesso mais as views que estão relacionadas a 'features' que vem com o sistema, que estão no sistema e que apenas serão selecionadas pelo usuário.
Ações: Buscar/Selecionar, Adicionar, Listar.

### Views (Views):
- Reportes do Time: Aba na qual o usuário poderá comunicar ao time informação relevante para a semana, sobre possíveis necessidade de mudanças de horários, compromissose avisos importantes.
- Ver avaliações: Aba na qual o usuário conseguirá visualizar sua autoavaliação e a média das avaliações que seu grupo fez sobre ele;
- Bio Pessoal/Grupo: As bios são páginas (perfis) onde aparecem algumas informações sobre os indivíduos, como: foto, características, tags;
- Grupo: Aba na qual serão mostrados os integrantes do grupo, e suas respectivas 'bios'.
- Fazer Avaliações: Página onde serão realizadas as avalições pessoal e grupal;
- Login: Aba na qual o usuário conseguirá se logar à plataforma para ter acesso ao seu perfil (login e senha serão fornecido pela Zuyd)

### Infraestrutura:

No projeto, empregamos tecnologias como NodeJS para a execução de servidor JavaScript, Sails como framework web MVC sobre Node.js, e HTML, CSS e JavaScript para o frontend. Além disso, utilizamos DBeaver como ferramenta de gerenciamento de banco de dados universal e PostgreSQL como sistema avançado e open-source de gerenciamento de banco de dados relacional.


### Justifique as escolhas feitas e como elas impactam o projeto.
#### Implicações da Arquitetura:
As tecnologias escolhidas para realizar esse projeto foram pensadas estrategicamente para que o projeto seja escalável e possa expandir futuramente, tenha a possibilidades de que manutenções regulares sejam realizadas, tenha fácil acesso a realização de testes e todos as outras características típicas de uma aplicação Web. 


