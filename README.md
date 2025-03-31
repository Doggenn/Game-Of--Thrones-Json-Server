# 🏰 Game of Thrones - JSON Server  
📜 Servidor JSON con información sobre Juego de Tronos.  

Este **JSON Server** proporciona datos sobre personajes, casas y eventos de Juego de Tronos.  
Puede usarse para proyectos front-end sin necesidad de una base de datos real.  

## 🌐 API Pública (Vercel)
💡 No es necesario instalar el servidor, ya que está disponible en Vercel:  
🔗 **[https://game-of-thrones-json-server-one.vercel.app](https://game-of-thrones-json-server-one.vercel.app)**  

### 🔍 **Ejemplos de Endpoints:**  
- 🔗 **Todos los personajes:** [`/characters`](https://game-of-thrones-json-server-one.vercel.app/characters)  
- 🔗 **Todas las casas:** [`/houses`](https://game-of-thrones-json-server-one.vercel.app/houses)  
- 🔗 **Detalles de un personaje:** [`/characters/1`](https://game-of-thrones-json-server-one.vercel.app/characters/1)  

---

## ⚙️ **Cómo ejecutar en local**  
Si prefieres correr el servidor en tu PC:  

### 1️⃣ Clonar el repositorio  
```bash
git clone https://github.com/Doggenn/Game-Of--Thrones-Json-Server.git
cd Game-Of--Thrones-Json-Server
```
### 2️⃣ Instalar dependencias
```bash
npm install
```
### 3️⃣ Iniciar el servidor JSON
```bash
npm start
```
### 📌 Por defecto, la API estará en:
🔗 http://localhost:3000

### 📁 Estructura de la base de datos (db.json)
Este servidor utiliza un archivo JSON con la siguiente estructura:
```json
{
  "characters": [
    {
      "id": 1,
      "name": "Jon Snow",
      "house": "Stark",
      "alive": true
    }
  ],
  "houses": [
    {
      "id": 1,
      "name": "Stark",
      "motto": "Winter is Coming"
    }
  ]
}
```

### 📌 Uso con Fetch / Axios
Puedes consumir la API desde tu aplicación con JavaScript, React, Vue, etc.

🔹 Ejemplo con fetch
```js
fetch("https://game-of-thrones-json-server-one.vercel.app/characters")
  .then(response => response.json())
  .then(data => console.log(data));

```
🔹 Ejemplo con Axios
```js
import axios from "axios";

axios.get("https://game-of-thrones-json-server-one.vercel.app/characters")
  .then(response => console.log(response.data));

```

<!--
### 🚀 Cómo ejecutar la base de datos localmente:

Si quieres ejecutarlo en tu PC, clona el repositorio y usa los siguientes comandos:
   ```bash
   git clone https://github.com/Doggenn/Game-Of--Thrones-Json-Server.git
   cd Game-Of--Thrones-Json-Server
   npm install
   npm start
   ```
 # game-of-thrones-json-server

 Characters

 http://localhost:3000/characters
 
Filter characters

 http://localhost:3000/characters?name=Jon%20Snow

Detail characters (donde 5 es el id del personaje)

 http://localhost:3000/characters/5

Houses

 http://localhost:3000/houses

Detail houses (donde 2 es el id de la casa)

 http://localhost:3000/houses/2
 
-->
