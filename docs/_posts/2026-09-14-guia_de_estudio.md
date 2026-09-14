---
layout: post
title: Guía de Estudio
---

# Multiprocesadores · Grado en Ingeniería Informática
## Universidad de Almería (UAL) — Guía de Estudio

<p align="center">
  <img src="https://ual.es" alt="Logo Universidad de Almería" width="250">
</p>

---

## 1. Cronograma
El cronograma detallado de la asignatura se encuentra en el Aula Virtual, siguiendo la ruta: **Contenido ➔ Información General ➔ CronogramaEstudioMP**. Las aulas y los horarios oficiales de las clases presenciales están publicados en el Calendario del Aula Virtual y en la Página Web Oficial de la Asignatura.

### 🗓️ Excepciones en el calendario de clases:
Durante las semanas del **10 de septiembre**, **17 de septiembre** y **08 de octubre**, se aplicará la siguiente planificación:
* Se impartirá exclusivamente una sesión de teoría los martes (Grupo Docente - GD).
* **No habrá sesiones de actividades** para ninguno de los grupos de trabajo (GT1, GT2 ni GT3).

---

## 2. Objetivos, Contenidos, Actividades y Materiales del Curso

| Módulo | Objetivos | Contenidos | Actividades | Materiales Utilizados |
| :---: | :--- | :--- | :--- | :--- |
| **1** | Obtener los conocimientos básicos para realizar las actividades de los siguientes módulos. | • Introducción a HPC<br>• Introducción a Linux<br>• Introducción a C | • Bandera serie<br>• Mandel serie<br>• Wa-tor serie | • Compilador `gcc`<br>• PC del Laboratorio 2.02 o PC personal con Linux. |
| **2** | Obtener programas paralelos eficientes en sistemas de memoria compartida: OMP y PThreads. | • Introducción a OMP y Pthreads | • Bandera-OMP / PTh<br>• Mandel-OMP / PTh<br>• Wa-tor-OMP / PTh | • Compilador `gcc`<br>• PC del Laboratorio 2.02 o PC personal con Linux. |
| **3** | Obtener programas paralelos eficientes en sistemas de memoria distribuida: MPI. | • Introducción a MPI | • Cluster-MPI<br>• Bandera-MPI<br>• Mandel-MPI | • Compilador `gcc` y `mpicc`<br>• PC del Laboratorio 2.02 o PC personal con Linux. |

### 🏫 Dinámica de las Sesiones Presenciales
Los objetivos de la Guía Docente Oficial se desarrollan mediante dos tipos de clases:

* **Sesiones de Teoría (Grupos GDA y GDB):** El alumno debe estudiar los contenidos asignados **antes de acudir a la sesión**. En clase se realizará un resumen de los conceptos y se resolverán dudas colectivas.
* **Sesiones de Actividades (Grupos GT1, GT2 y GT3):** El alumno debe trabajar en los problemas previamente de forma autónoma. La clase presencial se usará exclusivamente para resolver los bloqueos o problemas surgidos. 
  * Se imparten siempre en el **Laboratorio 2.02 del CITE III** (requiere entorno Linux).
  * La asignación de grupos (GT1, GT2, GT3) se realiza por orden alfabético desde la ESI. Los cambios de grupo son excepcionales, no son de inscripción libre y requieren justificación ineludible al profesor, además de la existencia de plazas libres (el laboratorio cuenta con un límite estricto de **24 PCs**) o un intercambio con otro estudiante.
  * Los exámenes parciales se realizarán en este mismo laboratorio respetando los turnos de cada grupo de trabajo.

---

## 3. Estructura y Componentes de cada Módulo
Cada módulo del curso está compuesto de manera homogénea por los siguientes elementos:
1. **Contenidos de teoría,** material complementario e información adicional.
2. **Actividades prácticas**.
3. **Un ejemplo de pre-examen**.

> 📝 **Nota sobre la Información Adicional:** En el Módulo 1 se incluye una carpeta llamada `Intro Linux` con una guía para instalar la distribución de Linux recomendada. En la carpeta `Intro C` dispones del documento *"Man pages, debugging, profiling, memory leaks"*, fundamental para aprender comandos de depuración, análisis de rendimiento y detección de fugas de memoria en C.
>
> 🧪 **Nota sobre el Pre-examen:** Es una herramienta puramente formativa de autoevaluación que **no computa en la nota final**. Para visualizar el tipo test es obligatorio estar dado de alta en los grupos GTA. En la parte de programación se adjunta la solución explicada en teoría, pero se recomienda encarecidamente intentar resolverlo de manera individual antes de ver las respuestas.

---

## 4. Detalle de las Actividades Prácticas
El núcleo práctico de la asignatura gira en torno al desarrollo y optimización de tres programas específicos estructurados bajo diferentes paradigmas de computación:

* **Bandera:** Consiste en generar la bandera de España. Sirve para comprender y aplicar una distribución estática de datos básica entre las unidades de procesamiento.
* **Mandel:** Consiste en generar el fractal de Mandelbrot. Dado que la carga de cálculo de cada punto de la imagen varía drásticamente, la distribución estática es ineficiente. Requiere implementar mecanismos de **balanceo dinámico de carga** para mejorar la eficiencia paralela.
* **Wa-tor:** Simulador de una red trófica compleja con peces y tiburones. Requiere balanceo dinámico y presenta **dependencia de datos** crítica que debe controlarse (por ejemplo, evitar conflictos donde dos tiburones intenten devorar al mismo pez simultáneamente).

### 🛠️ Paradigmas de desarrollo por programa:
* Se desarrollarán versiones en **Serie**, en memoria compartida (**OpenMP y Pthreads**) y en memoria distribuida (**MPI**).
* *Excepción:* El programa **Wa-tor no se implementará en MPI**. En su lugar, en el Módulo 3 se realiza la práctica *"Clúster MPI"*, dedicada a aprender a configurar dos PCs físicos para ejecutar código paralelo de manera conjunta.

### 👥 Normas de Entrega de Prácticas:
* Las instrucciones y enunciados detallados de cada práctica se encuentran siempre en un archivo llamado `README.md` dentro de su respectiva carpeta.
* Se realizan en **grupos de 1, 2 o 3 alumnos**. Es obligatorio inscribirse formalmente en la pestaña "Grupos" del menú superior del Aula Virtual; de lo contrario, las actividades permanecerán ocultas.
* **Formato de entrega:** Se subirá un archivo comprimido adjunto (usando el icono del clip). Además, se debe indicar explícitamente en el cuadro de texto a qué grupo de trabajo (**GT1, GT2 o GT3**) pertenece la mayoría de los integrantes para asegurar que lo corrija el profesor correspondiente en el laboratorio.
* Cada actividad permite un **máximo de 2 intentos**. Las entregas fuera de plazo sufrirán una penalización en la nota. Las calificaciones y rúbricas detalladas se consultan desde el *Libro de calificaciones*.

---

## 5. Sistema de Evaluación Completo

Para superar la asignatura es requisito indispensable **aprobar de forma independiente cada una de las tres partes** (Actividades, Teoría y Programación). 

### 📊 Porcentajes de Calificación
* **Actividades Prácticas:** 20% de la nota final.
* **Teoría:** 30% de la nota final.
* **Programación:** 50% de la nota final.

### 📝 Estructura de Exámenes Parciales
Se realizarán dos evaluaciones parciales presenciales de 2 horas de duración en el Laboratorio 2.02:

1. **Examen Parcial del Módulo 2:**
   * **Teoría:** Contenidos de los Módulos 1 y 2.
   * **Programación:** Desarrollo de código en OpenMP y PThreads.
2. **Examen Parcial del Módulo 3:**
   * **Teoría:** Contenidos específicos del Módulo 3.
   * **Programación:** Desarrollo de código en MPI.

### 🔄 Evaluaciones Finales y Extraordinarias
* Si se suspende la teoría o la programación en los parciales, se deberá acudir al examen Final (o Extraordinario si fuera necesario).
* Los exámenes Final y Extraordinario constan de un **test teórico de todo el temario** y una **prueba práctica de programación** donde se debe aprobar obligatoriamente tanto la sección de PThreads como la de MPI de manera independiente.
* *Condición de Presentado:* La entrega de cualquier examen o actividad práctica implica que el alumno constará como **"Presentado"** en el acta de la convocatoria.

> ⚠️ **Política de Honestidad Académica:** Cualquier intento de copia, plagio o suplantación de identidad conllevará la pérdida automática de la convocatoria. Si la infracción ocurre durante un examen parcial, el alumno perderá adicionalmente el derecho a presentarse al examen final ordinario. (Ver *Acta de Copia en Examen*).

---

## 6. Profesorado y Estructura de la Plataforma Virtual
La plataforma Moodle (Aula Virtual) se organiza a través de los siguientes menús interactivos:

* **Contenido:** Menú principal estructurado en *Información General*, *Contexto* (motivación técnica), *Módulos* (1, 2 y 3) y *Exámenes*.
* **Calendario:** Horarios de clases presenciales y fechas clave de exámenes.
* **Anuncios y Mensajes:** Canal oficial de comunicación. **Importante:** Para contactar con los profesores se debe usar exclusivamente la pestaña interna de *Mensajes* del Aula Virtual, evitando saturar sus correos institucionales de la UAL.
* **Libro de calificaciones:** Seguimiento de notas, intentos y comentarios del docente.

### 👨‍🏫 Profesores de la Asignatura
* **Francisco José Orts Gómez**
* **José Antonio Martínez García**
*(Nota: Las sesiones de teoría presenciales se grabarán mediante Class Collaborate siempre que la infraestructura técnica del aula lo permita, aunque no se garantiza de forma estricta su disponibilidad ni calidad final).*

---

## 7. Decálogo de Convivencia Digital y Consejos de Éxito

### 💬 Normas de Comunicación Escrita 

* Mantener la cortesía y evitar el uso excesivo de lenguaje coloquial susceptible de malas interpretaciones.
* Utilizar la línea de Asunto de forma descriptiva (máximo 2 o 3 palabras). Queda prohibido usar términos alarmistas como "¡Urgente!" o "Caos".
* Aunque se responda sobre un hilo previo, contextualizar brevemente el problema actual en el cuerpo del mensaje.
* No escribir textos completamente en mayúsculas, ya que en entornos digitales equivale a gritar y dificulta notablemente la lectura.
* Emplear emoticonos [:-)] de forma estratégica para suavizar comentarios irónicos o aportar un tono distendido sin caer en la burla.    

### Consejos para Aprobar la Asignatura

* Dedicación constante: La asignatura requiere un trabajo semanal continuo; no es viable asimilar todo el contenido de golpe al final del cuatrimestre.

* Sigue el orden modular: Completa y entrega las actividades de un módulo y realiza su correspondiente pre-examen antes de intentar avanzar al siguiente bloque temático.

* Asistencia a clase: Aunque no es obligatoria, las estadísticas de cursos anteriores demuestran que la tasa de aprobados es drásticamente superior entre los alumnos que asisten regularmente a las clases presenciales.

* Persistencia: Aunque se suspenda el primer examen parcial, se recomienda presentarse al segundo. El feedback constructivo de los profesores en las correcciones es vital para preparar con garantías el examen final.

* Comprensión individual: Aunque los trabajos prácticos se realicen en equipos de hasta 3 personas, cada integrante debe dominar el código por completo, ya que los exámenes de programación son estrictamente individuales.
