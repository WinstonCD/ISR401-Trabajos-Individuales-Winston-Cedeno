# TA-IND-01 — Actividad Autónoma 1: Caso GAD cantonal

**Asignatura:** Ingeniería de Requisitos (ISR-401)  
**Estudiante:** Cedeño Avila Winston Damian  
**Carrera:** Ingeniería de Software  
**Nivel / paralelo:** Cuarto «B»  
**Universidad:** Universidad Técnica Estatal de Quevedo (UTEQ)

## Objetivo

Analizar el caso de un GAD cantonal que necesita un sistema de cobro de impuestos prediales en línea y documentar requisitos claros y comprobables, tomando como referencia ISO/IEC/IEEE 29148:2018.

## Estado del trabajo

**Borrador — primer avance técnico (1 de noviembre de 2026).**

El avance contiene la situación del caso, su alcance preliminar, las partes interesadas y cinco requisitos funcionales con propuestas de comprobación. No es el informe final: todavía falta desarrollar los requisitos no funcionales, su clasificación ISO/IEC 25010:2023, las restricciones y las dependencias.

Los actores y las pruebas descritas se han planteado para un **caso hipotético**. No se han realizado entrevistas al GAD ni pruebas sobre una aplicación implementada.

## Archivos

| Archivo | Contenido |
|---|---|
| `actividad_autonoma_1.tex` | Fuente LaTeX editable del avance. |
| `referencias.bib` | Bibliografía verificable gestionada con biblatex. |
| `actividad_autonoma_1.pdf` | PDF compilado de este mismo avance. |
| `README.md` | Descripción del avance y procedimiento para regenerar el PDF. |

## Compilación (criterio de reproducibilidad)

Se requiere una distribución LaTeX como MiKTeX o TeX Live, con **pdfLaTeX**, **Biber** y los paquetes `IEEEtran`, `babel`, `lmodern`, `microtype`, `csquotes`, `booktabs`, `tabularx`, `array`, `enumitem`, `hyperref`, `biblatex` y su estilo `ieee`.

Desde la carpeta `TA-IND-01`, ejecutar:

```bash
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
biber actividad_autonoma_1
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
```

Después de modificar el `.tex` o la bibliografía, debe volver a compilarse y subirse el PDF actualizado para mantener ambos archivos coherentes.

## Fuentes e integridad académica

Se utiliza la ficha verificable de la norma ISO/IEC/IEEE 29148:2018. En el documento se declara la asistencia de ChatGPT como apoyo para preparar una plantilla y un borrador de redacción. El contenido necesita revisión crítica, ajustes y comprensión por parte del estudiante antes de presentarlo como trabajo evaluable. No se atribuyen entrevistas o verificaciones que no se hayan ejecutado.
