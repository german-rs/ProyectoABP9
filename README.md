# 📊 Diagnóstico y Comunicación de Insights Organizacionales
### Evaluación Módulo 9 – Fundamentos de la Narrativa de Datos | Alkemy

---

## 📍 Situación Inicial

La Dirección de Planificación Estratégica de una empresa de tecnología detectó una **caída sostenida en el rendimiento** de tres equipos internos (Desarrollo, QA y Soporte) durante los últimos dos trimestres. Los reportes mensuales existen, pero no comunican con claridad qué está ocurriendo ni por qué.

---

## 🔍 Lección 1: El Análisis de Datos

### Datos simulados – Rendimiento por equipo (Q1 a Q4)

| Equipo      | Q1 (%) | Q2 (%) | Q3 (%) | Q4 (%) |
|-------------|--------|--------|--------|--------|
| Desarrollo  | 87     | 83     | 74     | 65     |
| QA          | 91     | 88     | 80     | 72     |
| Soporte     | 85     | 84     | 83     | 81     |

> **Métricas consideradas:** tareas completadas a tiempo, bugs entregados al cliente, tickets resueltos dentro del SLA.

### 🧠 Hipótesis

> *"La caída en el rendimiento de los equipos de Desarrollo y QA no es aleatoria: responde a un aumento en la carga de trabajo sin un ajuste proporcional de recursos ni procesos, lo que genera deuda técnica acumulada y fatiga operativa."*

### 💡 Insight Principal

**Los equipos de Desarrollo y QA perdieron más de 20 puntos porcentuales de rendimiento en 4 trimestres, mientras que Soporte se mantuvo estable.** Esto sugiere que el problema no es cultural ni organizacional global, sino específico de los equipos que gestionan el ciclo de producto.

### 📌 Implicancia en la Toma de Decisiones

Este insight permite a la dirección enfocar la intervención: **no es necesario rediseñar toda la organización**, sino revisar la carga, los procesos y los recursos asignados específicamente a Desarrollo y QA. Actuar sin este foco podría generar soluciones costosas e ineficaces.

---

## 📖 Lección 2: La Estructura Narrativa

### Mensaje Principal

> *"Dos de nuestros tres equipos clave están en caída libre. Si no actuamos en Q1 del próximo año, el impacto llegará al cliente."*

### 🎬 Storyboard Narrativo

```
┌─────────────────────────────────────────────────────────────────┐
│  CUADRO 1 – CONTEXTO                                            │
│  La empresa creció un 30% en clientes durante el último año.    │
│  Los equipos internos no escalaron al mismo ritmo.              │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│  CUADRO 2 – PROBLEMA                                            │
│  El rendimiento de Desarrollo cayó de 87% a 65% en 4 trimestres.│
│  QA bajó de 91% a 72%. Soporte se mantuvo estable.             │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│  CUADRO 3 – HALLAZGO                                            │
│  La caída es progresiva y sistemática, no puntual.              │
│  El equipo de Soporte (sin cambios en carga) no se vio afectado.│
│  → El problema está en la gestión de carga del ciclo de producto│
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│  CUADRO 4 – RECOMENDACIÓN                                       │
│  Intervenir en Q1 con: revisión de backlog, incorporación de    │
│  al menos 2 recursos en Desarrollo, y sprint de deuda técnica   │
│  en QA antes del próximo release mayor.                         │
└─────────────────────────────────────────────────────────────────┘
```

**Formato de comunicación:** Mixto – presentación visual para directivos + documento escrito de respaldo.

---

## 🗂️ Lección 3: Estructuras de Datos

### Tipo de datos identificados

| Dimensión        | Clasificación                        |
|------------------|--------------------------------------|
| Temporalidad     | **Temporales** (Q1 → Q4, serie de tiempo) |
| Variables        | **Cuantitativas continuas** (% de rendimiento) |
| Categorías       | **Cualitativas nominales** (nombre del equipo) |
| Estructura       | **Relacional-comparativa** (equipos entre sí a lo largo del tiempo) |

### ✅ Justificación del Gráfico Elegido

Se elige un **gráfico de líneas múltiples (line chart)** porque:

- Los datos son **temporales** → el eje X representa trimestres en orden cronológico.
- Permite ver la **tendencia de cada equipo** de forma simultánea.
- Facilita la **comparación visual** entre equipos (Desarrollo y QA vs. Soporte).
- Evita distorsiones que generarían gráficos de torta o barras apiladas en este contexto.

> ⚠️ Se descarta el gráfico de barras agrupadas porque, si bien es válido para comparar valores puntuales, **no comunica la tendencia de caída** con la misma inmediatez que una línea descendente.

---

## 📈 Lección 4: Visualización de Datos

### Representación en tabla (equivalente al gráfico de líneas)

```
Rendimiento por equipo – Evolución trimestral

100% ┤
 90% ┤  ●──●              ← QA (inicia alto, cae)
 80% ┤      ╲   ●──●      ← Soporte (estable)
 70% ┤  ●──● ╲─╱
 60% ┤         ●──●       ← Desarrollo (caída más pronunciada)
     └──────────────────
        Q1   Q2   Q3   Q4
```

### 🎨 Principios de Diseño Aplicados

| Principio             | Aplicación                                                                 |
|-----------------------|----------------------------------------------------------------------------|
| **Limpieza visual**   | Sin grillas innecesarias. Solo ejes X e Y con etiquetas mínimas.           |
| **Foco en lo importante** | Línea de Desarrollo destacada en rojo. QA en naranja. Soporte en gris neutro. |
| **Confianza en datos**| Cada punto del gráfico corresponde a un valor real de la tabla.            |
| **Marcas visuales**   | Posición (eje Y = rendimiento), Color (diferencia equipos), Forma (puntos en cada Q). |
| **Título accionable** | *"Desarrollo y QA perdieron más del 20% de rendimiento en un año"*        |

### 🖼️ Especificaciones del Gráfico Final

```
Título:    "Desarrollo y QA perdieron más del 20% de rendimiento en un año"
Subtítulo: "Comparación trimestral de rendimiento interno – 2024"
Eje X:     Trimestre (Q1 / Q2 / Q3 / Q4)
Eje Y:     % de Rendimiento (0% – 100%)
Series:    Desarrollo (🔴), QA (🟠), Soporte (⚫)
Herramienta sugerida: Datawrapper o Flourish Studio
```

---

## ✅ Conclusiones y Recomendaciones

1. **El problema es focalizado:** Solo Desarrollo y QA muestran caída sistemática. Soporte es el grupo de control que valida que el problema no es organizacional global.

2. **La tendencia es urgente:** A este ritmo, en Q1 del próximo año ambos equipos podrían caer por debajo del 60%, nivel crítico para la entrega al cliente.

3. **Acciones recomendadas:**
   - 🔧 Auditar la carga de trabajo de Desarrollo y QA (comparar volumen Q1 vs Q4).
   - 👥 Incorporar al menos 2 recursos en el equipo de Desarrollo antes de Q1.
   - 🧹 Planificar un sprint dedicado exclusivamente a deuda técnica en QA.
   - 📅 Establecer una revisión mensual de rendimiento con alerta temprana.

---

## 🛠️ Herramientas Utilizadas

- **Análisis:** Simulación de datos basada en métricas reales de equipos tech.
- **Narrativa:** Estructura storytelling (contexto → problema → hallazgo → recomendación).
- **Visualización:** Datawrapper / Flourish Studio (line chart).
- **Presentación:** Markdown + Google Slides / Canva.

---

## 📚 Referencias

- [Storytelling with Data](https://storytellingwithdata.com/)
- [Datawrapper Blog – Story Structure](https://blog.datawrapper.de/storystructure/)
- [Tableau – Data Visualization](https://www.tableau.com/learn/articles/data-visualization)

---

*Proyecto desarrollado como parte del Módulo 9 – Alkemy | 2024*