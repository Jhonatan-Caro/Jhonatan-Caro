# Jhonatan Caro Suárez

Desarrollador web full stack. Técnico Superior en Desarrollo de Aplicaciones Web y actualmente cursando un **Máster en Big Data e Inteligencia Artificial**.

Esa combinación es la que me interesa: aplicaciones que no solo guardan datos, sino que los convierten en algo que sirve para decidir. Mi proyecto principal va exactamente de eso — importar archivos de ventas desordenados y sacar de ellos estadísticas fiables.

Busco mi primera posición como desarrollador, en ESPAÑA - AlMERIA o en remoto.

jhonatancaro.dev

---

## Stack

| | |
|---|---|
| **Lenguajes** | JavaScript · TypeScript · Python · Java · PHP |
| **Frontend** | React · Next.js · Vue.js · Tailwind CSS · HTML · CSS |
| **Backend** | Node.js · Express · Laravel · FastAPI · APIs REST · JWT |
| **Bases de datos** | PostgreSQL · MySQL |
| **IA / LLMs** | Integración de agentes conversacionales sobre datos propios |
| **Cloud** | AWS(S3, CloudFront, ACM) · Cloudflare DNS |
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

### [Portfolio · jhonatancaro.dev](https://jhonatancaro.dev/)

Sitio construido con Next.js y TypeScript, exportado como estático y desplegado en Amazon S3. Se distribuye con CloudFront sobre HTTPS mediante un certificado de ACM, y el DNS del dominio propio está gestionado en Cloudflare.

`Next.js` `React` `TypeScript` `Tailwind` `AWS S3` `CloudFront` `ACM` 

---

## Formación

- **Máster en Big Data e Inteligencia Artificial** — en curso
- **Técnico Superior en Desarrollo de Aplicaciones Web (DAW)**

## Ahora mismo

**Sistema RAG híbrido en Stocken-Data.** Las métricas de ventas se seguirán consultando con SQL —un embedding no sabe sumar ni comparar magnitudes— y la búsqueda vectorial se reserva para los playbooks de negocio, que sí son texto con significado. Sobre **pgvector**, en el mismo PostgreSQL del proyecto, para poder filtrar por usuario dentro de la propia consulta de similitud. En desarrollo.

**AWS.** Tras desplegar mi portfolio con S3, CloudFront y ACM, estudiando
EC2, Lambda y RDS.

**Validación en la importación de Stocken-Data:** sugerencia automática del
mapeo de columnas y comprobación del contenido antes de escribir en base
de datos.


## Contacto

- **LinkedIn:** [jhonatan-caro-suarez](https://www.linkedin.com/in/jhonatancarosuarez/)
- **Email:** jhonycaro1301@gmail.com
