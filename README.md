# Universidad [Universidad Tecnica de Ambato]  
## Facultad de [ INGENIERÍA EN SISTEMAS, ELECTRÓNICA E INDUSTRIAL]  
### Carrera de Ingeniería en Software  

**Asignatura:** Manejo y Configuración de Software  
**Nombre del Estudiante:** Washington Villalba  
**Fecha:** 07 / 10 / 2025 

---

# Evaluación Práctica de Git y GitHub

## Instrucciones Generales

- Cada pregunta debe ser respondida directamente en este archivo **(README.md)** debajo del enunciado correspondiente.
- Cada respuesta debe ir acompañada de uno o más **commits**, según se indique en cada pregunta.
- Cuando se indique, deberán realizarse acciones prácticas dentro del repositorio (como creación de archivos, ramas, resolución de conflictos, etc.).
- Cada pregunta debe estar **etiquetada con un tag**, únicamente en el commit final correspondiente, con el formato: `"Pregunta 1"`, `"Pregunta 2"`, etc.

---

## Pregunta 1 (1 punto)

**Explicar la diferencia entre los siguientes conceptos/comandos en Git y GitHub:**

- `git clone`  
- `fork`  
- `git pull`

### Parte práctica:

- Realizar un **fork** de este repositorio en la cuenta personal de GitHub del estudiante.
- Luego, realizar un **clone** del fork en el equipo local.
- En este README, describir el proceso seguido:

  - ¿Cómo se realizó el fork?
 
  - ¿Cómo se realizó el clone del fork?
   

  - ¿Cómo se verificó que se estaba trabajando sobre el fork y no sobre el repositorio original?

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta a la Pregunta 1 -->

---
  - `git clone` : Es un comando de Git que se ejecuta en la terminal local. Su función es descargar una copia exacta de un repositorio remoto (ya sea el original o un fork) a tu máquina. Este proceso crea un directorio con todos los archivos, el historial de commits y las ramas del proyecto, y configura automáticamente una conexión remota llamada origin que apunta al repositorio desde el cual se clonó.

 - `fork`  : Es una acción que se realiza en la plataforma de GitHub (no es un comando de Git). Consiste en crear una copia personal y completa de un repositorio ajeno en tu propia cuenta de GitHub. Este "fork" se convierte en un repositorio independiente sobre el cual tienes derechos de escritura, permitiéndote experimentar y proponer cambios sin afectar el proyecto original. Es el primer paso para contribuir a un proyecto de código abierto.

- `git pull` Es un comando de Git que se utiliza para actualizar tu repositorio local con los cambios existentes en el repositorio remoto. Es una combinación de dos comandos: git fetch (que descarga los cambios desde el remoto pero no los integra) y git merge (que fusiona dichos cambios en tu rama local).


  - ¿Cómo se realizó el fork?
    Se realizó mediante el siguiente link https://github.com/santiagojara/EVALUACION_1P en el cual se presionó el botón "Fork" y se seleccionó la cuenta personal del estudiante.

  - ¿Cómo se realizó el clone del fork?

    En la página de su repositorio (su fork) se copió la URL de clonación y se ejecutó en la terminal local, por ejemplo:

    git clone https://github.com/<TU_USUARIO>/EVALUACION_1P.git

  - ¿Cómo se verificó que se estaba trabajando sobre el fork y no sobre el repositorio original?

    Se verificó de forma local y en GitHub usando las siguientes comprobaciones y comandos:

    1) En GitHub (interfaz web):
       - En la página de su repositorio fork aparece la etiqueta "forked from santiagojara/EVALUACION_1P" debajo del nombre del repositorio. Esa etiqueta confirma que es un fork del repositorio original.

    2) En la máquina local (terminal):
       - Comprobar la URL del remoto "origin" con cualquiera de estos comandos:

         git remote -v
         git remote show origin
         git branch -vv

       - En la salida de "git remote -v" debe verse algo como:

         origin  https://github.com/<TU_USUARIO>/EVALUACION_1P.git (fetch)
         origin  https://github.com/<TU_USUARIO>/EVALUACION_1P.git (push)

       Si en lugar de su usuario aparece "https://github.com/santiagojara/EVALUACION_1P.git" entonces clonó el repositorio original y no su fork.

    3) Comprobación adicional (recomendado): añadir un remoto llamado "upstream" apuntando al repositorio original para distinguir claramente los remotos:

       git remote add upstream https://github.com/santiagojara/EVALUACION_1P.git
       git remote -v

       Tras esto verá ambos remotos: "origin" (su fork) y "upstream" (repositorio original). Esto facilita traer cambios del original sin confundir los remotos.

    Resumen: la verificación principal es inspeccionar la URL del remoto "origin" con "git remote -v" y comprobar la etiqueta "forked from" en la interfaz web de GitHub. Si origin apunta a su cuenta, está trabajando sobre el fork.


## Pregunta 2 (1 punto)

**Configurar un archivo `.gitignore` para que ignore:**

- Todos los archivos con extensión `.log`.
- Una carpeta llamada `temp/`.
- Todos los archivos `.md` y `.txt`de la carpeta `doc/`. (Probar agregando un archivo `prueba.md` y un archivo `prueba.txt` dentro de la carpeta y fuera de la carpeta.)

### Requisitos:

1. Realizar un **primer commit** que incluya únicamente el archivo `.gitignore` con las reglas de exclusión definidas.
2. Realizar un **segundo commit** donde se explique en este README la función del archivo `.gitignore` y se muestre evidencia de que los archivos y carpetas indicadas no están siendo rastreadas por Git.

**Importante:**  
- Solo el **segundo commit** debe llevar el **tag `"Pregunta 2"`**.

**📝 Respuesta:**

<!-- Escribe aquí tu explicación y evidencia para la Pregunta 2 -->

---

## Pregunta 3 (2 puntos)

**Utilizar Git Flow para desarrollar una nueva funcionalidad llamada `ingresar-encabezado`.**

### Requisitos:

- Inicializar el repositorio con Git Flow, utilizando las ramas por defecto: `main` y `develop`.
- Crear una rama de tipo `hotfix` con el nombre `ingresar-encabezado`.
- En dicha rama, **completar con los datos personales del estudiante** el encabezado que ya se encuentra al inicio de este archivo `README.md`.
- Realizar al menos un commit durante el desarrollo.
- Finalizar el hotfix siguiendo el flujo de trabajo establecido por Git Flow.

### En este README, se debe incluir:

- Los **comandos exactos** utilizados desde la inicialización de Git Flow hasta el cierre del hotfix.
- Una descripción del **proceso seguido**, indicando el propósito de cada paso.
- Una reflexión sobre las **ventajas de aplicar Git Flow**, especialmente en contextos colaborativos o proyectos de larga duración.

**Importante:**

- Deben realizarse varios commits durante esta pregunta.
- **Solo el commit final** debe llevar el **tag `"Pregunta 3"`**.
- El flujo debe respetar la estructura de Git Flow con las ramas `develop` y `main`.

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta completa a la Pregunta 3 -->

---

## Pregunta 4 (2 puntos)

**Trabajo con Issues y Pull Requests**

### Parte teórica:

- Explicar qué es un **issue** en GitHub.
- Explicar qué es un **pull request** y cuál es su finalidad.
- Indicar la diferencia entre ambos y cómo se relacionan en un entorno de trabajo colaborativo.

### Parte práctica:

- Trabajar en la rama `develop`, ya existente desde la configuración de Git Flow.
- Crear un **issue** titulado `"Respuesta a la Pregunta 4"`, en el que se indique que su objetivo es documentar esta pregunta.
- Realizar los cambios necesarios en este archivo `README.md` para responder esta pregunta.
- Realizar un **commit** con los cambios y subirlo a la rama `develop` del repositorio remoto.
- Crear un **pull request** desde `develop` hacia `main` en GitHub.
- **Vincular el pull request con el issue creado**, de manera que al ser aprobado y fusionado, el issue se cierre automáticamente.
- **Aprobar** el pull request para que se haga el merge respectivo hacia `main`.

### En este README, se debe incluir:

- Un resumen del procedimiento realizado.
- El número y enlace del issue creado.
- El número y enlace al pull request.

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta completa a la Pregunta 4 -->

---

## Pregunta 5 (2 puntos)

**Resolver conflictos entre ramas y realizar un Pull Request**

### Requisitos:

- Crear dos ramas llamadas `ramaA` y `ramaB`, ambas a partir de la rama `develop`.
- En `ramaA`, crear un archivo llamado `archivoA.txt` con el contenido:  
  `Contenido A`
- En `ramaB`, crear un archivo con el mismo nombre (`archivoA.txt`), pero con el contenido:  
  `Contenido B`
- Intentar fusionar `ramaB` sobre `ramaA`, lo cual debe generar un conflicto.
- Resolver el conflicto combinando ambos contenidos.
- Realizar el merge de `ramaA` hacia `develop`.
- Crear un **pull request** desde `develop` hacia `main`.
- Una vez completado lo anterior, eliminar las ramas `ramaA` y `ramaB` tanto local como remotamente.

### En este README, se debe incluir:

- El procedimiento completo:
  - Cómo se crearon las ramas.
  - Cómo se generó y resolvió el conflicto.
  - Cómo se realizó el merge hacia `develop`.
  - Cómo se eliminaron las ramas al finalizar.
- El enlace al pull request.
- Una breve explicación de qué es un conflicto en Git y por qué ocurrió en este caso.

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta completa a la Pregunta 5 -->

---

## Pregunta 6 (2 puntos)

**Realizar limpieza, explicar versionamiento semántico y enviar cambios al repositorio original**

### Requisitos:

- Trabajar en la rama `develop` del fork del repositorio.
- Eliminar los archivos `archivoA.txt` y `archivoB.txt` creados en preguntas anteriores.
- Realizar un merge desde `develop` hacia `main` en el repositorio local.
- Enviar los cambios de la rama `main` local a la rama `develop` del repositorio remoto (fork). Recuerde incluir todos los tags creados (6 tags).
- Finalmente, crear un **pull request** desde la rama `develop` del fork hacia la rama `main` del repositorio original (del cual se realizó el fork en la Pregunta 1). El titulo del pull request debe ser "NOMBRE APELLIDOS", en la descripción colocar el link de su repositorio de GitHub.

### En este README, se debe incluir:

- Una explicación del proceso realizado paso a paso.
- Una explicación del **versionamiento semántico**, indicando:
  - En qué consiste.
  - Sus tres componentes (MAJOR, MINOR, PATCH).
- El enlace al pull request creado hacia el repositorio original.
- Si hace falta agregar alguna evidencia adicional, agregue un tag adicional que sea `Version Final`.

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta completa a la Pregunta 6 -->
