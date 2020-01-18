#Aula 1

1. - instalar node através de algum gerenciador de pacote ex: NVM
2. - instalar algum gerenciador de depêndencias do projeto ex: NPM, Yarn
3. - instalar vsCode como IDER de desenvolvimento
4. - instalar extensões: Dracula theme, material icons, rocketSeat snippets
5. - instalar fonte fira-code para um visual melhor no código
6. - setar no json settings do vsCode para habilitar o fira-code:
```sh
editor.fontFamily: "Fira Code",
editor.fontLigatures: true
```


#Aula 2

1. - adicionar o yarn ao projeto
```sh
yarn init -y
```
2. - adicionar express como dependência do projeto
3. - criar arquivo server.js
3. - testar se o express está funcionando no arquivo server
    1. instânciar o express
    2. setar a porta na função listen ex: **app.listen('3333');**
    3. setar requisição ex: **app.get('/', (req, res)=>{res.send('test')});**
    4. subir o servidor 'ouvindo' o arquivo server: **node server.js**
    5. abrir o browser e testar se a resposta **test** do servidor node aparecerá
4. - adicionar o nodemon como dependência de desenvolvimento: yarn nodemon -D
5. - adicionar script dev no yarn para inicializar o nodemon
6. - testar nodemon
7. - para acessar query params 
    1. adicionar na url de requisição ?param=valor
    2. o valor é capturada no **req.query.nomedaquery**
8. - para acessar routes params
    1. adicionar /:nomerouteparam ao final da url que está sendo 'ouvida'
    2. o valor é capturado no **req.params.nomedarouteparam**
9. - para retornar o próprio body da requisição : **req.body**
10. - para retornar tipo body formato em json, é necessário ativar o modulo do express json(): **app(express.json());**
11. criar pasta src e colocar o server.js dentro
12. separar as rotas em outro arquivo: routes.js
    1. requite express novamente
    2. instânciar o router
    3. usar as rotas com esse router
    4. exportar as rotas como modulo
13. - importar as rotas no arquivo server
14. - usar as rotas no app: **app.use(routes);**
15. - criar banco no mongo atlas
    1. criar um novo cluster
    2. criar novo usuário no database access
    3. liberar acesso do servidor a qualquer IP
    4. pegar a configuração de conexão com o node no cluster criado
16. - adicionar o mongoose como dependência do projeto
    1. importar o mongoose no arquivo server
    2. connectar com a configuração fornecida no mongo atlas
17. - estruturar pastas MVC
18. - criar model User.js
19. - criar estrutura mongoose do User
20. - criar SessionController.js
21. - importar o SessionController nas rotas e chamar o seu método store
22. - criar um novo usuário através da rota do post, só criar se o usuário não exisitir no banco
22. - criar model Spot
23. - criar SpotController
24. - criar configuração de upload de imagens para o spot com multer dependência
25. - criar model Booking
26. - criar BookingController
27. - estruturar as rotas especificas para cada controller
