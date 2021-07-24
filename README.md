# Bot-Dashboard
Tutorial Site com Dashboard para bot Discord

**Tutorial YouTube**: 

<img src="https://media.discordapp.net/attachments/829462283553210378/856352058609369148/unknown-2.png">

<h3>LIB'S USADAS</h3>
• EXPRESS
</br>
• EJS
</br>
• DISCORD.JS

<h3>USANDO EXPRESS<h3>


```js
const express = require('express');//express
const { port } = require('./config.json');//arquivo com dados do bot/site

const app = express();

app.set('view engine', 'ejs');
app.use(express.static('public'))

app.listen(port, () => console.log(`App listening at http://localhost:${port}`));

```
    
<h3>CSS<h3>

<p>em server.js coloque</p>
    
```js
app.use('/css', express.static(__dirname + 'public/css'));
```
<p>em seguida crie uma pasta public e uma css apos isso você ja podera colocar seus arquivos .css</p>

<h3>USANDO ROTAS<h3>

```js
//verificando se a rota e https://dominio.com/menu
app.route('/menu').get((req, res) => {
    res.render('menu');//irá renderizar o arquivo menu.ejs
  }).post((req, res) => {
    console.log('processing...')//aguardando renderizar o arquivo
    res.send('processing...')
  });

app.get('/', (request, response) => {
 let html = 'index';
  response.render(html);//renderizando a pagina padrão index.ejs
});

```
    
<h3>CONFIG.JS<h3>
    
```json
{
	"clientID": "854395492364058674",
	"clientSecret": "W_7dIi97-zQMNMd25hA8rXst3pSxR4BN",
	"port": 53134
} 
```


<h2>CREDITOS</h2>
• Gusttavo Dev
