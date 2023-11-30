# Exploración de la Inteligencia Artificial: El Rol Fundamental de las Heurísticas

El término "heurística" se emplea en los campos de la psicología y ciencias de la computación para hacer referencia a estrategias o reglas prácticas que agilizan la resolución de problemas y la toma de decisiones, priorizando la eficiencia aunque no asegurando necesariamente la solución óptima. Estas reglas, por lo general, son simples y se fundamentan en la experiencia previa, el sentido común y el conocimiento acumulado con el tiempo.

El propósito esencial de la heurística en la resolución de problemas consiste en facilitar el proceso cognitivo, capacitando a las personas para abordar situaciones complejas de manera más efectiva, incluso cuando la información sea incompleta o existan restricciones temporales. En lugar de explorar exhaustivamente todas las soluciones posibles, las heurísticas ofrecen atajos mentales que reducen la carga cognitiva y permiten tomar decisiones de forma más expedita.

Es crucial destacar que, aunque las heurísticas resultan útiles en diversos contextos, también pueden dar lugar a errores sistemáticos, conocidos como sesgos heurísticos. Estos sesgos pueden originarse debido a la simplificación excesiva de la información o a la aplicación inapropiada de reglas heurísticas.

# Algunos ejemplos de heurísticas comunes engloban:

Heurística de Representatividad: Tendencia a evaluar la probabilidad de un evento según cuánto se asemeje a un prototipo o estereotipo.

Heurística de Disponibilidad: Tendencia a estimar la probabilidad de un evento basándose en la facilidad con que se puede recordar o recuperar información relevante.

Heurística de Anclaje y Ajuste: Tendencia a fundamentar decisiones en un valor inicial (anclaje) y a ajustar la estimación final de manera insuficiente.

Heurística de la Satisfacción: Tendencia a concluir la búsqueda de soluciones tan pronto como se encuentra una que parezca aceptable.

En resumen, las heurísticas son estrategias cognitivas que permiten a las personas tomar decisiones y resolver problemas de manera más eficiente. No obstante, es esencial reconocer que también pueden introducir sesgos y errores. Su aplicación efectiva se encuentra en el equilibrio entre la simplificación útil y la capacidad de adaptarse a situaciones específicas.



# Problema Laberinto
~~~python
laberinto = [
       [1 , 1 , 1 , 1 , 1 , 1 , 1 , 1 , 1 ],
       [0 , 0 , 0 , 0 , 0 , 0 , 1 , 0 , 1 ],
       [1 , 1 , 1 , 0 , 1 , 1 , 1 , 0 , 1 ],
       [1 , 0 , 0 , 0 , 1 , 0 , 1 , 0 , 1 ],
       [1 , 0 , 1 , 1 , 1 , 0 , 1 , 0 , 1 ],
       [1 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 1 ],
       [1 , 0 , 1 , 1 , 1 , 0 , 1 , 0 , 1 ],
       [0 , 0 , 1 , 0 , 0 , 0 , 1 , 0 , 1 ],
       [1 , 1 , 1 , 1 , 1 , 1 , 1 , 1 , 1 ],
      ]

