# Herramientas Computacionales → Clase-08 → 6/10/2025

### Trabajo práctico, en sala (20% del promedio final)

Hoy ponemos a prueba lo avanzado en InDesign con una publicación breve.

La calificación resulta del promedio de 2 pautas (cada nota tiene misma importancia o peso): 

**Primera pauta**:

| Pts. | Criterio |
|:----:|:-----------------|
| 0,5 | Para el texto extenso utiliza un sucedáneo de fuente clásica ofrecida por Google Fonts (Crimson Pro, que es suficientemente parecida a Minion Pro) |
| 0,5 | Utiliza una segunda fuente de Google Fonts, propuesta por un *prompt* que debe ceñirse a la indicación e informarse debidamente. Esta segunda fuente destaca o diferencia partes del mismo texto |
| 0,5 | Se limita a utilizar los cuerpos, grosores y estilos necesarios para establecer, cada vez, sólo una distinción de unos textos sobre otros |
| 0,5 | Cuida el promedio de 60 caracteres por línea cuando el texto está justificado a ambos lados, y evita tal justificación cuando el promedio de caracteres es menor. |
| 0,5 | Utiliza espacio entre líneas (interlínea), espacio entre letras (interletra) y espacio entre palabras adecuados a una lectura que “camina sin tropiezos”. |
| 0,5 | Usa sangrías discretas para diferencias párrafos, manteniendo su articulación en un bloque de texto y evitando marcaciones redundantes de párrafos. |
| 0,5 | Evita “viudas” y “huérfanas”. |
| 0,5 | Evita dejar algunas palabras completamente en mayúsculas o siglas dentro de un texto extenso. |
| 1,0 | Mejora imágenes reales con Inteligencia Artificial Generativa para sacar el mejor provecho posible a su presentación | 
| 1,0 | Ajusta datos reales con Inteligencia Artificial Generativa para informar y persuadir de sus capacidades y méritos en función de propuestas laborales específicas |
| 1,0 | Punto base |

- - - - - 

**Segunda pauta**:

El resultado debe publicarse en una página web, como PDF. La página web debe basarse en el siguiente código fuente, generado, en parte, con [Claude](https://claude.ai/):

```

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Portafolio en PDF</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Climate+Crisis&display=swap');

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* 
            Primer punto:
            Cambie los colores, usando alguna armonía de color tomada de 
            https://color.adobe.com/es/create/color-wheel
            Indique en este comentario la armonía que decide utilizar 
        */

        :root{
            --colorPrincipal:#4DDBD6;
            --colorOpuesto:#DB4DBF;
            --colorMediador:#DBC24D;
        }

        /* 
            No sería necesario hacer más ajustes en el CSS 
        */

        body {
            font-family: Helvetica, Arial, sans-serif;
            background-color: #FFF;
            color: #000;
            overflow-x: hidden;
        }

        a{
            color:black;
        }

        a:hover{
            text-decoration: none;
        }

        .container {
            min-height: 100vh;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 0;
        }

        /* ===========LO QUE VA A LA IZQUIERDA, O ARRIBA============== */

        .left-section {
            background-color: var(--colorPrincipal);
            padding: 80px 60px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            border-right: 8px solid #000;
            position: relative;
        }

        /* 
            Pero revise la extensión de su nombre, 
            podría requerir un ajuste de font-size, 
            y nada más.
        */


        h1 {
            font-family: "Climate Crisis", sans-serif;
            font-weight: 400;
            font-size: calc(2rem + 2vw);
            line-height: 1.1;
            margin-bottom: 30px;
            text-transform: uppercase;
            position: relative;
            z-index: 1;
        }

        p {
            font-weight: 800;
            font-size: calc(1rem + 0.5vw);
            line-height: 1.5;
            margin-bottom: 50px;
            position: relative;
            z-index: 1;
        }

        .download-btn {
            font-family: "Climate Crisis", sans-serif;
            letter-spacing: 2px;
            font-size: calc(0.75rem + 0.75vw);
            background-color: var(--colorMediador);
            color: #000;
            border: 6px solid #000;
            padding: 25px 50px;
            text-transform: uppercase;
            cursor: pointer;
            box-shadow: 12px 12px 0 #000;
            transition: all 0.1s ease;
            text-decoration: none;
            display: inline-block;
            width: fit-content;
            position: relative;
            z-index: 1;
        }

        .download-btn:hover {
            transform: translate(4px, 4px);
            box-shadow: 8px 8px 0 #000;
        }

        .download-btn:active {
            transform: translate(8px, 8px);
            box-shadow: 4px 4px 0 #000;
        }

        /* ===========LO QUE VA A LA DERECHA, O ABAJO============== */

        .right-section {
            background-color: var(--colorOpuesto);
            padding: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }

        .mugshot-container {
            width: 100%;
            max-width: 500px;
            position: relative;
        }

        .mugshot-frame {
            border: 8px solid #000;
            box-shadow: 20px 20px 0 #000;
            background-color: #FFF;
            padding: 20px;
            transform: rotate(2deg);
            transition: transform 0.3s ease;
        }

        .mugshot-frame:hover {
            transform: rotate(-1deg) scale(1.02);
        }

        .mugshot {
            width: 100%;
            height: auto;
            background:black;
        }

        .mugshot img{
            border: 4px solid #000;
            border-bottom: 1px solid #000;
            width: 100%;
            height: auto;
            object-fit: cover;
            aspect-ratio: 1 / 1;
        }

        .badge {
            font-family: "Climate Crisis", sans-serif;
            position: absolute;
            top: -30px;
            right: -30px;
            background-color: var(--colorMediador);
            color: #000;
            padding: 20px 30px;
            border: 5px solid #000;
            border-radius: 50%;
            font-size: 1rem;
            font-weight: 400;
            transform: rotate(15deg);
            box-shadow: 8px 8px 0 #000;
            z-index: 2;
        }

        /* ===========AJUSTES SEGÚN PANTALLAS============== */


        @media (max-width: 992px) {
            .container {
                grid-template-columns: 1fr;
            }

            .left-section {
                border-right: none;
                border-bottom: 8px solid #000;
            }
        }

        @media (max-width: 576px) {
            .left-section, .right-section {
                padding: 50px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="left-section">
            <!--segundo punto por los ajuste en la sección izquierda-->
            <h1>NOMBRE APELLIDO</h1>
            <p>Reemplace este texto, manteniendo la brevedad y usando un <a href="https://www.nngroup.com/videos/tone-of-voice-dimensions/" target="_blank">tono de voz</a> que coincida con el <a href="https://www.nngroup.com/articles/neobrutalism/" target="_blank">neobrutalismo</a> que inspira el estilo de la página; y cambie la foto por un retrato suyo.</p>
            <!--suba el PDF a GitHub y cambie la referencia de hipertexto-->
            <a href="#" class="download-btn" download>MI PORTAFOLIO</a>
        </div>
        
        <div class="right-section">
            <!--tercer punto por los ajuste en la sección izquierda-->
            <div class="mugshot-container">
                <div class="badge">
                    <!--vincule a su cuenta en GitHub-->
                    <a href="#" target="_blank">2025</a>
                </div>
                <div class="mugshot-frame">
                    <div class="mugshot">
                        <!--incluya la misma imagen que utiliza en su portafolio, a resolución, tamaño y peso adecuado para la web-->
                        <img src="https://picsum.photos/500/500.jpg">
                    </div>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
```

- - - - - 

Corresponde revisar las indicaciones dejadas como comentarios en el código fuente recién desplegado para poder obtener 3 puntos. A los que se le sumarán 4 que considerarán:

- Calidad de CV en portafolio en PDF descargable (0,0 a 1,0), considerando [imagen personal adaptada a un tono pertinente a su identidad](https://bananaprompts.xyz/), además de un texto adaptado a determinada oferta laboral de su interés.

- Calidad de presentación de trabajos en PDF descargable (0,0 a 1,0), considerando nivel y votación del curso.

- Calidad de cubierta en continuidad con contracubierta, página de créditos (página legal o nota de edición) y colofón en PDF descargable (0,0 a 1,0), considerando nivel y votación del curso.

- Punto base de 1,0.

- - - - - 

### Entregas

| Nombre | Web | Creada | PDF descargable |
|:-----------|:-------------------------|:-----:|:-------:| 
| [Claudio Abarca](https://github.com/Kupaa-0/segunda-nota/) | https://kupaa-0.github.io/segunda-nota | P | P |
| [Anaís Aedo](https://github.com/anaisvalentina/segunda-nota/) | https://anaisvalentina.github.io/segunda-nota/ | ✓ | P |
| [Carol Álvarez](https://github.com/CarolMabel/segunda-nota/) | https://carolmabel.github.io/segunda-nota/ | ✓ | P |
| [Martina Araos](https://github.com/martina-af/segunda-nota/) | https://martina-af.github.io/segunda-nota/ | ✓ | P |
| [Valentina Ávila](https://github.com/valentinaavila21/segunda-nota/) | https://valentinaavila21.github.io/segunda-nota/ | ✓ | P |
| [Camila Calquín](https://github.com/Camila-calquin/segunda-nota/) | https://camila-calquin.github.io/segunda-nota/ | ✓ | P |
| [Javier Castillo](https://github.com/javvierCC/segunda-nota/) | https://javviercc.github.io/segunda-nota/ | P | P |
| [Angelina Caviedes](https://github.com/gilicvnz/segunda-nota/) | https://gilicvnz.github.io/segunda-nota/ | ✓ | P |
| [Millaray Dinamarca](https://github.com/milladincea/segunda-nota/) | https://milladincea.github.io/segunda-nota/ | ✓ | P |
| [Catalyna Dunsmore](https://github.com/catadunsmore/segunda-nota/) | https://catadunsmore.github.io/segunda-nota/ | P | P |
| [Fernanda García](https://github.com/marfghid/segunda-nota/) | https://marfghid.github.io/segunda-nota | ✓ | P |
| [Antonia Lara](https://github.com/antonialarah/segunda-nota/) | https://antonialarah.github.io/segunda-nota/ | P | P |
| [Antonia Mardones](https://github.com/antoniamardones/segunda-nota/) | https://antoniamardones.github.io/segunda-nota/ | P | P |
| [Ayline Marín](https://github.com/aylineoff/segunda-nota/) | https://aylineoff.github.io/segunda-nota | P | P |
| [Vicente Medina](https://github.com/vicentemedinat/segunda-nota/) | https://vicentemedinat.github.io/segunda-nota/ | P | P |
| [Constanza Ortega](https://github.com/shootingstarcony/segunda-nota/) | https://shootingstarcony.github.io/segunda-nota/ | ✓ | P |
| [Sayen Padilla](https://github.com/evorakie/segunda-nota/) | https://evorakie.github.io/segunda-nota/ | ✓ | P |
| [Sofia Parra](https://github.com/SofiaParraLunaUCH/segunda-nota/) | https://sofiaparralunauch.github.io/segunda-nota/ | ✓ | P |
| [Giulia Pepe](https://github.com/catsgugu/segunda-nota/) | https://catsgugu.github.io/segunda-nota/ | P | P |
| [Renata Pereira](https://github.com/lenapereoso/segunda-nota/) | https://lenapereoso.github.io/segunda-nota/ | P | P |
| [Bastián Petric](https://github.com/Bastich03/segunda-nota/) | https://bastich03.github.io/segunda-nota/ | ✓ | P |
| [Francisco Pino](https://github.com/FranciscoPinoAUCh/segunda-nota/) | https://franciscopinoauch.github.io/segunda-nota/ | ✓ | P |
| [Benjamín Rivas](https://github.com/benjaminrivasm/segunda-nota/) | https://benjaminrivasm.github.io/herramientas-computacionales/segunda-nota/ | P | P |
| [Antonia Solar](https://github.com/antoniasolar/segunda-nota/) | https://antoniasolar.github.io/segunda-nota/ | P | P |
| [Alanis Soto](https://github.com/Alanissq/segunda-nota/) | https://alanissq.github.io/segunda-nota/ | P | P |
| [Veronica Soto](https://github.com/ronnistp/segunda-nota/) | https://ronnistp.github.io/segunda-nota/ | ✓ | P |
| [Valentina Troncoso](https://github.com/valentinatroncoso/segunda-nota/) | https://valentinatroncoso.github.io/segunda-nota/ | ✓ | P |
| [Martina Urzúa](https://github.com/martinaurzua/segunda-nota/) | https://martinaurzua.github.io/segunda-nota/ | ✓ | P |
| [Diego Vera](https://github.com/dv29ast/segunda-nota/) | https://dv29ast.github.io/segunda-nota/ | P | P |



- - - - - 

[← Clase 07](https://github.com/profesorfaco/herramientas/tree/main/clase-07) | [Clase 09 →](https://github.com/profesorfaco/herramientas/tree/main/clase-09)
