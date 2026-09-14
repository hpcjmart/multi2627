---
layout: post
title: Guía de Estudio
---

# Multiprocesadores · Guía de Estudio
## Universidad de Almería (UAL) — Curso 2026/2027

---

## 1. Cronograma
El cronograma de la asignatura se encuentra en el Aula Virtual, dentro de: **Contenido ➔ Información General ➔ Planificación Multiprocesamiento 2026/2027**. Las aulas y los horarios oficiales de las clases presenciales están detallados en el Calendario del curso en el Aula Virtual y en la Página Web Oficial de la Asignatura.

### 🗓️ Planificación de semanas especiales:
Durante las semanas del **14 de septiembre**, **21 de septiembre** y **12 de octubre**, se aplicará el siguiente esquema:
* Se impartirá exclusivamente una sesión de teoría los **jueves** (Grupo Docente - GD).
* **No habrá sesiones de actividades** para ninguno de los grupos de trabajo (GT1, GT2 ni GT3).

---

## 2. Objetivos, Contenidos, Actividades y Materiales del Curso

| Módulos | Objetivos | Contenidos | Actividades | Materiales |
| :---: | :--- | :--- | :--- | :--- |
| **1** | Obtener los conocimientos básicos para realizar las actividades de los siguientes módulos. | • Introducción a HPC<br>• Introducción a Linux<br>• Introducción a C | • Bandera serie<br>• Mandel serie<br>• Wa-tor serie | **Se usará:**<br>• Compilador `gcc`<br>• PC del Lab. 2.02 o PC personal con Linux. |
| **2** | Obtener programas paralelos eficientes en sistemas de memoria compartida: OMP y PThreads. | • Introducción: OMP y Pthreads | • Bandera-OMP / PTh<br>• Mandel-OMP / PTh<br>• Wa-tor-OMP / PTh | **Se usará:**<br>• Compilador `gcc`<br>• PC del Lab. 2.02 o PC personal con Linux. |
| **3** | Obtener programas paralelos eficientes en sistemas de memoria distribuida: MPI. | • Introducción a MPI | • Cluster-MPI<br>• Bandera-MPI<br>• Mandel-MPI | **Se usará:**<br>• Compilador `gcc` y `mpicc`<br>• PC del Lab. 2.02 o PC personal con Linux. |

### 🏫 Dinámica de las Sesiones Presenciales
Los objetivos de la Guía Docente Oficial se desarrollarán mediante clases presenciales de teoría en el grupo docente **GD**, y de actividades en los grupos de trabajo **GT1, GT2 y GT3**.

* **Sesiones de Teoría:** El alumno debe trabajar los contenidos correspondientes antes de la sesión. En la clase presencial se realizará un resumen del contenido asignado y se resolverán dudas.
* **Sesiones de Actividades:** El alumno debe preparar las actividades antes de la clase presencial. La sesión en el aula se utilizará exclusivamente para resolver los problemas surgidos. 
  * Se realizarán siempre en el **Lab. 2.02 del CITE III** (se necesita un ordenador con Linux).
  * Los alumnos se asignan a cada grupo (GT1, GT2, GT3) por orden alfabético en la ESI. Estos grupos están configurados de forma "personalizada" (no son de inscripción por cuenta propia).
  * **Requisitos para cambios de grupo:** Presentar una razón ineludible al profesor, que exista plaza libre (límite de **24 PCs** en el laboratorio), o intercambiarse directamente con otro alumno del grupo destino.
  * Los exámenes parciales se realizarán en el mismo Lab. 2.02 respetando los horarios de cada grupo.

---

## 3. Contenidos y Materiales del Curso
Cada módulo consta de de los siguientes elementos:
1. Contenidos de teoría, material complementario e información adicional.
2. Actividades.
3. Un ejemplo de pre-examen.

> 📂 **Información Adicional de Utilidad:** En el Módulo 1 (carpeta `Intro Linux`) se encuentra el documento *"Instalar Linux"* con enlaces explicativos. En la carpeta `Intro C` dispones del documento *"Man pages, debugging, profiling, memory leaks"*, con comandos útiles para obtener información de funciones, depurar, medir rendimiento y detectar pérdidas de memoria en C.
>
> 🧪 **Ejemplo de Pre-examen:** No cuenta para la calificación final; es una "herramienta de entrenamiento" para la autoevaluación. Se compone de un pre-examen teórico de opción múltiple y uno de programación (este último incluye la solución explicada en teoría). Se recomienda resolverlo por cuenta propia antes de ver la explicación presencial.

---

## 4. Detalle de las Actividades Prácticas
Las actividades principales se basan en el desarrollo de tres programas específicos:

* **Bandera:** Generar la bandera de España. Permite experimentar con una distribución estática de datos para su cómputo entre las unidades de procesamiento.
* **Mandel:** Generar la imagen de Mandelbrot. Al tener una carga computacional desigual por unidad de proceso, la distribución estática es ineficiente; requiere aplicar mecanismos de **balanceo dinámico de carga**.
* **Wa-tor:** Simulador de red trófica con peces y tiburones. Presenta dependencia de datos y requiere evitar situaciones de conflicto (por ejemplo, que dos tiburones intenten comerse al mismo pez de forma simultánea).

### 🛠️ Versiones y Entornos:
* Se realizarán versiones en **Secuencial**, en memoria compartida (**OpenMP y Pthreads**) y en memoria distribuida (**MPI**).
* *Excepción:* La actividad **Wa-tor no se realizará en MPI**. Se reemplaza por la práctica **"MPI Cluster"**, donde se configurarán dos ordenadores para ejecutar un programa MPI en paralelo compartiendo la carga.

### 👥 Normas de Inscripción y Entrega:
* Las instrucciones detalladas de cada práctica están en el archivo `README.md` de su carpeta. Además, el archivo `AnswerToStudents.md` recopila las respuestas comunes a los problemas detectados en las entregas de años anteriores.
* Se trabaja en grupos de **1, 2 o 3 estudiantes**. Es obligatorio inscribirse en la pestaña "Grupos" del menú superior del Aula Virtual; si no estás inscrito, las actividades no serán visibles.
* **Formato de entrega:** Se debe adjuntar un archivo comprimido mediante el icono del clip.
* **Intentos y Penalizaciones:** Se disponen de **dos intentos** por actividad (las entregas tardías reducen la calificación). Se abrirá un intento nuevo para el examen final y otro adicional para el extraordinario.
* ⚠️ **Importante sobre la Retroalimentación:** **Solamente el primer intento recibirá comentarios y feedback a tiempo antes de su correspondiente examen**. El resto de intentos se enfocan exclusivamente en poder aprobar la asignatura o subir nota.

---

## 5. Detalle del Sistema de Evaluación
Para superar la asignatura es obligatorio **aprobar de forma independiente las tres partes**: actividades, teoría y programación.

### 📊 Porcentajes de Puntuación
* **Actividades:** 20%.
* **Teoría:** 30%.
* **Programación:** 50%.

### 📝 Exámenes Parciales
Se realizarán dos exámenes parciales de dos horas de duración en el Lab. 2.02 del CITE III:
1. **Examen Parcial del Módulo 2:**
   * **Teoría:** Examen de opción múltiple con contenidos de los módulos 1 y 2.
   * **Programación:** Centrado en las librerías OpenMP y PThread.
2. **Examen Parcial del Módulo 3:**
   * **Teoría:** Examen de opción múltiple con contenidos del módulo 3.
   * **Programación:** Centrado en la librería MPI.

### 🔄 Convocatorias Finales
* Si se suspende cualquier bloque en los parciales, se debe realizar el examen final. Si se suspende el final, se deberá superar el examen extraordinario.
* La entrega y corrección de cualquier actividad o examen calificará automáticamente al alumno como **"Presentado"** en la convocatoria.
* Los exámenes Final y Extraordinario consistirán en un test de opción múltiple para toda la teoría y un examen práctico de programación de las librerías PThreads y MPI (es obligatorio aprobar ambas partes de programación por separado).
* *Nota de acceso:* Los exámenes están en la carpeta "Exámenes" dentro de "Contenido", pero **no podrás visualizar esta carpeta hasta que realices el primer examen**.

> 🚨 **Política contra el Plagio:** Cualquier intento de copia o suplantación resultará en que se correrá la convocatoria. Si ocurre en un examen parcial, el alumno perderá el derecho a presentarse al examen final ordinario. (Ver *Acta de Copia en Examen*).

---

## 6. Estructura del Curso en el Aula Virtual
La interfaz de la plataforma en línea consta de los siguientes apartados principales:

* **Contenido:** Da acceso a *Información General* (guía y cronograma), *Contexto* (motivación del alumnado), *Módulos* (teoría, prácticas y pre-exámenes) y *Exámenes*.
* **Calendario:** Muestra horarios, aulas asignadas y fechas de evaluaciones.
* **Anuncios e Hilos:** Espacio para comunicados institucionales y debates (estos últimos inactivos por defecto).
* **Libro de calificaciones (GradeBook):** Permite ver los elementos calificables, las notas obtenidas, seleccionar el intento enviado y desplegar los comentarios o la rúbrica del docente.
* **Mensajes:** Canal prioritario para contactar con los profesores. **Se debe evitar el uso del correo institucional de los docentes**, ya que se encuentra saturado.
* **Grupos y Logros:** Gestión de los equipos de trabajo (los "Logros" no se utilizan en este curso).

### 👨‍🏫 Profesores del curso
* **José Antonio Martínez**
* **Francisco José Orts Gómez** (Grupo de Trabajo)

*(Las sesiones de teoría se grabarán mediante Class Collaborate siempre que la infraestructura técnica del aula lo permita y no existan fallos informáticos).*

---

## 7. Normas de Comunicación y Consejos de Éxito

### 💬 Uso de las Herramientas de Comunicación (Netiqueta)
* Sé cortés y evita expresiones demasiado coloquiales que puedan ser malinterpretadas.
* Trata a todos los miembros de la comunidad académica con respeto.
* Línea de Asunto: Utilízala correctamente reduciendo el tema a 2 o 3 palabras descriptivas. No incluyas textos largos ni uses términos alarmistas como "¡Urgente!" o "Caos".
* Contextualiza siempre tu situación y el motivo del mensaje, aunque esté relacionado con conversaciones anteriores.
* No escribas textos en mayúsculas, ya que en la comunicación digital equivale a gritar y resulta incómodo de leer.
* Emplea emoticonos [:-)] para transmitir emociones correctamente y evitar malas interpretaciones ante comentarios irónicos o toques de humor.

### 💡 Recomendaciones del Equipo Docente
* Sigue el orden modular: Completa las prácticas de un módulo y realiza su pre-examen correspondiente antes de pasar al siguiente bloque temático.
* Constancia: La asignatura exige una dedicación semanal continua y planificada.
* Asistencia a clase: Aunque no es obligatoria, las estadísticas de años anteriores confirman que un alto porcentaje de los alumnos asistentes aprueban, mientras que una gran parte de los no asistentes suspenden.
* Aprovecha los parciales: Aunque suspendas el primer parcial, preséntate al segundo. Los comentarios de las calificaciones te servirán como herramienta de aprendizaje para el examen final.
* Estudio individual del código: Aunque las actividades se entreguen en grupo, cada estudiante debe comprender el código al 100% de cara a superar la parte de programación de los exámenes, que es estrictamente individual.
 
