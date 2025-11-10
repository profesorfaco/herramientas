# Herramientas Computacionales → Clase-13 → 10/11/2025

Seguimos avanzando.

De tener un arreglo (`[…]`) con detalles de cada trabajo en objetos ([{…},{…},{…}]), pasaremos a tener un JSON. 

Si antes teníamos un arreglo, dentro del código JavaScript, que se llamaba `trabajitos` y debíamos repetir en `index.html` y `single.html`, ahora tendremos un documento independiente que se llamará `trabajitos.json`.

JSON (JavaScript Object Notation - Notación de Objetos de JavaScript) es un formato ligero de intercambio de datos que utiliza convenciones que son conocidas por los programadores que trabajan en C, C++, C#, Java, Python, etc. Por eso JSON es ideal para el intercambio de datos.

El gran cambio respecto de lo anterior está en unas comillas más.

Si antes cada trabajo debía describirse: 

```
{
	id: 1,
	photo: "https://anaisvalentina.github.io/primera-nota/img/lahora.webp",
	title: "La hora de conectarnos",
	course: "Proyecto III",
}
```

En JSON debe describirse:

```
{
	"id": 1,
	"photo": "https://anaisvalentina.github.io/primera-nota/img/lahora.webp",
	"title": "La hora de conectarnos",
	"course": "Proyecto III",
}
```


Aprovechando este cambio, agregaremos un par de datos más por cada trabajo, para que termine estructurándose de la siguiente manera: 

```
{
	"id": 1,
	"photo": "https://raw.githubusercontent.com/anaisvalentina/imagenes/refs/heads/main/te.webp",
	"title": "La hora de conectarnos",
	"course": "Proyecto III",
	"description": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed rutrum hendrerit lorem. Curabitur sodales feugiat libero. Nullam in lorem ut sem tempor accumsan nec vitae lacus. Sed vel finibus ex, quis euismod lorem. Aliquam eget leo sapien. Proin velit diam, suscipit vitae mi vel, laoreet finibus nisl. Pellentesque a purus eleifend, congue ante nec, aliquam risus.",
	"gallery": "https://raw.githubusercontent.com/profesorfaco/herramientas/refs/heads/main/clase-13/gallery.webp"
}
```

La `description` aportará un texto que, idealmente, dé indicaciones de estar terminando un ciclo que, según reglamento de carrera: 

> tiene como objetivo fundamental formar al (a la) estudiante para observar, interactuar y comprender su entorno, estableciendo una mirada crítica y problematizándolo mediante el análisis y diagnóstico inicial. A partir de ello el (la) estudiante podrá idear soluciones innovadoras que se traducirán en modelos conceptuales y físicos. Al finalizar la etapa, el (la) estudiante reconocerá problemas esenciales, modelará y formalizará posibles soluciones mediante metodologías y herramientas propias de la disciplina, y habrá adquirido las competencias básicas para conceptualizar, representar y comunicar sus propuestas de Diseño.

La `gallery` debe ser única imagen, que se vean como un conjunto de imágenes que nos muestran distintas perspectivas del mismo trabajo.


- - - - - - -


| 🎓 Generación 2025 🎓 | Clase 13 |
|:----------------|:-----:|
| https://disenouchile.github.io/portafolio/alanis_soto | P | 
| https://disenouchile.github.io/portafolio/anais_aedo | x | 
| https://disenouchile.github.io/portafolio/angelina_caviedes | P | 
| https://disenouchile.github.io/portafolio/antonia_lara | P | 
| https://disenouchile.github.io/portafolio/antonia_mardones | P | 
| https://disenouchile.github.io/portafolio/antonia_solar | P | 
| https://disenouchile.github.io/portafolio/ayline_marin | P | 
| https://disenouchile.github.io/portafolio/bastian_petric | P | 
| https://disenouchile.github.io/portafolio/benjamin_rivas | ✅ | 
| https://disenouchile.github.io/portafolio/camila_calquin | P | 
| https://disenouchile.github.io/portafolio/carol_alvarez | P | 
| https://disenouchile.github.io/portafolio/catalyna_dunsmore | ✅ | 
| https://disenouchile.github.io/portafolio/claudio_abarca | P | 
| https://disenouchile.github.io/portafolio/constanza_ortega | ✅ | 
| https://disenouchile.github.io/portafolio/diego_vera | P | 
| https://disenouchile.github.io/portafolio/fernanda_garcia | x | 
| https://disenouchile.github.io/portafolio/francisco_pino | P | 
| https://disenouchile.github.io/portafolio/giulia_pepe | P | 
| https://disenouchile.github.io/portafolio/javier_castillo | P | 
| https://disenouchile.github.io/portafolio/martina_araos | P | 
| https://disenouchile.github.io/portafolio/martina_urzua | P | 
| https://disenouchile.github.io/portafolio/millaray_dinamarca | P | 
| https://disenouchile.github.io/portafolio/renata_pereira | P | 
| https://disenouchile.github.io/portafolio/sayen_padilla | P | 
| https://disenouchile.github.io/portafolio/sofia_parra | P | 
| https://disenouchile.github.io/portafolio/valentina_avila | P | 
| https://disenouchile.github.io/portafolio/valentina_troncoso | P | 
| https://disenouchile.github.io/portafolio/veronica_soto | P | 
| https://disenouchile.github.io/portafolio/vicente_medina | P | 


- - - - - - - 

#### Para más adelante:

¿Sabía ud. que puede usar GitHub Pages con dominios de primer nivel?

Los dominios de primer nivel pueden ser geográficos ([ccTLD – country code Top Level Domains](https://es.wikipedia.org/wiki/Dominio_de_nivel_superior_geogr%C3%A1fico)) o genéricos ([gTLD – generic Top Level Domains](https://es.wikipedia.org/wiki/Dominio_de_nivel_superior_gen%C3%A9rico))

Por ejemplo, `minombre.cl` es uno geográfico. Mientras `minombre.com` es uno genérico.

Es posible configurar un sitio de tal tipo con GitHub Pages. O sea, con lo mismo que han podido aprender hasta ahora, podría crear su sitio web personal, con un dominio profesional. Para hacerlo, recomiendo guiarse con:

- **Artículo: [Configurar GitHub Pages para usar dominios.cl](https://ggerena.medium.com/configurar-github-pages-para-usar-dominios-cl-13c1a644699f)**

- Video de complemento al artículo: [Hosting gratuito con GitHub Pages y dominio personalizado](https://www.youtube.com/watch?v=nbUR1jzVI5g&t=328s)

- Otro video de complemento al artículo: [Hosting GRATIS con Dominio propio (Dominio Personalizado Github Pages)](https://www.youtube.com/watch?v=tzjl91RP_To)

**Toma algunos minutos seguir los pasos descritos en el [artículo](https://ggerena.medium.com/configurar-github-pages-para-usar-dominios-cl-13c1a644699f)**. No exige horas. Sí exige concentrarse mucho en tales minutos

- - - - - 

[← Clase 12](https://github.com/profesorfaco/herramientas/tree/main/clase-12) | [Clase 14→](https://github.com/profesorfaco/herramientas/tree/main/clase-14)

