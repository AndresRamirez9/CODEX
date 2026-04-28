# Práctica Temática: Propuesta de Mini Proyecto Documentado para Sistemas

## 1) Título de la práctica
**Diseño de Propuesta: Herramienta Temática de Terminal (Mini Proyecto)**

> Ejemplos de temas válidos:
> - *Mini Toolkit en ARM64*
> - *Asistente de Estudio en Terminal*
> - *Reporteador de Información del Sistema*
> - *Organizador de Archivos*
> - *Juego de Aprendizaje en Línea de Comandos*

---

## 2) Descripción general
En esta actividad **no se busca construir un sistema grande**, sino diseñar una **propuesta sólida, clara y bien documentada** para una práctica pequeña de arquitectura/computación de sistemas.

Cada estudiante definirá una idea temática y elegirá **un solo lenguaje principal** para su implementación:
- **ARM64 Assembly**
- **C**
- **Python**
- **Bash**

### Lineamientos importantes
- Si eliges **ARM64 Assembly**, tu alcance debe ser **muy pequeño** (programas cortos y específicos).
- La prioridad es la **documentación, planeación y justificación técnica** antes de escribir mucho código.
- El proyecto debe ser **compatible con trabajo académico de bajo costo** (considerando límites de uso de herramientas gratuitas).
- **No** se permiten proyectos que dependan de:
  - frameworks pesados,
  - APIs pagadas,
  - bases de datos complejas,
  - servicios en la nube,
  - contenedores,
  - integraciones difíciles de replicar.

---

## 3) Entregables del estudiante
Tu repositorio debe incluir, como mínimo, los siguientes archivos:

- `README.md`
- `docs/propuesta.md`
- `docs/caso_de_uso.md`
- `docs/estructura_repositorio.md`
- `docs/plan_de_pruebas.md`
- opcional: `src/`
- opcional: `scripts/`
- opcional: `tests/`

### Requisitos de contenido por archivo

#### `README.md`
Debe incluir:
1. Nombre del mini proyecto.
2. Lenguaje principal elegido (ARM64 Assembly, C, Python o Bash).
3. Resumen en 5–8 líneas.
4. Alcance limitado (qué **sí** y qué **no** hará).
5. Instrucciones básicas de uso (aunque sea preliminar).
6. Estructura general del repositorio.

#### `docs/propuesta.md`
Debe incluir:
1. Problema u oportunidad que atiende.
2. Objetivo general y 2–4 objetivos específicos.
3. Usuarios objetivo.
4. Lista de funcionalidades mínimas (MVP).
5. Restricciones técnicas (tiempo, herramientas, recursos).
6. Riesgos y mitigaciones.

#### `docs/caso_de_uso.md`
Debe incluir:
1. Descripción narrativa del escenario de uso.
2. Actor principal.
3. Precondiciones.
4. Flujo principal paso a paso.
5. Flujos alternos (al menos 2).
6. Resultado esperado.

#### `docs/estructura_repositorio.md`
Debe incluir:
1. Árbol de carpetas del proyecto propuesto.
2. Propósito de cada carpeta/archivo.
3. Convenciones de nombres (scripts, código, pruebas, docs).
4. Estrategia para separar documentación y código.

#### `docs/plan_de_pruebas.md`
Debe incluir:
1. Objetivo de pruebas.
2. Casos de prueba funcionales mínimos (al menos 5).
3. Entradas y salidas esperadas por caso.
4. Criterios de aceptación.
5. Evidencia sugerida (capturas, logs, comandos ejecutados).

---

## 4) Estructura recomendada del repositorio
Usa como base esta estructura mínima:

```text
nombre-del-proyecto/
├── README.md
├── docs/
│   ├── propuesta.md
│   ├── caso_de_uso.md
│   ├── estructura_repositorio.md
│   └── plan_de_pruebas.md
├── src/
│   └── main.<ext>
├── scripts/
│   └── run.sh
└── tests/
    └── test_plan.md
```

> `main.<ext>` depende del lenguaje elegido:
> - `main.s` (ARM64 Assembly)
> - `main.c` (C)
> - `main.py` (Python)
> - `main.sh` (Bash)

---

## 5) Restricciones de alcance (obligatorias)
Para mantener la práctica pequeña y viable:
1. Máximo **1 problema principal** a resolver.
2. Máximo **3 funcionalidades núcleo**.
3. Máximo **2 scripts auxiliares**.
4. Dependencias externas: idealmente **0** (o mínimas y gratuitas).
5. Tiempo estimado de implementación inicial: **4 a 8 horas**.

---

## 6) Rúbrica sugerida (100 puntos)

- **Claridad de la propuesta (25 pts)**
  - Problema bien definido, objetivo claro y alcance realista.
- **Calidad de documentación (30 pts)**
  - Archivos completos, redacción técnica y buena estructura.
- **Diseño del caso de uso (20 pts)**
  - Flujo principal correcto, alternos coherentes y resultado verificable.
- **Plan de pruebas (15 pts)**
  - Casos útiles, medibles y alineados al objetivo.
- **Orden del repositorio (10 pts)**
  - Estructura limpia, consistente y fácil de navegar.

---

## 7) Criterios de aceptación de la actividad
Tu entrega se considera completa si:
- Incluye todos los archivos obligatorios.
- Está escrita con enfoque técnico y académico.
- Define alcance pequeño y realista.
- Es coherente con un solo lenguaje principal.
- Permite que otra persona implemente el proyecto sin ambigüedad mayor.

---

## 8) Sugerencias por lenguaje

### ARM64 Assembly
- Recomendada solo para utilidades muy pequeñas.
- Ejemplos: conversión simple de unidades, suma/resta de arreglos cortos, manejo básico de entrada/salida.

### C
- Útil para utilerías de sistema, parsing simple de texto, procesamiento básico de archivos.

### Python
- Ideal para prototipos rápidos en terminal y automatización sencilla.

### Bash
- Adecuado para automatización de tareas de sistema y organización de archivos.

---

## 9) Formato de entrega en GitHub Classroom
1. Crea tu repositorio desde la asignación.
2. Agrega los archivos obligatorios con contenido completo.
3. Realiza commits descriptivos (ejemplo: `docs: define caso de uso y plan de pruebas`).
4. Sube tu propuesta final antes de la fecha límite.

---

## 10) Plantilla breve de inicio (opcional para estudiantes)
Puedes iniciar `docs/propuesta.md` con este formato:

```md
# Propuesta del Mini Proyecto

## Nombre tentativo

## Lenguaje principal

## Problema a resolver

## Objetivo general

## Objetivos específicos
- 
- 
- 

## Funcionalidades mínimas (MVP)
- 
- 
- 

## Alcance y límites

## Riesgos y mitigación
```

---

### Nota final
La meta de esta práctica es que aprendas a **pensar como arquitecto/a de soluciones pequeñas**: delimitar, justificar, documentar y planear pruebas antes de programar a gran escala.
