# TA-IND-01 — Actividad Autónoma 1: Caso GAD cantonal

**Asignatura:** Ingeniería de Requisitos (ISR-401)  
**Estudiante:** Cedeño Avila Winston Damian  
**Carrera:** Ingeniería de Software  
**Nivel / paralelo:** Cuarto «B»  
**Universidad:** Universidad Técnica Estatal de Quevedo (UTEQ)

## Objetivo

Analizar el caso hipotético de un GAD cantonal que necesita un sistema de cobro de impuestos prediales en línea. Se proponen requisitos claros y verificables como aplicación académica de ISO/IEC/IEEE 29148:2018 y el modelo de calidad ISO/IEC 25010:2023.

## Estado del trabajo

**Borrador — segundo avance técnico (2 de noviembre de 2026).**

Se mantienen los seis actores y los cinco requisitos funcionales del primer avance. En esta revisión se agregan cinco RNF medibles, cada uno clasificado en una característica de ISO/IEC 25010:2023 y acompañado por una prueba propuesta. Los valores numéricos no se presentan como datos oficiales ni como resultados de mediciones.

**Pendiente:** tres restricciones y dos dependencias justificadas; revisar la coherencia final del documento y las fuentes antes de la entrega.

La especificación se refiere a un **GAD hipotético**: todavía no se dispone de entrevistas, contratos de servicio, sistema implementado ni resultados de pruebas.

## Archivos

| Archivo | Contenido |
|---|---|
| `actividad_autonoma_1.tex` | Documento fuente LaTeX del avance. |
| `referencias.bib` | Referencias verificables (ISO/IEC/IEEE 29148:2018, ISO/IEC 25010:2023). |
| `actividad_autonoma_1.pdf` | PDF compilado a partir del `.tex` del mismo avance. |
| `README.md` | Descripción y pasos para reproducir el PDF. |

## Compilación

Instalar MiKTeX o TeX Live con `pdflatex`, `biber` y los paquetes `IEEEtran`, `babel`, `lmodern`, `microtype`, `csquotes`, `booktabs`, `tabularx`, `array`, `enumitem`, `hyperref`, `biblatex` y `biblatex-ieee`.

Situarse en la carpeta `TA-IND-01` y ejecutar, en este orden:

```bash
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
biber actividad_autonoma_1
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
```

Después de cambiar el `.tex` o el `.bib`, recompilar y subir el PDF regenerado para que coincidan.

## Fuentes, supuestos e integridad

La norma ISO/IEC/IEEE 29148:2018 se referencia en https://www.iso.org/standard/72089.html y el modelo ISO/IEC 25010:2023 en https://www.iso.org/standard/78176.html.

El documento declara asistencia de ChatGPT para la preparación del borrador técnico y la edición LaTeX. Las decisiones y metas propuestas requieren revisión crítica del estudiante antes de la entrega. No se atribuyen entrevistas, consultas a personal municipal ni pruebas que no se han realizado.
