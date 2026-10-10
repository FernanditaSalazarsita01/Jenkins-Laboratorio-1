# Laboratorio 1 — Jenkins: Hola Mundo

## Objetivo
Crear un Pipeline básico en Jenkins que ejecute un mensaje en la consola y comprobar el resultado de la ejecución.

## Archivos
- `Jenkinsfile`: ejemplo de Pipeline declarativo para ejecutar en Jenkins.
- `Reporte_Jenkins_Corregido.docx`: reporte con explicación, capturas y resultados documentados.
- `evidencias/`: imágenes extraídas del reporte proporcionado.

## Requisitos
- Jenkins funcionando, con acceso a su interfaz web y permisos para crear trabajos.
- Un agente capaz de ejecutar Pipeline (por ejemplo, el agente integrado habilitado para la práctica).

## Ejecución en Jenkins
1. Abre Jenkins (por ejemplo, `http://localhost:8080` si está ejecutándose localmente).
2. Selecciona **Nueva tarea / New Item**.
3. Escribe `pipe-hola-mundo`, selecciona **Pipeline** y acepta.
4. En **Configurar → Pipeline**, selecciona **Pipeline script from SCM** si Jenkins puede acceder a este repositorio. Elige Git, pega la URL del repositorio, selecciona la rama y usa `Jenkinsfile` como Script Path. Alternativamente, elige **Pipeline script** y copia el contenido de `Jenkinsfile`.
5. Guarda y selecciona **Construir ahora / Build Now**.
6. Abre **Console Output** y verifica el mensaje `Hola Mundo desde Jenkins` y el resultado `Finished: SUCCESS`.
7. Si deseas evidenciar esta ejecución del código publicado, genera nuevas capturas mostrando el mensaje exacto y el resultado.

## Evidencias y alcance
Las capturas son las conservadas del documento original y muestran la interfaz de Jenkins, un trabajo `pipe-hola-mundo` y una ejecución con `Finished: SUCCESS`. **No demuestran que este Jenkinsfile específico haya sido el que se ejecutó**. El Jenkinsfile es un ejemplo reproducible que se debe probar para confirmar su funcionamiento.

El contenido fue preparado sobre la base del reporte proporcionado. No se pudo verificar el contenido interno de la carpeta `Lab 1` del repositorio de referencia: https://github.com/jorgealmeidamontiel/jenkins-laboratories/tree/main/Lab%201 . Compara con las instrucciones originales del docente antes de entregar.

## Historial Git
Al subir archivos mediante la interfaz web, GitHub puede registrar un único commit. Para cumplir el requisito de **historial de commits claro**, haz cambios reales y confirma cada uno con mensajes descriptivos (por ejemplo, `feat: agregar Jenkinsfile`, `docs: agregar instrucciones`, `docs: incorporar evidencias`). No se incluye un historial preconstruido ni se representan commits ficticios.
