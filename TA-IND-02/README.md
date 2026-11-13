# TA-IND-02 — Priorización de requisitos: MoSCoW, Kano y votación ponderada

**Asignatura:** Ingeniería de Requerimientos (ISR-401)  
**Estudiante:** Cedeño Avila Winston Damian  
**Carrera:** Ingeniería de Software — cuarto nivel, paralelo B  
**Universidad:** Universidad Técnica Estatal de Quevedo (UTEQ)  
**Actividad del SGA:** TA-TAR-02 — SUM — Trabajo individual: priorización de requisitos con MoSCoW, Kano y votación ponderada  
**Estado:** Estructura inicial del trabajo. **Aún no se ha asignado aquí un dominio ni se han recopilado respuestas de participantes.**

## Objetivo

Aplicar tres técnicas de priorización a un conjunto de requisitos de un dominio **asignado por sorteo en el SGA**. La prioridad final deberá justificarse con criterios explícitos y datos originales de personas reales, no solamente con la opinión del analista. El dominio no puede coincidir con el del Proyecto Final de Carrera (PFC).

## Actividades por desarrollar

1. **Catálogo de requisitos:** formular 20 requisitos según ISO/IEC/IEEE 29148:2018: al menos 12 funcionales y 8 de calidad con métricas y umbrales verificables.
2. **MoSCoW:** clasificar y justificar individualmente cada requisito como Must, Should, Could o Won't. Estimar el esfuerzo y comprobar que los Must **no superen el 60 % del esfuerzo total estimado**; el límite no se refiere al número de requisitos.
3. **Kano:** seleccionar 8 características y aplicar a por lo menos **5 participantes reales** una pregunta funcional y otra disfuncional por característica; conservar las respuestas, tabularlas y clasificarlas con la tabla de evaluación Kano.
4. **Votación ponderada:** solicitar a por lo menos **3 participantes reales** que distribuyan **100 puntos por persona** entre los 20 requisitos; sumar y ordenar los puntajes.
5. **Comparación:** explicar coincidencias y diferencias entre MoSCoW, Kano y la votación; calcular y justificar la correlación de rangos de **Spearman entre MoSCoW y votación**, documentando el tratamiento de empates.
6. **Decisión:** proponer el conjunto priorizado para la primera versión del sistema y justificar qué requisitos quedan fuera.

## Estructura prevista (archivos aún no creados)

```text
TA-IND-02/
├── README.md
├── main.tex                        # Informe LaTeX, previsto: 6 a 10 páginas de contenido
├── referencias.bib                 # Bibliografía real en estilo IEEE
├── main.pdf                        # PDF compilado desde main.tex
├── datos/
│   ├── kano.csv                    # Respuestas reales anonimizadas
│   └── votacion_ponderada.csv      # Votos reales anonimizados
└── evidencias/
    └── MANIFIESTO.md               # Referencias a originales guardados en privado
```

Los dos CSV deberán permitir reproducir los cálculos. El manifiesto público registrará nombre de archivo de respaldo, fecha, duración y huella SHA-256, **sin nombres, cédulas, contactos ni respuestas identificables**. Consentimientos, audios, fotografías o documentos originales de participantes se conservarán en una carpeta institucional privada accesible para el docente; no en este repositorio público.

## Compilación prevista

Cuando exista `main.tex`, se documentarán sus paquetes y se verificará una compilación limpia con **pdfLaTeX y Biber**, en este orden:

```bash
pdflatex -interaction=nonstopmode -halt-on-error main.tex
biber main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

No se declara reproducibilidad hasta que los archivos estén creados y la compilación haya sido comprobada.

## Entrega e integridad académica

- En el **SGA** se subirá **únicamente una carátula PDF de una página**, con datos de la actividad, fecha límite y URL pública del repositorio completa en **una sola línea**.
- El historial debe reflejar **avances sustantivos en por lo menos tres días distintos**. Se registrarán fechas y cambios reales; no se simularán commits ni encuestas.
- La guía exige al menos **3 referencias IEEE verificables**, al menos **2 de los últimos 5 años**, y una declaración precisa de uso o no uso de IA.
- La actividad requiere la **formativa vinculada entregada válidamente**. No se publicarán datos personales de participantes ni se inventarán respuestas, votaciones o resultados.

## Diferencias que deben confirmarse en el SGA del paralelo B

| Campo | Descripción de TA-TAR-02 en el SGA | PDF de guía TA-IND-02 (indica paralelo A) |
|---|---|---|
| **Cierre** | **28 de noviembre de 2026, 23:59** | **5 de diciembre de 2026, 23:59** |
| **Formativa previa** | **GA-SIM-01** | **FORM-SIM-01** |

Antes de planificar la entrega se debe confirmar con el docente cuál fecha y código se aplican al **paralelo B**. Hasta aclararlo, conviene trabajar con la **fecha más temprana: 28 de noviembre de 2026**.

## Próximo paso

Confirmar el **dominio adjudicado por sorteo** y la **formativa vinculada**. Solo después se comenzará el catálogo de requisitos y se prepararán los instrumentos de recogida de datos reales.
