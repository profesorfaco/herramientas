# Herramientas Computacionales → Clase-10 → 20/10/2025

### Modelando con Blender

En la clase exploratoria de [la semana pasada](https://github.com/profesorfaco/herramientas/tree/main/clase-09) se dijo, más de una vez, **Geometría** y **Mesh**. Lo dicho se refería a la base del modelado 3D en Blender.

Entender tal base es el primer paso para crear cualquier objeto, sea un simple cubo, una máscaras de Halloween o algo mucho más complejo. Por eso conviene leer lo que sigue:

#### Geometría

La **Geometría** es el término amplio que describe forma, tamaño, posición, propiedades de los objetos en el espacio 3D. En el contexto de Blender. Refiere a **todo lo que tiene una forma espacial**.

La calidad de la geometría insidirá en cómo el objeto interactúa con las luces y las sombras, y cómo puede [modificarse](https://www.youtube.com/watch?v=qIlXmWFZxyQ). 

Una "buena geometría" a veces es llamada "buena topología", otro concepto usado en la clase recién pasada.

#### Mesh (Malla)

**Mesh** (Malla) es el tipo de geometría más común y el principal con el que se trabaja en Blender. Es la estructura digital que define la superficie de un objeto 3D. Una malla está compuesta por tres elementos interconectados:

1. **Vértices (Vertices):** Los puntos individuales en el espacio que definen la ubicación de la malla. Son los bloques de construcción básicos.

2. **Bordes (Edges):** Las líneas que conectan dos vértices. Forman el esqueleto de la malla.

3. **Caras (Faces):** Las superficies planas delimitadas por los bordes (idealmente cuatro, llamados **Quads**, aunque Blender también usa **Tris** (tres lados) o **N-gons** (más de cuatro lados)). Estas caras son lo que ves y lo que se renderiza.

Sea que agreguemos un cubo o un mono, Blender añadirá un **Mesh**. Para darle forma, trabajas en el **Modo Edición** (Edit Mode) moviendo, añadiendo o eliminando sus **vértices, bordes y caras**.




