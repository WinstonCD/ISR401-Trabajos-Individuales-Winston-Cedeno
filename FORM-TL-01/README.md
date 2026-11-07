# FORM-TL-01 — Identificación y clasificación de tipos de requisitos

**Asignatura:** Ingeniería de Requisitos (ISR-401)  
**Estudiante:** Cedeño Avila Winston Damian  
**Nivel y paralelo:** Cuarto «B» — Ingeniería de Software  
**Universidad:** Universidad Técnica Estatal de Quevedo

## Tema

Clasificación de requisitos para la **Plataforma de gestión de citas médicas** del Policlínico Ribera del Quevedo (caso académico ficticio).

## Contenido

El informe contiene 20 enunciados clasificados y justificados en las dimensiones solicitadas: tipo principal de requisito, producto/proceso y sistema/software. Se identifican cinco requisitos de calidad vagos y se proponen redacciones con métricas y umbrales. Incluye una comparación documental con el trabajo de Mendoza Palma Allan Jeremy, con coincidencias, diferencias y justificaciones.

## Archivos

- `main.tex`: informe fuente en LaTeX (clase `IEEEtran`, una columna).
- `referencias.bib`: referencias para `biblatex` con estilo IEEE.
- `main.pdf`: PDF compilado desde el código fuente.
- `README.md`: descripción e instrucciones de compilación.

## Compilación

Se requiere TeX Live o MiKTeX con `pdflatex`, `biber`, `IEEEtran`, `babel`, `lmodern`, `microtype`, `csquotes`, `longtable`, `tabularx`, `booktabs`, `needspace`, `hyperref` y `biblatex-ieee`.

Desde esta carpeta, ejecutar:

```bash
pdflatex -interaction=nonstopmode -halt-on-error main.tex
biber main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

## Alcance y declaración

Las cifras de los requisitos de calidad son **objetivos de prueba propuestos** y no resultados medidos. La comparación presentada contrasta los dos informes y explica los criterios técnicos adoptados; no atribuye al compañero acuerdos que no constan en los documentos. Se utilizó ChatGPT (GPT-6) como apoyo para organizar el borrador, clasificaciones, métricas y LaTeX; las referencias se contrastaron con el material académico y las fichas bibliográficas.

Según la indicación comunicada para cuarto «B», el trabajo se publica en GitHub y se presenta una carátula informativa de una página en el SGA hasta el sábado 7 de noviembre de 2026, 23:59.
