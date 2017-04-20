# RAI Framework

RAI é um framework baseado em flexbox para a criação de hotsites da Prefeitura Municipal de São João de Meriti.

### Conteúdo

RAI já vem com algumas ferramentas prontas para uso.

* [SASS] - Pré-processador CSS
* [Grunt] - Automatizador de tarefas
* [Jquery] - Biblioteca Javascript
* [WOW.js + Animate.css] - Biblioteca utilizada para animações
* [Odometer] - Biblioteca utilizada para criação de contadores animados
* [Parallax] - Biblioteca utilizada para efeito parallax

### Tasks List

####  - Grunt Development
 - Watch
 - SASS
 - CSSMin
 - Uglify
#### - Grunt Production
 - Copy
 - minifyHtml
 - Imagemin
 - Ftp-deploy

### Configuração

Existem três arquivos que devem ser configurados antes do desenvolvimento do hotsite.
`{
    package.json, Gruntfile.js, .ftppass
}`

 - No arquivo `package.json`, você irá configurar as informações básicas do projeto(Nome, descrição, etc).
 - No arquivo Gruntfile.js, você deverá modificar a task de `'ftp-deploy'` informando o caminho da pasta no servidor.
 - E, finalmente, no arquivo `.ftppass`, você deverá configurar o usuário e senha do servidor ftp.


### Instalação

RAI requer [Node.js](https://nodejs.org/) v4+ e [Grunt](https://gruntjs.com/) para funcionar.

Instale as dependências de produção e de desenvolvimento digitando o código abaixo dentro do diretório do projeto.

```sh
$ cd rai
$ npm install -d
```

Depois, basta iniciar a tarefa de desenvolvimento do grunt.

```sh
$ grunt development
```
Após desenvolver, rode a tarefa de produção do grunt.

```sh
$ grunt production
```
