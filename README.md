# S02---LISTA-DE-EJERCICIOS-



Texto para el LOG.md (cambios respecto al post “DBSCAN in Python: learn how it works”)
Inspiración

El código de este proyecto se inspiró en el artículo “DBSCAN in Python: learn how it works” de Ander Fernández https://anderfernandez.com/en/blog/dbscan-python-tutorial/
Ese post explica la lógica de DBSCAN paso a paso y da ejemplos con Python.


Uso de pairwise_distances
El tutorial sugería usar bucles para calcular distancias.
Aquí se reemplazó por sklearn.metrics.pairwise_distances, lo que hace el código más compacto y rápido.
Expansión de clusters con lista seeds
Se mantuvo la idea de expansión iterativa (añadir vecinos densos a una lista y recorrerla), pero se redujo a un while en lugar de funciones recursivas.
Bloque de ejecución __main__
Se agregó un bloque al final para que, si el archivo se ejecuta directamente, genere un dataset con make_blobs y muestre los clusters en consola.
Esto no estaba en el post original, pero facilita las pruebas rápidas.
Enfoque educativo
Se priorizó que el código fuese corto y fácil de leer, más que una implementación optimizada como la de scikit-learn.
