# Herramientas Computacionales → Clase 04 → 1/09/2025

Veamos lo que ya se ha podido avanzar.

| Nombre | Cuenta en GitHub | Trabajo de la clase pasada |
| :--------------- | :--------------- | :--------------- |
| Claudio Abarca | https://github.com/Kupaa-0 | https://kupaa-0.github.io/Clase-2/ |
| Anaís Aedo | https://github.com/anaisvalentina | https://anaisvalentina.github.io/Clase-2/ |
| Carol Álvarez | https://github.com/CarolMabel | https://carolmabel.github.io/clase2/ |
| Martina Araos | https://github.com/martina-af | https://martina-af.github.io/clase-3/ |
| Valentina Ávila | https://github.com/valentinaavila21 | https://valentinaavila21.github.io/mi_segunda_web/ |
| Camila Calquín | https://github.com/Camila-calquin | https://camila-calquin.github.io/Segundo-trabajo/ |
| Javier Castillo | https://github.com/javvierCC | https://javviercc.github.io/segunda-vez-mish/ |
| Angelina Caviedes | https://github.com/gilicvnz | https://gilicvnz.github.io/segunda_vez/ |
| Millaray Dinamarca | https://github.com/milladincea | https://milladincea.github.io/segundavezmillantitos/ |
| Catalyna Dunsmore | https://github.com/catadunsmore | https://catadunsmore.github.io/Clase-2/ |
| Fernanda García | https://github.com/marfghid | https://marfghid.github.io/hercom-02/ |
| Antonia Lara | https://github.com/antonialarah | https://antonialarah.github.io/clase-2/ |
| Antonia Mardones | https://github.com/antoniamardones | https://antoniamardones.github.io/clase-2/ |
| Ayline Marín | https://github.com/aylineoff | Pendiente |
| Vicente Medina | https://github.com/vicentemedinat | https://vicentemedinat.github.io/Clase_2/ |
| Constanza Ortega | https://github.com/shootingstarcony | https://shootingstarcony.github.io/Segundo-trabajo/ |
| Sayen Padilla | https://github.com/evorakie | https://evorakie.github.io/03-herramientas-computacionales/ |
| Sofia Parra | https://github.com/SofiaParraLunaUCH | Pendiente |
| Giulia Pepe | https://github.com/catsgugu | https://catsgugu.github.io/Mi-segundo-post-jaja-ya-soy-pro/ |
| Renata Pereira | https://github.com/lenapereoso | https://lenapereoso.github.io/oli-2/ |
| Bastián Petric | https://github.com/Bastich03 | https://bastich03.github.io/Clase_25_08/ |
| Francisco Pino | https://github.com/FranciscoPinoAUCh | Pendiente |
| Benjamín Rivas | https://github.com/benjaminrivasm | https://benjaminrivasm.github.io/herramientas-computacionales/clase-03/ |
| Antonia Solar | https://github.com/antoniasolar | https://antoniasolar.github.io/clase-2/ |
| Alanis Soto | https://github.com/Alanissq | https://alanissq.github.io/herramientas-computacionales-2/ |
| Veronica Soto | https://github.com/ronnistp | https://ronnistp.github.io/clase-03-herramientas/ |
| Valentina Troncoso | https://github.com/valentinatroncoso | https://valentinatroncoso.github.io/clase-2/ |
| Martina Urzúa | https://github.com/martinaurzua | https://martinaurzua.github.io/mi-segunda-vez/ |
| Diego Vera | https://github.com/DiegoV29-AST | https://diegov29-ast.github.io/clase_2_otra_vez_waos/ |

Lo primero que corresponde rescatar del trabajo de la semana pasada y de la previa, en un informe breve, formal y organizado encargado de [ChatGP](https://chatgpt.com/s/t_68b5d77b8a688191bb4289aa11198d3a):

*Tras el análisis de las intenciones de aprendizaje expresadas por los estudiantes, se identifican las siguientes coincidencias y prioridades temáticas*:

### 1. Programación y Desarrollo Web

* Alta frecuencia de interés en aprender **programación básica y avanzada**.
* Interés por **desarrollo web** (HTML, JavaScript, creación de páginas).
* Preferencia por aprender a **usar código como medio de expresión visual**.

### 2. Manejo de Software de Edición y Diseño

* Múltiples menciones a programas como **Illustrator, Photoshop e InDesign**.
* Interés en **After Effects para edición de video**.
* Énfasis en **aprovechar mejor las herramientas de diseño digital** ya conocidas.

### 3. Modelado y Herramientas 3D

* Recurrente interés en **modelado en 3D** y uso de programas relacionados (ej. Blender).
* Deseo de integrar herramientas 3D como complemento al diseño gráfico.

### 4. Exploración de Nuevas Herramientas Digitales

* Apertura a **descubrir nuevos programas y métodos de trabajo**.
* Búsqueda de **retos creativos y experimentación con software variado**.

### 5. Dimensión Personal y Motivacional

* Expresiones vinculadas a **aprender lo más posible** y **nivelar lagunas de conocimiento**.
* Menciones al deseo de **no estresarse**, **disfrutar el proceso** y **ser feliz aprendiendo**.

**Conclusión:**
Las principales coincidencias se concentran en **programación/desarrollo web**, **software de diseño y edición (Adobe Suite)** y **modelado 3D**. Como preferencias complementarias, destacan la exploración de nuevas herramientas digitales y la motivación personal por un aprendizaje significativo, desafiante y disfrutable.

- - - - - 

Ahora, volviendo al asunto de **Programación y Desarrollo Web**, del que ya estamos aprendiendo:

Podríamos juntar y separar lo que corresponde a cada lenguaje que debemos reconocer en el código fuente de una página web. 

En el código fuente de una página podríamos usar `<etiquetas></etiquetas>` que no demarcan a un elemento de HTML, sino que abren y cierra un espacio para usar otro lenguaje, distinto de HTML.

- Si uso las etiquetas `<svg></svg>`: Puedo incluir SVG.

- Si uso las etiquetas `<style></style>`: Puedo incluir CSS.

- Su uso las etiquetas `<script></script>`: Puedo incluir JavaScript.

Hace sentido tener todo junto, aprovechando las etiquetas recién indicadas, si el código fuente es breve. 

Pero si el código es muy extenso, o parte del código debe afectar a distintas páginas HTML, lo mejor es separar cada lenguaje en su documento, con su propia extensión. 

- HTML en un `*.html`

- SVG en un `*.svg`

- CSS en un `*.css`

- JavaScript en un `*.js`

- - - - - - - -




[← Clase 03](https://github.com/profesorfaco/herramientas/tree/main/clase-03) | [Clase 05 →](https://github.com/profesorfaco/herramientas/tree/main/clase-05)



