# TA-IND-01 / TA-TAR-01 — Banca Móvil Banco Guayaquil

**Asignatura:** Ingeniería de Requerimientos (ISR-401)  
**Estudiante:** Cedeño Avila Winston Damian  
**Nivel y paralelo:** 4.º "B" — UTEQ  
**Sistema elegido:** App Banco Guayaquil, aplicación de banca móvil.  
**Estado:** Borrador académico. **Faltan tres capturas auténticas del estudiante y la confirmación del registro del sistema en el foro del SGA.**

## Contenido

El documento analiza los fundamentos de la norma ISO/IEC/IEEE 29148:2018 y aplica la clasificación de calidad ISO/IEC 25010:2023 al caso de la App Banco Guayaquil. Incluye resumen analítico de las cláusulas 5.2.4–5.2.7, glosario de diez términos de la cláusula 3, quince requisitos distribuidos en cinco tipos, una tabla de clasificación y aceptación, autoevaluación con versiones anterior y corregida y reflexión crítica.

**Alcance:** los flujos observables de saldo, movimientos, beneficiarios, transferencias y comprobantes se apoyan en documentación pública del banco. La arquitectura interna, respuestas de las API y los umbrales de calidad son propuestas académicas que requieren validación; no son mediciones ni afirmaciones oficiales del banco.

## Archivos

- `main.tex`: fuente editable y archivo principal del informe.
- `main.pdf`: compilación reproducible del informe (6 páginas en el borrador actual).
- `referencias.bib`: fuentes verificables en formato IEEE mediante `biblatex`/`biber`.
- `figuras/captura_inicio.png`: evidencia propia de inicio o consulta, sin datos privados (**pendiente**).
- `figuras/captura_transferencia.png`: evidencia propia del acceso a Transferir/Pagos (**pendiente**).
- `figuras/captura_comprobantes.png`: evidencia propia de la ruta de comprobantes (**pendiente**).
- `figuras/README.md`: indicaciones para preparar las evidencias.

> El código contiene controles `\IfFileExists`: cuando una figura no existe, aparece una caja identificada como **CAPTURA PROPIA PENDIENTE**. Eso permite revisar el borrador, pero **no equivale a entregar las tres capturas exigidas**. Después de añadirlas hay que recompilar `main.pdf`.

## Compilación desde el repositorio

Instalar **TeX Live** o **MiKTeX**, con `pdfLaTeX`, `biber`, la clase `IEEEtran` y los paquetes `babel` (español), `lmodern`, `microtype`, `csquotes`, `graphicx`, `booktabs`, `tabularx`, `array`, `xcolor`, `biblatex` con estilo `ieee`, `hyperref` y `needspace`.

En una consola, situarse en `TA-IND-01` y ejecutar exactamente:

```bash
pdflatex -interaction=nonstopmode -halt-on-error main.tex
biber main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

El PDF de la versión preparada compila sin referencias faltantes. Los tres PNG deben permanecer con esos nombres y dentro de `figuras/` para incorporarse de forma automática. Se debe revisar que el documento compilado definitivo permanezca entre 4 y 7 páginas de contenido.

## Material y limitaciones

- Normas: ISO/IEC/IEEE 29148:2018 e ISO/IEC 25010:2023.
- Libro: Klaus Pohl, *Requirements Engineering*, 2.ª ed., Springer, 2025.
- Manual: *SWEBOK Guide*, v4.0, IEEE Computer Society, 2024.
- Ayuda y comunicaciones oficiales de Banco Guayaquil (consultar `referencias.bib`).

La app puede mostrar recorridos distintos según versión y sistema operativo; los apartados de la interfaz deben comprobarse con el dispositivo realmente observado. No se usan datos bancarios de terceros ni se publican contraseñas, códigos SMS, saldos, números de cuenta o transacciones identificables.

## Integridad académica

Se utilizó ChatGPT (OpenAI, GPT-6) para apoyar la redacción, clasificación y edición LaTeX. Las fuentes normativas se contrastaron con la documentación citada y las funcionalidades visibles con ayuda oficial del banco. Los requisitos se presentan como **propuestas**, no como resultados obtenidos mediante pruebas. La redacción, reflexión y evidencia visual deben ser revisadas y completadas por el estudiante antes de la entrega.

## Entrega al SGA

La guía indica subir al SGA **solo una carátula PDF de una página** con nombre, tarea, plazo y URL pública completa en una línea. El informe, fuentes y evidencias van en este repositorio. **Fecha de cierre indicada por la guía: 7 de noviembre de 2026, 23:59** (verificar cualquier prórroga con el docente).
