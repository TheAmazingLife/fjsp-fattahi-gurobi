Objetivo: Implementar en Python un modelo de programación entera mixta, utilizando la librería GUROBIpy.


Descripción: Implementar el modelo matemático que resuelve el problema de job shop flexible, propuesto por Fattahi et al. 2007. Notar que el artículo propone también algoritmos heurísticos y metaheurísticos para el problema, pero estos no deben ser implementados.

Fattahi2007.pdfDownload Fattahi2007.pdf

Resolver las instancias del problema presentes en el repositorio https://github.com/SchedulingLab/fjsp-instances/blob/main/README.mdLinks to an external site.

Son 20 instancias de tamaños pequeños y grandes. Dar un tiempo límite de una hora de cómputo a GUROBIpy utilizando los parámetros del solver.

Generar una tabla de resultados incluyendo tamaño de la instancia, número de variables, restricciones, tiempo (s), función objetivo, gap y tiempo de cómputo. El gap corresponde a la diferencia entre la mejor solución conocida y una cota superior de solución. Lo entrega el solver.

En el informe deben incluir la tabla con los resultados y un análisis en cuanto a tiempos y función objetivo, respecto a los resultados presentados para el modelo en la Tabla 1 del artículo.

Las conclusiones deben ser en relación al desempeño del solver (¿El gap final indica que el solver encontró una buena solución o aún hay espacio para mejora?), el modelo (¿Qué características del modelo (número de variables, restricciones, tipo de variables, etc.) parecen influir más en la dificultad de resolución?), sobre la tarea (¿Qué habilidades o conocimientos crees que desarrollaste al implementar y analizar este modelo?). No se deben responder las preguntas de manera textual, si no que pueden utilizarlas para guiar el relato.

Se recuerda que la entrega de archivos en blanco, corresponde a NCR. No pueden ser tareas presentadas en semestres anteriores. Se puede utilizar inteligencia generativa pero, al entregar el trabajo, garantizan que han revisado y validado su contenido.


Fecha de Entrega: viernes 14 de noviembre de 2025, 23:59 hrs. por Canvas.


Entrega: Deben subir a la plataforma Canvas dos archivos:

-Informe de máximo 2 páginas con la identificación de la pareja/grupo, con la tabla, análisis y conclusiones. Formato PDF.

-Script en Python (.py o .ipynb) con la implementación en GUROBI.
