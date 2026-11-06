# TA-IND-01 — Actividad Autónoma 1: Caso GAD cantonal

**Asignatura:** Ingeniería de Requisitos (ISR-401)  
**Estudiante:** Cedeño Avila Winston Damian  
**Carrera:** Ingeniería de Software — cuarto nivel, paralelo B  
**Universidad:** Universidad Técnica Estatal de Quevedo (UTEQ)

## Tema y alcance

Especificación inicial de requisitos para el cobro de impuestos prediales en línea de un GAD cantonal hipotético. Incluye una pasarela local de pagos y una integración con el SRI condicionada a la existencia de un servicio autorizado.

## Contenido

- Seis partes interesadas y sus necesidades preliminares.
- Cinco requisitos funcionales (RF-01 a RF-05) con comprobaciones propuestas.
- Cinco requisitos no funcionales (RNF-01 a RNF-05) clasificados según ISO/IEC 25010:2023, con métricas y métodos de verificación.
- Tres restricciones justificadas (R-01 a R-03).
- Dos dependencias entre requisitos (D-01 y D-02).
- Matriz de trazabilidad entre necesidades, requisitos y comprobaciones.

Los valores de rendimiento, disponibilidad y demás metas son **supuestos de prueba del caso académico**, no mediciones de un GAD. Las condiciones de integración con proveedores externos están pendientes de confirmación en un proyecto real.

## Archivos

| Archivo | Descripción |
|---|---|
| `actividad_autonoma_1.tex` | Fuente LaTeX del informe. |
| `referencias.bib` | Bibliografía BibLaTeX con estilo IEEE. |
| `actividad_autonoma_1.pdf` | PDF compilado desde la fuente. |
| `README.md` | Información e instrucciones de reproducción. |

## Reproducción del PDF

Se requiere una instalación de TeX Live o MiKTeX con `pdflatex`, `biber`, la clase `IEEEtran` y los paquetes indicados en el preámbulo del `.tex` (entre ellos `biblatex-ieee`). Desde `TA-IND-01`, ejecutar:

```bash
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
biber actividad_autonoma_1
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
```

## Referencias

- [ISO/IEC/IEEE 29148:2018 — Requirements engineering](https://www.iso.org/standard/72089.html)
- [ISO/IEC 25010:2023 — Product quality model](https://www.iso.org/standard/78176.html)

## Declaración de uso de IA

Se utilizó ChatGPT (OpenAI, GPT-6) como apoyo para la redacción, la propuesta de métricas y la edición en LaTeX. El contenido fue revisado antes de su presentación. No se realizaron entrevistas ni pruebas de un sistema municipal.
