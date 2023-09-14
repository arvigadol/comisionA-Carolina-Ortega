<h1 align="center"> EPICA - Argentina Programa 4.0 </h1>
<h2 align="center"> comision-A-Carolina-Ortega </h2>


<p align="center">
<img src="https://img.shields.io/badge/STATUS-EN%20DESAROLLO-green">
</p>

<h2 align="left">Breve descripción del proyecto</h2>

# Este es el trabajo final del Tramo 2. Nos pidieron realizar un foro personalizado en el que el usuario pueda escribir y presentar sus publicaciones de manera atractiva. Para ello, se desarrolló una página en la que, mediante un botón, aparece un formulario para realizar una publicación. Al agregar una entrada, en el main de la página, van sumándose las publicaciones, ordenadas según la fecha de creación.

<h2 align="left">Instrucciones para ejecutarlo localmente</h2>
<p>
    Para visualizar correctamente la página, deberían seguirse estos pasos:  
</p>
<ol>
    <li>Clonar el proyecto mediante esta URL: https://github.com/arvigadol/comisionA-Carolina-Ortega.git o bien, descargar el archivo zip que allí se encuentra disponible.</li>
    <li>2Abrir la carpeta principal del proyecto con un Visual Studio Code</li>
    <li>Abrir una terminal e instalar todas las librerías indicadas en el archivo package.json, incluyendo nodemon como dependencia de desarrollo</li>
    <li>Descargar Xampp, instalarlo, abrirlo y clickear sobre Start en los módulos Apache y MySQL</li>
    <li>En el editor, navegar hasta la carpeta server mediante el comando $ cd server. Luego tipear: $ npm run dev</li>
    <li>Si todo salió bien, se debería poder acceder al proyecto en: http://localhost:3000/posteos</li>
</ol>

Dudas y problemas encontrados:

-Estructura: no entiendo como renderizar otras secciones desde el servidor, por ejemplo, Sobre Mi. Pude agregarla con HTML en public, pero quería ponerla como una vista, intenté agregar una ruta y un controlador y hacerlo en ejs, pero no me salió.

-HTML: 1- No sé cómo cambiar que la card pueda soportar más contenido. Me deja poner muy poquito texto. Agregué incluso un scroll con css, pero no se copia el texto en la card, en el text-area del modal no hay ningún problema, puedo poner un texto largo, pero se pegan sólo las primeras frases al article.

-CSS: 1- el archivo reset no está teniendo efecto. Puse el link a bootstrap antes del style.css para que la cascada haga que quede el estilo en el último archivo. Puse *{margin:0px; padding:0px;} tanto en el reset como en, por ejemplo, body.css o card.css y sólo tuvo efecto cuando puse esas propiedades dentro de la clase que estaba modificando.
2- Como hacer para que el footer esté abajo incluso aunque aún no haya ninguna publicación. Luego, cuando se agregue publicaciones, que vaya bajando debajo de cada publicación.

-Git y Git-Hub: 1- me parece que hay más ramas de las que debería, una puede que la haya creado por error (-origin), las otras no entiendo que pasó. No debería estar todo en -main?
2- Tuve algunos problemas con los pusheos a github, aparece un commit con un merge que no sé cómo pasó, y aparece una rama que creo que creé por error, por eso me parece que los commits figuran desordenados.


Nota 1: me apareció demasiadas veces el error puerto YYYY ocupado. Solución: abrir el cmd como administrador y tipear: netstat -nao|findstr 0.0:YYYY (nos mostrará el PID XXXX; |=alt124) -> taskkill /pid XXXX /f = Correcto, se terminó el proceso con PID XXXX


Nota 2: Dejo 3 URL a mano para las imágenes:

https://thumbs.dreamstime.com/b/paisajes-de-yosemite-46208063.jpg

https://img.freepik.com/foto-gratis/paisaje-niebla-matutina-montanas-globos-aerostaticos-al-amanecer_335224-794.jpg

https://images.unsplash.com/photo-1494500764479-0c8f2919a3d8?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxleHBsb3JlLWZlZWR8Mnx8fGVufDB8fHx8fA%3D%3D&w=1000&q=80

