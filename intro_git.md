⸻

Sesión 1: Introducción a Git

Objetivo

Que los participantes comprendan:
	•	Qué es Git y para qué se usa.
	•	Cómo funciona Git internamente (conceptos básicos).
	•	Los comandos principales para empezar a trabajar con Git.

⸻

1. ¿Qué es Git?

Definición básica:

Git es un sistema de control de versiones distribuido, gratuito y de código abierto, diseñado para manejar todo tipo de proyectos con rapidez y eficiencia.

¿Para qué sirve?
	•	Guardar cambios en el código o archivos.
	•	Volver a versiones anteriores.
	•	Trabajar en equipo sin sobrescribir el trabajo de otros.
	•	Rastrear la historia de los cambios.

Diferencia entre Git y GitHub:
	•	Git: herramienta local para control de versiones.
	•	GitHub: plataforma en la nube para alojar repositorios Git.

⸻

2. ¿Cómo funciona Git?

Snapshots, no diferencias

Git no guarda cambios como "deltas" (como otros sistemas), sino que guarda un "snapshot" del contenido cada vez que haces un commit.

Tres áreas principales:
	•	Working Directory (directorio de trabajo): donde editas tus archivos.
	•	Staging Area (índice): zona temporal donde seleccionas los cambios a guardar.
	•	Repositorio (commit): el historial de versiones confirmadas.

Diagrama simple:

[Working Directory] --> git add --> [Staging Area] --> git commit --> [Repository]


⸻

3. Primeros pasos: Instalación y configuración

git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"


⸻

4. Principales comandos

Inicializar un repositorio

git init

Ver el estado del repositorio

git status

Añadir archivos al staging

git add archivo.txt        # Archivo específico
git add .                  # Todos los archivos modificados

Hacer un commit

git commit -m "Mensaje descriptivo"

Ver el historial de cambios

git log

Crear una nueva rama

git branch nombre_rama

Cambiar de rama

git checkout nombre_rama

Fusionar ramas

git merge nombre_rama

Ver diferencias

git diff


⸻

5. Git remoto (breve mención)

Puedes conectar tu repositorio local con GitHub u otro servidor:

git remote add origin https://github.com/usuario/repositorio.git
git push -u origin main


⸻

6. Buenas prácticas iniciales
	•	Hacer commits con mensajes claros.
	•	No hacer git add . sin revisar qué estás agregando.
	•	Hacer commits pequeños y frecuentes.
	•	Usar ramas para trabajar en nuevas funcionalidades o correcciones.

⸻

7. Actividad práctica (opcional)
	1.	Crear una carpeta y un archivo.
	2.	Inicializar un repositorio Git.
	3.	Hacer cambios y registrar el historial.
	4.	(Si hay conexión a internet) Subirlo a GitHub.

⸻