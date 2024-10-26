# ¿Qué es la especificidad?

La especificidad es la manera mediante la cual los navegadores deciden qué valores de una propiedad CSS son más relevantes para un elemento y, por lo tanto, serán aplicados. La especificidad está basada en las reglas de coincidencia que están compuestas por diferentes tipos de selectores CSS.

## Introducción a los selectores básicos y cómo afectan la especificidad

Los selectores en CSS son patrones utilizados para seleccionar elementos HTML y aplicarles estilos. Comprender los selectores básicos y su especificidad es esencial para diseñar y desarrollar sitios web de manera efectiva. Algunos ejemplos son el selector de tipo, selector de clase, selector de ID, selector universal y selectores de atributo.

## Tabla de especificidad con diferentes tipos de selectores:

![image](https://github.com/user-attachments/assets/0a02e334-71c9-4353-8196-61379c466267)



### PARTE 2

![image](https://github.com/user-attachments/assets/15650ea4-ce57-4684-ad7e-b45e29d0b906)


- Selector de etiqueta (`p`) tiene especificidad de 1 y el color aplicado es azul.
- Selector por clase (`.container p`) tiene especificidad de 11 y el color aplicado es verde.
- Selector por ID (`#parrafo`) tiene especificidad de 100 y el color aplicado es rojo.

**Resultado final:** El color de texto será rojo porque la regla del ID (`#parrafo`) tiene la mayor especificidad (100).

Slides con ejemplos de especificidad: [Presentación de Slides](https://docs.google.com/presentation/d/1DGhsHSR-q982nFsyU7x7alpOBO5xjIfN7lnDzz4TKe4/edit?usp=sharing)

### 2.2

![image](https://github.com/user-attachments/assets/bd22c2d2-edc9-48b5-aa31-f6fca92ef21b)


**Resultado final:** El color será azul porque el `!important` tiene prioridad, independientemente de la especificidad.

### PARTE 3

![image](https://github.com/user-attachments/assets/b98922b5-1636-48b4-a45f-cea6d32d61a7)

**Pregunta:** ¿Qué color tendrá el título `<h1>`?

**Respuesta:** El título `<h1>` será de color rojo, pues el selector ID (`#main`) tiene mayor especificidad (100).

### 3.2

![image](https://github.com/user-attachments/assets/9fefd5ed-4fa3-4729-8872-72ce0f4597fe)

**Modificar el siguiente código para que el párrafo tenga color amarillo sin usar `!important`.**

**Respuesta:** La solución es poner un selector de ID (`#Box`) con el color amarillo, así tendrá mayor especificidad y el color será amarillo en vez de azul.

### PARTE 4

Basado en el siguiente código HTML, haga un CSS para lograr un diseño específico (El `<h1>` en el `.header` debe ser de color blanco, el texto `<p>` en `.content` debe ser rojo, el texto `<footer>` debe ser gris).

![image](https://github.com/user-attachments/assets/18cd5e5e-ff0f-4d3d-ac10-602074f3e6ca)

**Resultado CSS:**

![image](https://github.com/user-attachments/assets/325f2aa6-afc7-4372-b0bf-675a3b23ccf6)


