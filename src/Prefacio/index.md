# Prefacio

Este libro está diseñado y escrito para:

* Servir como apoyo didáctico en un *primer curso* sobre los *fundamentos* de la arquitectura de ordenadores y de los sistemas operativos
* Servir también como *iniciación concreta*[^1] al estudio de los sistemas operativos, en un curso sobre estos sistemas (que se supone precedido de otro sobre fundamentos de la arquitectura).
* Servir al lector que, de manera autónoma, desee adquirir *conocimientos básicos* sobre la estructura y el funcionamiento de los ordenadores.
  
## Lectores

Independientemente de la clasificación implícita en el párrafo anterior (alumno de un curso, o "autónomo"), el libro se ha elaborado teniendo presentes tres perfiles de lector:[^2]

* Estudiantes de ingeniería, con conocimientos previos de programación en un lenguaje de alto nivel y de circuitos lógicos
* Profesionales en proceso de "reconversión" a las tecnologías de la información y las comunicaciones.
* Profesionales o estudiantes de otras materias en las que el ordenador se utiliza como una herramienta cuya organización, estructura y funcionamiento internos es conveniente conocer para obtener de ella el máximo provecho.

Como requisito previo, se supone que el lector tiene unos conocimientos mínimos de programación. No es necesario que sepa diseñar programas en ningún lengujae determinado, pero sí que sea capaz de entender algoritmos sencillos escritos en un lenguaje de alto nivel. Algunas de las lecciones requiren también ciertas nociones de codificación y aritmética binario, así como de circuitos lógicos; sobre estos dos temas, se incluyen sendos apéndices con todo lo que hace falta saber para la comprensión del libro.


## Temática

El objeto de estudio aquí es el **ordenador**, no la informática. Es decir, el instrumento, no la ciencia construida a su alrededor.[^3]

Ahora bien, los ordenadores pueden estudiarse en diferentes niveles de abstracción (la explicación de estos niveles es el objeto de la "lección 0"). Otras dos palabras del título, "**arquitectura"** y "**sistemas operativos**", determinan los niveles en los que se centra este libro: los que tienen que ver con el funcionamiento interno del hardware y del software, sin descender más que lo imprescindible a los detalles de los circuitos.


## Enfoque

Tabmién se ha querido dejar constancia en el título del enfoque adoptado. Veámoslo.

Se trata de un **curso** (y no tiene "capítulos", sino "lecciones"). Sea el lector un alumno "regular" o no, está escrito para que pueda seguirse "sin ir a clase".[^4] Como consecuencia, se encontrarán más reiteraciones de las habituales. Pretendemos asegurar la comprensión de cada concepti, asumiendo el riesgo de excedernos en el número de palabras. No obstante, hemos buscado un término medio, pues las lecciones están muy interrelacionadas y la reiteración tienen un límite. El lector encontrará con frecuencia referencias a "apartados" de otras lecciones distintas a la que está estudiando (fácilmente localizables por la forma de encabezar las páginas).

Y es un curso sobre **conceptos básicos**. Además de complejos, los ordenadores son dependientes de unas tecnologías que cambian muy rápidamente. Un curso basado en los productos que hoy se encuentran en el mercado tendria una utilidad efímera, y los conocimientos transmitidos quedarían rápidamente obsoletos. Afortunadamente, después de cincuitea años de sucesivas innovaciones, pueden ya identificarse ciertos conceptos relativamente invariantes e independientes de la tecnología, y en ellos se centra el libro. Para concentrarse mejor en esos conceptos básicos, la exposición se hace sobre "ordenadores ficticios" ("Símplez", "Algorítmez" y "Regístrez"). Pero el "aislamiento" (o abstracción) total de la tecnología es imposible. Algunos datos y modelos concretos, especialmente dentro de las lecciones 5, 8, 12, 15, 16, 17, 18 y 23, pueden empezar a resultar "antiguos" dentro de muy poco (¡quizás antes de que el libro vea la luz!).







[^1]: "**Iniciar** [...] **3.** fig. Instruir en cosas abstractas o muy frofundas". "**Concretar**[...] **3.** Reducir a lo más esencial y seguro la materia sobre la que se habla o escribe". (Diccionario de la Real Academia Española).

[^2]: De hecho, este libro es una refundición de otros tres del mismo autor, de difusión restringida, dirigidos a distintos tipos de lectores: *Fundamentos de los ordenadores*, Servicio de Publicaciones de la E.T.S.I. Telecomunicación, Madrid, 1991 (vol.1) y 1992 (vol.2), *Iniciación concreta a los sistemas operativos*, Servicio de Publicaciones de la E.T.S.I. Telecomunicación, Madrid, 1993, y *Arquitectura de ordenadores* (dos volúmenes), Escuela de Organización Industrial, Madrid, 1993

[^3]: "La informática [*computer science*] es el estudio de los fenómenos que rodean a los ordenadores [...] La máquina, —no ya el hardware, sino la máquina programada, viviente— es el organismo que estudiamos". A. Newell y H. Simon: "Computer science as scientific inquiry: symbols and search". *Communications of the ACM*, 19, 3 (Mar. 1976), pp. 113-126

[^4]: Si no fuera por la renuncia del autor a las "dedicatorias", habría dirigido la de este libro "a los alumnos que se aburren en clase". Esto necesita una explicación (entre otras cosas, para apaciguar el enojo de los colegas). Una de las aberraciones de nuestro sistema educativo universitario es el acto en que se ha convertido la "lección magistral" en la mayoría de los centros. Entendemos que debería ser una clase de síntesis y reforzamiento, impartida tras un período de estudio, acciones tutoriales, clases prácticas y evaluaciones parciales, y preparada muy cuidadosamente. La limitación de recursos no sólo hace inviable este proceso. Determina también un número de alumnos por grupo (más del centener en nuestro caso) que conduce a las "clases teóricas", monólogos en los que el profesor, casi sin interacción con los alumnos (y agobiado a veces por "cubrir el programa"), expone, con su mejor voluntad de hacerse entender, una sucesión más o menos ordenada de conocimientos. Muy frecuentemente, preparando estas clases, reflexiono sobre su escasa eficacia educativa. Y me asombra la capacidad de los alumnos para cumplir estoicamente un "horario" que a veces incluye ¡seis horas seguidas de clase! Salvo que uno fuese, además de profesor, un excepcional orador con poder de seducción del auditorio, ¿no sería más rentable y gratificante para el alumno adquirir los conocimientos por medio de la palabra escrita, a su ritmo y manera? Esta ha sido una de las motivaciones para escribir este libro. Esperamos que nos sirva para organizar las clases de un modo más sensato.
