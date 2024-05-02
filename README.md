# hi_nodejs

nvm install --lts                     Install the latest LTS version
nvm use --lts                         Use the latest LTS version

Depois de instalar o Node.js, abra o terminal ou prompt de comando e crie uma nova pasta para o seu projeto. Navegue até esta pasta usando o terminal e execute o seguinte comando para iniciar um novo projeto Node.js:

npm init -y

Este comando criará um arquivo package.json na sua pasta, que contém informações sobre o seu projeto e suas dependências.

Instalar Dependências
Agora você pode instalar as dependências necessárias para o seu projeto. Por exemplo, se você quiser criar um servidor web simples, você pode instalar o Express, um framework web para Node.js. Execute o seguinte comando no terminal para instalar o Express:

npm install express

Dentro da sua pasta do projeto, crie um arquivo JavaScript que conterá o código do seu servidor. Por exemplo, você pode chamar este arquivo de server.js.


No arquivo server.js, você pode escrever o código para configurar e iniciar o seu servidor. Aqui está um exemplo básico usando o Express:




---

meu-projeto-backend/
  |- node_modules/      # Pasta onde as dependências do projeto são instaladas
  |- src/               # Pasta que contém o código-fonte do projeto
  |   |- controllers/   # Pasta para controladores, que lidam com a lógica de roteamento e manipulação de solicitações
  |   |- models/        # Pasta para modelos, que representam os dados do aplicativo
  |   |- routes/        # Pasta para rotas, que definem os endpoints da API e vinculam solicitações HTTP a controladores
  |   |- app.js         # Arquivo principal do aplicativo, onde o servidor Express é configurado e inicializado
  |- config/            # Pasta para arquivos de configuração, como configurações de banco de dados, variáveis de ambiente, etc.
  |- tests/             # Pasta para testes automatizados
  |- .gitignore         # Arquivo que especifica os arquivos e pastas a serem ignorados pelo git
  |- package.json       # Arquivo que contém metadados e dependências do projeto
  |- package-lock.json  # Arquivo gerado pelo npm para manter a árvore de dependências exata


conectar o projeto a um banco sqllite 

instalando o sqllite no computador
sudo apt install sqlite3

add dependencia ao projeto
npm install sqlite3


para ter algo como jpa exite ORMs para node e express
Sequelize: Sequelize é um ORM completo e maduro para Node.js que suporta vários bancos de dados relacionais, incluindo MySQL, PostgreSQL, SQLite e outros. Ele fornece uma API poderosa e flexível para trabalhar com bancos de dados, incluindo suporte a migrações, associações, validações e muito mais.
TypeORM: TypeORM é outro ORM popular para Node.js que oferece suporte a vários bancos de dados, incluindo MySQL, PostgreSQL, SQLite e outros. Ele permite definir modelos de dados usando classes TypeScript e fornece uma ampla gama de recursos, incluindo associações, validações, suporte a transações e muito mais.
Bookshelf.js: Bookshelf.js é um ORM leve e flexível para Node.js baseado no Knex.js. Ele foi projetado para funcionar bem com o Express e oferece suporte a vários bancos de dados, incluindo PostgreSQL, MySQL e SQLite. Ele permite definir modelos de dados usando classes JavaScript e oferece uma API simples e expressiva para trabalhar com bancos de dados.
Objection.js: Objection.js é outro ORM construído no topo do Knex.js que oferece uma API semelhante ao ActiveRecord do Ruby on Rails. Ele fornece suporte a associações, validações, consultas avançadas e muito mais.

vou utilizar o sequelize

npm install sequelize