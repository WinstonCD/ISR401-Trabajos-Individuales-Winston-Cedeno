# TA-IND-01 / TA-TAR-01 — Banca Móvil Banco Guayaquil

**Asignatura:** Ingeniería de Requerimientos (ISR-401)  
**Estudiante:** Cedeño Avila Winston Damian  
**Nivel y paralelo:** 4.º "B" — UTEQ  
**Sistema elegido:** App Banco Guayaquil, aplicación de banca móvil.  
**Estado:** Versión revisada del informe, con tres figuras numeradas por separado. **Pendiente de confirmar en el SGA:** registro de la elección del sistema en el foro.

## Contenido

El documento analiza los fundamentos de la norma ISO/IEC/IEEE 29148:2018 y aplica la clasificación de calidad ISO/IEC 25010:2023 al caso de la App Banco Guayaquil. Incluye resumen analítico de las cláusulas 5.2.4–5.2.7, glosario de diez términos de la cláusula 3, quince requisitos distribuidos en cinco tipos, una tabla de clasificación y aceptación, autoevaluación con versiones anterior y corregida y reflexión crítica.

**Alcance:** los flujos observables de saldo, movimientos, beneficiarios, transferencias y comprobantes se apoyan en documentación pública del banco. La arquitectura interna, respuestas de las API y los umbrales de calidad son propuestas académicas que requieren validación; no son mediciones ni afirmaciones oficiales del banco.

## Archivos

- `main.tex`: fuente editable y archivo principal del informe.
- `main.pdf`: PDF compilado desde `main.tex`, con tres figuras independientes y siete páginas.
- `referencias.bib`: fuentes verificables en formato IEEE mediante `biblatex`/`biber`.
- `figuras/figura_01_inicio.jpg`: fotografía de la pantalla inicial, con datos privados ocultos.
- `figuras/figura_02_pagos.jpg`: fotografía del panel de pagos de servicios.
- `figuras/figura_03_movimientos.jpg`: fotografía del historial de movimientos, con datos financieros ocultos.

Las figuras están insertadas en `main.tex` por sus rutas relativas. El PDF se debe compilar con esas tres imágenes presentes en la carpeta `figuras/`.

## Compilación desde el repositorio

Instalar **TeX Live** o **MiKTeX**, con `pdfLaTeX`, `biber`, la clase `IEEEtran` y los paquetes `babel` (español), `lmodern`, `microtype`, `csquotes`, `graphicx`, `booktabs`, `tabularx`, `array`, `xcolor`, `biblatex` con estilo `ieee`, `hyperref` y `needspace`.

En una consola, situarse en `TA-IND-01` y ejecutar exactamente:

```bash
pdflatex -interaction=nonstopmode -halt-on-error main.tex
biber main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

El PDF de la versión preparada compila sin referencias faltantes. Las tres imágenes JPG deben conservar sus nombres y permanecer dentro de `figuras/` al compilar. La presente versión produce 7 páginas (rango de la guía: 4 a 7 páginas).

## Material y limitaciones

- Normas: ISO/IEC/IEEE 29148:2018 e ISO/IEC 25010:2023.
- Libro: Klaus Pohl, *Requirements Engineering*, 2.ª ed., Springer, 2025.
- Manual: *SWEBOK Guide*, v4.0, IEEE Computer Society, 2024.
- Ayuda y comunicaciones oficiales de Banco Guayaquil (consultar `referencias.bib`).

La app puede mostrar recorridos distintos según versión y sistema operativo; los apartados de la interfaz deben comprobarse con el dispositivo realmente observado. No se usan datos bancarios de terceros ni se publican contraseñas, códigos SMS, saldos, números de cuenta o transacciones identificables.

## Integridad académica

Se utilizó ChatGPT (OpenAI, GPT-6) para apoyar la redacción, clasificación y edición LaTeX. Las fuentes normativas se contrastaron con la documentación citada y las funcionalidades visibles con ayuda oficial del banco. Los requisitos se presentan como **propuestas**, no como resultados obtenidos mediante pruebas. La documentación distingue observaciones de interfaz, fuentes del banco y requisitos propuestos para un ejercicio académico; no se realizaron pruebas de infraestructura.

## Entrega al SGA

La guía indica subir al SGA **solo una carátula PDF de una página** con nombre, tarea, plazo y URL pública completa en una línea. El informe, fuentes y evidencias van en este repositorio. **Fecha de cierre indicada por la guía: 7 de noviembre de 2026, 23:59** (verificar cualquier prórroga con el docente).

## Evidencias fotográficas

Las fotografías aparecen como **Figura 1** (inicio), **Figura 2** (panel de pagos) y **Figura 3** (historial de movimientos), cada una con su pie de figura independiente. Los nombres y los importes sensibles se ocultaron antes de su incorporación. No constituyen pruebas de carga, disponibilidad ni seguridad del servicio.
