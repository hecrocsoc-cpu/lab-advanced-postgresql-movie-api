## Preguntas del lab

1. ¿Cuándo es contraproducente crear un índice?
La tabla tiene muchas escrituras frecuentes (logs, métricas, auditorías), la tabla es muy pequeña o el índice es sobre una columna que apenas se usa en consultas.

2. ¿Qué diferencia hay entre RANK() y DENSE_RANK()?
Con RANK() si dos películas empatan en la posición 1, la siguiente es la 3 (se salta el 2).
Con DENSE_RANK() si dos películas empatan en la posición 1, la siguiente es la 2 (no se salta ningún número).

3. ¿Por qué el trigger usa AFTER en lugar de BEFORE?
Con AFTER el registro en la auditoría se hace después de que la operación se complete con éxito. Esto garantiza que solo se auditan cambios que realmente ocurrieron.

4. ¿Por qué LEFT JOIN en lugar de INNER JOIN?
Con INNER JOIN las películas sin director o sin género desaparecerían del resultado mientras que con LEFT JOIN aparecen todas las películas aunque les falte algún dato, mostrando NULL en los campos vacíos.

5. ¿Qué películas tienen usuarios más entusiastas que la crítica? ¿Y al revés?
Roma: usuarios dan 10, crítica 7.7 (diferencia +2.30) y Get Out: usuarios dan 9, crítica 7.7 (diferencia +1.30)
Barbie: usuarios dan 6.5, crítica 6.9 (diferencia -0.40)

6. ¿Qué directores tienen trayectoria ascendente?
 Denis Villeneuve.

 