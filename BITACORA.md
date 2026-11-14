# Bitácora de trabajo — TA-IND-01

**Actividad:** Análisis crítico de etcd y comparación con Apache ZooKeeper  
**Asignatura:** Aplicaciones Distribuidas  
**Unidad:** 1  
**Modalidad:** Individual

---

## Sesión 1 — Jueves 12 de noviembre de 2026

**Horario aproximado:** 20:00 – 01:00 del viernes 13 de noviembre (5 horas).

### Actividades realizadas

- Creación del repositorio público `TA-IND-01-etcd-zookeeper` en GitHub.
- Organización de la estructura inicial del proyecto.
- Creación de las carpetas `anexos`, `evidencias`, `experimentos`, `figuras` y `secciones`.
- Preparación del documento principal `main.tex`.
- Creación del archivo `referencias.bib`.
- Configuración inicial de LaTeX y Biber.
- Preparación del archivo `.gitignore`.

### Problemas encontrados

Se presentaron dificultades iniciales para organizar los archivos y preparar el entorno de trabajo.

### Soluciones aplicadas

Se organizaron los directorios del repositorio y se prepararon los archivos necesarios para comenzar el desarrollo del informe.

---

## Sesión 2 — Viernes 13 de noviembre de 2026

**Horario aproximado:** 20:00 – 00:30 del sábado 14 de noviembre (4 horas y 30 minutos).

### Actividades realizadas

- Instalación y comprobación de Docker Desktop y Docker Compose.
- Configuración del archivo `docker-compose.yml`.
- Creación de un clúster de tres nodos de etcd versión 3.7.3.
- Comprobación de la salud de los nodos y del consenso Raft.
- Pruebas de escritura y lectura de datos entre los nodos.
- Simulación de la caída del nodo `etcd3`.
- Comprobación del funcionamiento del clúster con dos nodos activos.
- Pruebas de escritura y lectura durante la caída de un miembro.
- Revisión de los registros del contenedor para diagnosticar problemas durante la recuperación.
- Organización de las capturas de pantalla como evidencias experimentales.
- Registro de los avances mediante commits en GitHub.

### Problemas encontrados

Durante las pruebas de tolerancia a fallos, el nodo `etcd3` presentó dificultades para reincorporarse al clúster después de haber sido detenido.

### Soluciones aplicadas

Se revisaron los registros del contenedor mediante Docker, se inició nuevamente el nodo y se comprobaron los endpoints, el estado de los miembros y la disponibilidad de los datos.

---

## Sesión 3 — Sábado 14 de noviembre de 2026

**Horario aproximado:** Desde las 10:00. Sesión en desarrollo.

### Actividades realizadas

- Comprobación de la recuperación del nodo `etcd3`.
- Verificación de la salud de los tres miembros del clúster.
- Comprobación de la disponibilidad de los datos después de la recuperación.
- Organización y revisión de las evidencias experimentales.
- Actualización del repositorio mediante commits.
- Revisión de la consigna y de los criterios de evaluación de la actividad.
- Inspección de la estructura del repositorio y del historial de cambios.
- Revisión de los archivos `main.tex`, `referencias.bib` y `README.md`.
- Verificación de la codificación UTF-8 de los archivos.
- Identificación de las secciones y evidencias que todavía deben desarrollarse.
- Preparación de la bitácora de trabajo.

### Problemas encontrados

Se identificó que el informe académico todavía contiene una estructura inicial sin desarrollar y que el archivo de referencias bibliográficas aún no contiene las fuentes definitivas.

### Soluciones aplicadas

Se revisó el contenido de los archivos existentes y se estableció un orden de trabajo para completar las referencias académicas, los diagramas, el análisis comparativo y las demás secciones del informe.

### Estado de la sesión

Trabajo en desarrollo.

---

## Observaciones generales

El proyecto se desarrolla progresivamente mediante experimentación con Docker, documentación de resultados y análisis de los sistemas distribuidos seleccionados.

Las evidencias se almacenan en el repositorio para respaldar las pruebas realizadas y facilitar la revisión del trabajo.