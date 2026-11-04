# TA-IND-01 — Actividad Autónoma 1: Caso GAD cantonal

**Asignatura:** Ingeniería de Requisitos (ISR-401)  
**Estudiante:** Cedeño Avila Winston Damian  
**Carrera:** Ingeniería de Software — cuarto nivel, paralelo B  
**Universidad:** Universidad Técnica Estatal de Quevedo (UTEQ)

## Tema

Propuesta de requisitos para un sistema de cobro de impuestos prediales en línea de un GAD cantonal, con conexión a una pasarela local y una posible integración autorizada con el SRI.

## Estado del documento

**Tercer avance técnico (3 de noviembre de 2026) — borrador en revisión.**

Se conservan el alcance del caso, las seis partes interesadas, los cinco requisitos funcionales (RF) y los cinco requisitos no funcionales (RNF) cuantificados del avance anterior. En esta revisión se agregan **tres restricciones, dos dependencias justificadas y una matriz de trazabilidad** que conecta actores, requisitos y comprobaciones previstas.

Las reglas y las metas de rendimiento, disponibilidad, seguridad, interacción e interoperabilidad son propuestas para un ejercicio académico. **No son datos oficiales ni pruebas realizadas en un GAD.** La integración con el SRI se plantea condicionada a un servicio autorizado y la existencia de un convenio aplicable.

## Archivos

| Archivo | Descripción |
|---|---|
| `actividad_autonoma_1.tex` | Fuente LaTeX del tercer avance. |
| `referencias.bib` | Bibliografía en formato IEEE, procesada con `biblatex`/`biber`. |
| `actividad_autonoma_1.pdf` | PDF compilado a partir de la misma fuente. |
| `README.md` | Descripción del avance e instrucciones de compilación. |

## Cómo compilar

Instalar MiKTeX o TeX Live con `pdflatex`, `biber`, `IEEEtran`, `babel`, `lmodern`, `microtype`, `csquotes`, `booktabs`, `tabularx`, `array`, `enumitem`, `needspace`, `hyperref`, `biblatex` y `biblatex-ieee`.

Desde la carpeta `TA-IND-01` ejecutar:

```bash
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
biber actividad_autonoma_1
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
pdflatex -interaction=nonstopmode -halt-on-error actividad_autonoma_1.tex
```

Después de modificar la fuente, regenerar el PDF antes de publicarlo.

## Referencias y declaración de IA

- [ISO/IEC/IEEE 29148:2018](https://www.iso.org/standard/72089.html): ingeniería de requisitos.
- [ISO/IEC 25010:2023](https://www.iso.org/standard/78176.html): modelo de calidad de producto con nueve características.

ChatGPT (OpenAI, GPT-6) ha colaborado en la preparación y organización del borrador técnico, la redacción de ejemplos y el soporte LaTeX. El estudiante debe estudiar, revisar y, cuando corresponda, corregir el contenido antes de presentarlo como trabajo propio. No se atribuyen entrevistas, contratos, pruebas ejecutadas ni datos municipales inexistentes.

## Pendiente para el cierre

Revisión individual de los requisitos, las relaciones y las citas; confirmación del enunciado publicado en el SGA; compilación final desde una copia limpia del repositorio; y portada del SGA con la URL pública. El cierre señalado por el encuadre para TA-IND-01 es **7 de noviembre de 2026 a las 23:59**.
