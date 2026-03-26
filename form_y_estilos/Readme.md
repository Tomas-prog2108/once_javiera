# Formularios y estilos

Hoy en la clase de Desarrollo de Software realizamos una actividad sobre **formularios y estilos**.

La actividad consistía en hacerle unos cambios a un archivo HTML y CSS que contenian un formulario.

Los cambios que hice fueron los siguientes:

1. Cambie el nombre del archivo HTML de "formulario.html" a "index.html".

2. Cambie el nombre del archivo CSS de "contacto.css" a "styles.css".

3. A el HTML le cambie la etiqueta `link`.
    
    Paso de: 
    ```html
    <link rel="stylesheet" href="contacto.css">
    ```
    A esto:
    ```html
    <link rel="stylesheet" href="style.css">
    ```
    Esto lo hice para que el archivo HTML se pueda conectar al archivo CSS.

4. Después cree un apartado en el fórmulario:
    ```html
    <div class="campo">
        <label for="Caracterización familiar">Personas con las que vive <span class="obligatorio">*</span></label>
        <input type="text"
        id="Caracterización familiar"
        name="Caracterización familiar"
        placeholder="Personas con las que vive"
        maxlength="1000">
      </div>
    ```
    
    - La etiqueta `div` es para **organizar la información.** O sea **crear una nueva sección en el formulario.**

    - La etiqueta `class` es para **aplicar estilos.**

    - La etiqueta `label` indica **qué debe escribir en el campo del formulario.** En este caso es para preguntar con **cuáles y con cuantas personas vive.**

    - El atributo `for` conecta el `label` con el `input`. En este caso es **"Caracterización familiar".**

    - La etiqueta `input` es el campo **donde el usuario debe escribir su respuesta.** O sea con cuáles personas vive.

    - El atributo `type="text`significa que **el usuario puede escribir un texto libre.**

    - El atributo `name` es el **nombre del campo cuando se envía el formulario al servidor.** En este caso es "Caracterización familiar".

    - El atributo `placeholder` es un **texto que aparece en gris dentro del recuadro de respuesta.** En este caso es **"Personas con las que vive".**

    - El atributo `maxlength` nos dice la **cantidad de caracteres que puede ir en la respuesta.** En este caso es de **1000 caracteres.**

5. Hice unos ajustos al CSS, como:

    Cambiar esto:

    ```css
    :root {
    --primario: #2563eb;
    --primario-oscuro: #1d4ed8;
    --texto: #1f2937;
    --texto-suave: #6b7280;
    --borde: #d1d5db;
    --fondo: #f9fafb;
    --blanco: #ffffff;
    --error: #dc2626;
    --exito: #16a34a;
    --radio: 8px;
    --sombra: 0 4px 20px rgba(0,0,0,0.08);
    }
    ```
    A esto:

    ```css
    :root {
    --primario: #3a4161;
    --primario-oscuro: #000630;
    --texto: #1f2937;
    --texto-suave: #6b7280;
    --borde: #d1d5db;
    --fondo: #f9fafb;
    --blanco: #ffffff;
    --error: #dc2626;
    --exito: #16a34a;
    --radio: 30px;
    --sombra: 0 4px 20px rgba(0,0,0,0.08);
    }
    ```
    - Cambie el `--primario: #2563eb` a `--primario: #3a4161`. Esto hizo que el **color primario de la pagina cambiara.**
    - Cambie el `--primario-oscuro: #1d4ed8` a `---primario-oscuro: #000630`. Esto hizo que el **color complementario de la pagina cambiara.**

6.  Otra cosa que se cambio fue:
    
    Que paso de:

    ```css
    .btn-primario {
    background: var(--primario);
    color: white;
    box-shadow: 0 2px 8px rgba(37, 99, 235, 0.3);
    }
    ```
    A esto:

    ```css
    .btn-primario {
    background: var(--primario);
    color: white;
    box-shadow: 10px 19px 10px rgba(136, 135, 155, 0.318);
    }
    ```

    - Cambie el `box-shadow` para que el boton tuviera una sombra **10px** más en **eje x**. De igual manera aumente el número de pixeles del **eje y**, pasando de **2px** a **19px**. Por último, aumente la **opacidad** de la sombra que paso de **8px** a **10px**.

    - Además cambie **el color de la sombra**, utlizando los **primeros tres digitos del rgba.** También le cambie la **intencidad a este color**, utilizando el **último digito del rgba**, la aumente.

    7. Por último cambie el hover del boton primario:

    Paso de esto:

    ```css
    .btn-primario:hover {
    background: var(--primario-oscuro);
    transform: translateY(-1px);
    box-shadow: 0 4px 12px rgba(37, 99, 235, 0.4);
    }
    ```

    A esto:

    ```css
    .btn-primario:hover {
    background: var(--primario-oscuro);
    transform: translateY(-2px);
    box-shadow: 10px 22px 5px rgba(214, 212,  218, 0.320);
    }
    ```

    - Cambie el `transform` para que el **boton se elevara otro pixel más**, pasando de **-1px** a **-2px**.

    - Cambie el `box-shadow` para que el boton tuviera una sombra **10px** más en **eje x**. De igual manera aumente el número de pixeles del **eje y**, pasando de **4px** a **22px**. Por último, aumente la **opacidad** de la sombra que paso de **12x** a **5px**.

    - Además cambie **el color de la sombra**, utlizando los **primeros tres digitos del rgba.** También le cambie la **intencidad a este color**, utilizando el **último digito del rgba**, la disminuí.
    


    
    



