# Jhonatan Caro Suárez

Desarrollador web full stack. Técnico Superior en Desarrollo de Aplicaciones Web y actualmente cursando un **Máster en Big Data e Inteligencia Artificial**.

Esa combinación es la que me interesa: aplicaciones que no solo guardan datos, sino que los convierten en algo que sirve para decidir. Mi proyecto principal va exactamente de eso — importar archivos de ventas desordenados y sacar de ellos estadísticas fiables.

Busco mi primera posición como desarrollador, en ESPAÑA - AlMERIA o en remoto.

---

## Stack

| | |
|---|---|
| **Lenguajes** | JavaScript · TypeScript · Python · Java · PHP |
| **Frontend** | React · Tailwind CSS · HTML · CSS |
| **Backend** | Node.js · Express · FastAPI · APIs REST · JWT |
| **Bases de datos** | PostgreSQL · MySQL |
| **IA / LLMs** | Integración de agentes conversacionales sobre datos propios |
| **Herramientas** | Docker · Git · GitHub · Figma · VS Code |
| **CMS** | WordPress |

---

## Proyecto destacado

### [Stocken-Data](https://github.com/Jhonatan-Caro/Stocken-Data)

Plataforma de gestión de inventario y análisis de ventas para pequeño comercio. Importa archivos CSV y XLSX —cada tienda exporta con nombres de columna distintos— y los normaliza mediante un mapeo dinámico de campos, para poder calcular estadísticas fiables sobre datos que llegan sin estructura fija.

[![Panel de estadísticas de Stocken-Data](https://raw.githubusercontent.com/Jhonatan-Caro/Stocken-Data/main/docs/grafica-mes.png)](https://github.com/Jhonatan-Caro/Stocken-Data)
[![Panel de estadísticas de Stocken-Data](https://raw.githubusercontent.com/Jhonatan-Caro/Stocken-Data/main/docs/grafica-mediana-canal.png)](https://github.com/Jhonatan-Caro/Stocken-Data)

`React` `Node.js` `Express` `Python` `FastAPI` `PostgreSQL` `Docker` `Tailwind`

Dos problemas que me obligaron a pensar en arquitectura y no solo en código:

**Estadísticas fiables sobre columnas que cambian.** Los campos que el usuario mapea van a columnas tipadas, porque agrupar por JSONB deja de funcionar cuando un cliente llama `canal` a lo que otro llama `Sales Channel`. La fila original se conserva íntegra en JSONB, sin perder nada de lo que se subió.

**Un asistente conversacional que no se inventa datos.** En vez de dejar que el modelo genere SQL libre, el agente consume las mismas consultas que alimentan el panel, expuestas como endpoints del backend y replicadas en Python. Así el chatbot y el dashboard responden siempre con la misma información, y el modelo nunca toca la base de datos directamente.

[→ Ver el proyecto y el resto de decisiones técnicas](https://github.com/Jhonatan-Caro/Stocken-Data)

---

## Formación

- **Máster en Big Data e Inteligencia Artificial** — en curso
- **Técnico Superior en Desarrollo de Aplicaciones Web (DAW)**

## Contacto

- **LinkedIn:** [jhonatan-caro-suarez](https://www.linkedin.com/in/jhonatan-caro-b29b47412/)
- **Email:** jhonycaro1301@gmail.com
