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


## Estructura

Este libro está compuesto sobre la base de una visión sistémica de los ordenadores. En cada *nivel de abstracción* se presentan diferentes tipos de descripciones o *modelos*. En la "lección 0" se explica esta concepción sistémica, y a su término podremos situar en ese contexto la estructura y el contenido del curso. Adelantemos aquí que, aparte de esa lección 0 y de tres apéndices, consta de tres partes con ocho lecciones cada una.

Todas las lecciones empiezan con un apartado de "Proósito". En él se fijan los objetos de la lección y, cuando es la primera de una parte, del conjunto de lecciones. Se incluyen también ahí las reflexiones o consideraciones previas que sean necesarias como introducción. En los apartados de "Resumen" se recuerda lo tratado y en su caso se añaden conclusiones finales. Nos ha parecido conveniente ir complementando la exposición con algunos particulares no estrictamente técnicos, que aparecen al final de las lecciones. Con los apartados de "Observaciones terminológicas" pretendemos compensar el abuso de barbarismos tan extendido en la informáticva; para algunos términos hemos adoptado traducciones poco usuales, que se explican o se justifican en esos apartados. En las "Notas históricas" presentamos algunos hechos que creemos conveniente conocer para la buena comprensión de los ordenadores.

Para su uso como "libro de texto", los conceptos incluidos en cada lección pueden tratarse en dos "clases" de unos cincuienta minutos, suponiendo que se trata de clases *de síntesis*. Estimamos que desarrollar el contenido de todas las lecciones requeriría una asignatura de unos quince créditos (150 horas). Para una (o dos) de seis créditos (módulo bastante extendido en los planes de estudio actuales) es preciso seleccionar. Al final de la lección 0 se dan algunas orientaciones a este respecto.

## Ensambladores y simuladores

Como complemento, están disponibles unos programas (para MS-DOS) que permiten practicar, y afianzar así los conceptos explicados en el texto. Se trata de ensambladores y simuladores de Símplez y Algorítmez. En lugar del procedimiento tradicional de incluir un disquete con el libro (que complica los procesos editoriales, repercute en el precio, y , sobre todo, dificulta la actualización de versiones) hemos preferido dejarlos accesibles por "ftp" a través de Internet. El procedimiento para obtenerlos es:[^5]

1. Conéctese al servidor:  
    ```% ftp ftp.dit.upm.es```

2. El servidor responde y pregunta por el nombre ("`Name:`"); escriba, simplemente: "`anonymous`". A continuación pide la contraseña ("`Password:`"); escriba su dirección de correo electrónico.
3. Cambie al directorio que contiene los programas:
   ```ftp> cd pub/doc/books```

4. Ponga el modo de transferencia binario:
    ```ftp> binary```

5. Copie el fichero en su máquina:
    ```ftp> get simalg.tar.Z```

6. Cierre la conexión
    ```ftp> bye```

7. El fichero obtenido está comprimido; haga la descompresión:

    ```% uncompress simalg.tar.Z```

8. El fichero es una concatenación de ficheros; sepárelos:

    ```% tar -xvf simalg.tar```

9. Lea el fichero "`leeeme`"



## Agradecimientos

El autor ha ido adquiriendo los conocimientos que trata de compartir aquí a lo largo de más de veinte años de actividad docente e investigadora en la Escuela Técnica Superior de Ingenieros de Telecomunicación de la Universidad Politécnica de Madrid. No es posible mencionar a todas las personas que, de algún modo, han contribuido en esta formación y maduración personal. Pero el riesgo de olvidar a muchos no justificaría el dejar de destacar a algunos.

Fernando Sáez Vacas me inició en la Informática y, sobre todo, en la forma abierta de estudiar la tecnología y en la docencia universitaria. Su amistad ininterrupmpida ha sido y es una fuente permanente de enriquecimiento.

Entre los profesores que han colaborado en la impartición de la asignatura "Fundamentos de los ordenadores" (cuyo programa ha sido el germen del libro), tengo que destacar, muy especialmente, a Mercedes Garijo, que ha dedicado muchas horas durante los tres últimos años a revisar sucesivas versiones del texto y de las figuras, lo que me ha permitido depurar inconsistencias, carencias, errores y erratas de todo tipo (huelga decir que los que aún quedan son de la exclusiva responsabilidad del autor). Pedro Alonso ha constribuido con un gran número de correcciones, como también Martín Llamas (de la Universidad de Vigo). Las lecciones de introducción a los sistemas operativos (19 a 23) se han beneficiado de numerosas sugerencias de Ángel Álvarez y de Gonzalo de León.

Un antecedente de este libro fueron los dos volúmenes editados en la Escuela hace dieciséis años. Eran el resultado de un trabajo de corrdinación de Fernando Sáez y mío en el que los profesores con los que iniciamos el diseño y la impartición de la citada asignatura contribuían con varios capítulos: Pedro Alonso, Carmen Costilla, Juan Quemada, Enrique Rivero y José María Vela quizás reconozcan aquí todavía algunos detalles inspirados en sus textos.

Además de los mencionados, otros compñaeros con los que he compartido la docencia de ésta y otras asignaturas, y de los que también he aprendido, han sido: Carlos Delgado, José Carlos González, Darío Maravall, Encarna Pastor, Juan Riera, Juan Ramón Velasco y Angel Viña.

Es difícil precisarla y cuantificarla, pero también es innegable y de obligado reconocimiento la positiva influencia de los alumnos en la evolución profesional y personal de un profesor. Por motivos obvios, es imposible dar los nombres de todos. Pero, por su ahínco en la detección de errores y en la crítica constructiva, valga como representantivo el de Oscar José Martínez de la Torre (que además, en estos momentos, es el delegado de los alumnos de la Escuela). Por otra parte, Jesús Pérez Garcilópez ha desarrollado los programas simuladores y ensambladores mencionados más arriba.

En los medios instrumentales, he hecho uso de las aportaciones de Donal Knuth y de Leslie Lamport, creadores de TEX y LATEX, respectivamente. También, de un útil programa de Jose Antonio Mañas, "ftc" (filtro de textos en castellano). Ignacio Bellido, José Miguel Goñi y Juan Ramón Velasco han estado siempre solícitos para resolver los problemas que a veces uno llega a atribuir a duendes infiltrados en las máquinas.

A la elaboración de este libro he dedicado más de seis mil horas, casi cuatro mil de elllas en períodos de vacaciones y fines de semana. La deuda contraída con mi familia es tan grande que sólo cabe dejar constancia de su existencia.

Madrid, junio de 1994  
Gregorio Fernández



[^1]: "**Iniciar** [...] **3.** fig. Instruir en cosas abstractas o muy frofundas". "**Concretar**[...] **3.** Reducir a lo más esencial y seguro la materia sobre la que se habla o escribe". (Diccionario de la Real Academia Española).

[^2]: De hecho, este libro es una refundición de otros tres del mismo autor, de difusión restringida, dirigidos a distintos tipos de lectores: *Fundamentos de los ordenadores*, Servicio de Publicaciones de la E.T.S.I. Telecomunicación, Madrid, 1991 (vol.1) y 1992 (vol.2), *Iniciación concreta a los sistemas operativos*, Servicio de Publicaciones de la E.T.S.I. Telecomunicación, Madrid, 1993, y *Arquitectura de ordenadores* (dos volúmenes), Escuela de Organización Industrial, Madrid, 1993

[^3]: "La informática [*computer science*] es el estudio de los fenómenos que rodean a los ordenadores [...] La máquina, —no ya el hardware, sino la máquina programada, viviente— es el organismo que estudiamos". A. Newell y H. Simon: "Computer science as scientific inquiry: symbols and search". *Communications of the ACM*, 19, 3 (Mar. 1976), pp. 113-126

[^4]: Si no fuera por la renuncia del autor a las "dedicatorias", habría dirigido la de este libro "a los alumnos que se aburren en clase". Esto necesita una explicación (entre otras cosas, para apaciguar el enojo de los colegas). Una de las aberraciones de nuestro sistema educativo universitario es el acto en que se ha convertido la "lección magistral" en la mayoría de los centros. Entendemos que debería ser una clase de síntesis y reforzamiento, impartida tras un período de estudio, acciones tutoriales, clases prácticas y evaluaciones parciales, y preparada muy cuidadosamente. La limitación de recursos no sólo hace inviable este proceso. Determina también un número de alumnos por grupo (más del centener en nuestro caso) que conduce a las "clases teóricas", monólogos en los que el profesor, casi sin interacción con los alumnos (y agobiado a veces por "cubrir el programa"), expone, con su mejor voluntad de hacerse entender, una sucesión más o menos ordenada de conocimientos. Muy frecuentemente, preparando estas clases, reflexiono sobre su escasa eficacia educativa. Y me asombra la capacidad de los alumnos para cumplir estoicamente un "horario" que a veces incluye ¡seis horas seguidas de clase! Salvo que uno fuese, además de profesor, un excepcional orador con poder de seducción del auditorio, ¿no sería más rentable y gratificante para el alumno adquirir los conocimientos por medio de la palabra escrita, a su ritmo y manera? Esta ha sido una de las motivaciones para escribir este libro. Esperamos que nos sirva para organizar las clases de un modo más sensato.

[^5]: Naturalmente, es necesario disponer de un ordenador, estación o terminal conectado a Internet. Este párrafo está dirigido a profesores e instructores. Los lectores no iniciados pueden despejar algo de su perplejidad sobre lo que aquí se dice leyendo el apartado 23.8.