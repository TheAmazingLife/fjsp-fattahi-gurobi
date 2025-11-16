# Flexible Job Shop Scheduling Problem (FJSP)

**Curso:** Optimización I
**Semestre:** 2-2025  
**Fecha límite:** 14 de noviembre, 2025, 23:59 hrs

---

## 📋 Descripción del Proyecto

Implementación en Python de un modelo de programación entera mixta para resolver el **Flexible Job Shop Scheduling Problem (FJSP)** utilizando GUROBIpy, basado en el modelo matemático propuesto por **Fattahi et al. (2007)**.

### Objetivo

Resolver 20 instancias del problema FJSP minimizando el makespan (tiempo total de finalización) mediante un modelo de optimización lineal entera mixta.

### Referencias

- **Paper:** Fattahi, P., Saidi Mehrabad, M., & Jolai, F. (2007). Mathematical modeling and heuristic approaches to flexible job shop scheduling problems. *Journal of Intelligent Manufacturing*, 18(3), 331-342.
- **Instancias:** [SchedulingLab/fjsp-instances](https://github.com/SchedulingLab/fjsp-instances)

---

## 📁 Archivos del Proyecto

```
├── fjsp_solver.ipynb      # Notebook con implementación y análisis
├── instances.json         # Metadata de las 20 instancias
├── fattahi/              # Carpeta con instancias
│   ├── sfjs01-10.txt     # Single Flexible Job Shop
│   └── mfjs01-10.txt     # Multi Flexible Job Shop
└── Fattahi2007.pdf       # Paper de referencia
```

---

## 🚀 Uso

### Ejecutar el Notebook

```bash
jupyter notebook fjsp_solver.ipynb
```

El notebook incluye:
- ✅ Carga de instancias desde carpeta `fattahi/`
- ✅ Metadata desde `instances.json`
- ✅ Implementación del modelo de Fattahi et al.
- ✅ Solución de las 20 instancias
- ✅ Generación de tabla de resultados
- ✅ Visualizaciones y análisis

### Instancias

Las 20 instancias en `fattahi/` contienen:
- **10 SFJS** (Single Flexible): Cada operación usa UNA máquina de varias opciones
- **10 MFJS** (Multi Flexible): Cada operación puede usar MÚLTIPLES máquinas

Formato por archivo:
```
<n_jobs> <n_machines>
<n_ops> <n_machines_op1> <machine> <time> ... <n_machines_op2> <machine> <time> ...
...
```

### Metadata (instances.json)

Contiene valores óptimos conocidos y cotas para comparación con resultados del solver.

## 📊 Resultados

El notebook genera:
- `results.csv` - Tabla con métricas (tiempo, makespan, gap, variables, restricciones)
- `results_analysis.png` - Gráficos de análisis