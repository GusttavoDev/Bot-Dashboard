# Bot-Dashboard
Tutorial Site com Dashboard para bot Discord

<img src="https://media.discordapp.net/attachments/829462283553210378/856352058609369148/unknown-2.png">

<h3>API'S USADAS</h3>
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

<h2>CREDITOS</h2>
• Gusttavo Dev
