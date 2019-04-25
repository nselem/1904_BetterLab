# Descubriendo tu información genética  
![BetterLab Logo](images/BetterLab.png)   

      
    
## Informacion General  
Bienvenido a aprender sobre tu información genética. Esta será la página web del taller, donde encontrarás el temario y los protocolos del curso. Además trabajaremos en un [documento colaborativo](https://etherpad.net/p/190419_BetterLab) donde podemos anotar dudas de los participantes y compartir información todos al mismo tiempo. Los documentos colaborativos ayudan a llevar un registro del trabajo comunitario  y te permiten ser una herrammienta de consulta en el futuro. Algunas de nuestras son parte del contenido habitual de [software carpentry](https://software-carpentry.org/) una organización dedicada a enseñar habilidades de cómuto para hacer más en menos tiempo y con menos sufrimiento, usaremos estas dos lecciones con su permiso. Las otras fueron pensadas de acuerdo a las necesidades específicas del taller.   

En este curso aprenderás un poco de biología tanto experimental como computacional. Adquirirás también nociones de marcadores y filogenias.   
  
## Calendario   
  
<table>
    <tr>
        <td></td>        <td>Sábado 27       </td> <td>           Domingo 28                 </td>
  </tr>  
      <tr><td>10:00 a 10:30</td>
      <td>  Introducción teórica a la Biología Molecular.   </td>  
      <td>  Introducción teórico-práctica a la reacción de PCR</td>
  </tr>
      <tr><td></td><td>Coffee Break</td><td>Coffee Break</td>
    
    <tr><td></td>
      <td>
        Sesión 5 (9:10 -12:10) Análisis de secuencias <a href="paginas/git/sesion3.md">Git </a> y <a href="https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf">Markdown</a>  </td></tr>  
    <tr><td></td><td>Sábado 4</td><td>Domingo 5 </td></tr>
    <tr><td></td>
          <td>
        Genómica y Bioinformática          </td>
      <td>Sesión 6 (12:50-3:50) <a href="paginas/genomica/genomica.md"> Arboles y metadatos</a></td>
    </tr>
    <tr><td>
    </td>
          <td> Sesión 1 (9:00 - 12:00 am) Introducción y <a href="https://swcarpentry.github.io/shell-novice-es/"> bash </a> 
        </td>    <td>Sesión 7 (4:00 -7:00 pm) Proyectos y exposición </td>
    </tr>
</table>  


## Temario detallado  
<table> 
<tr>
</tr>
</table>    
     
___         
## Entregables    
El objetivo del curso será que los alumnos tengan un panorama general de la Biología computacional, y que la vivan a través del desarrollo de sus primeros programas.   
1) Github con un script   25%  
2) Bacteria identificada   5%  
3) Exposición de Proyecto 70%  
  
___  
  
## Instalaciones y requerimientos previos  
<h2 id="setup">Setup</h2>  

<p>
  Para participar en este taller necesitas acceso al siguiente software. Además necesitarás acceso a un navegador como chrome o firefox.   
  </p>
<p>
  Aqui hay una referencia de posibles problemas durante la instalación.  
  <a href = "{{site.swc_github}}/workshop-template/wiki/Configuration-Problems-and-Solutions">Wiki de problemas de instalación y sus soluciones. </a>.
</p>

<div id="shell">  
  <h3>El Bash Shell</h3>  
  <p>  
    Bash es un intérprete de comandosque te da poder de hacer tareas simples rápidamente.  
  </p>  

  <div class="row">  
    <div class="col-md-4">  
      <h4 id="shell-windows">Windows</h4>  
      <a href="https://www.youtube.com/watch?v=339AEqk9c-8">Video Tutorial</a>  
      <ol>  
        <li>Baja para windows <a href="https://git-for-windows.github.io/">el instalador de git </a>.</li>  
        <li>Corre el instalador y sigue los siguientes pasos:  
          <ol>  
            <li>Click en "Next".</li>  
            <li>Click en "Next".</li>    
            <li>  
              <strong>  
               Manten el "Use Git from the Windows Command Prompt" seleccioinado y  click en "Next".  
              </strong>  
                Si se te olvida hacer esto algunos programas que necesitarás no funcionaran correctamente.  
                Si esto te pasa regrésate al paso anterior del instalador y selecciona la opción correcta.  
            </li>  
            <li>Click en "Next".</li>
            <li>  
              <strong>  
                Mantén "Checkout Windows-style, commit Unix-style line endings" seleccionado y click en "Next".
              </strong>
            </li>
            <li>  
              <strong>  
                Mantén "Use Windows' default console window" seleccionado y click en "Next".  
              </strong>  
            </li>  
            <li>Click en "Install".</li>
            <li>Click en "Finish".</li>  
          </ol>  
        </li>  
        <li>  
          si tu variable de ambiente "HOME" no está lista (o no sabes qué es esto):
          <ol>
            <li>Abre el prompt (Abre el menu start, escribe <code>cmd</code> y presiona enter [Enter])</li>
            <li>
              Escribe la siguiente línea en la ventana del promt exactamente como se  muestra:  
              <p><code>setx HOME "%USERPROFILE%"</code></p>  
            </li>  
            <li>Presiona [Enter], debes de ver <code>SUCCESS: Specified value was saved.</code></li>
            <li>Para salir del prompr escribe <code>exit</code> y presiona enter [Enter]</li>
          </ol>
        </li>
      </ol>
      <p>Esto te dará ambos Git y Bash en el programa Git Bash.</p>
    </div>
    <div class="col-md-4">
      <h4 id="shell-macosx">macOS</h4>
      <p>
        El shell por default en todas las versiones de macOS es Bash, asi que no debes instalar nada.  Podrás accesar a Bash desde la Terminal
        (que se encuentra en        <code>/Applications/Utilities</code>).
        Para la instalación de Git aqui tenemos un <a href="https://www.youtube.com/watch?v=9LQhwETCdwY ">video tutorial</a>
        for an example on how to open the Terminal.
        Tal vez quieras mantener la Terminal en tu dock para este taller.  
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="shell-linux">Linux</h4>
      <p>
        El shell es usualmente Bash, pero si tu máquina es diferente puedes abrir una terminal y escribir <code>bash</code>.  
        No se necesita intalar nada
      </p>
    </div>
  </div>
</div> 
