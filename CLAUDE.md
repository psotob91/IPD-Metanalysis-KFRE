# CLAUDE.md — Proyecto IPD Meta-analysis KFRE

## Qué es este proyecto
Redacción del **protocolo de investigación** de un meta-análisis con datos individuales
de participantes (IPD-MA) para validar externamente, recalibrar y evaluar la utilidad
clínica del **Kidney Failure Risk Equation (KFRE)** en América Latina. Diseño de datos
agrupados (clustered) → guía de reporte de referencia: **TRIPOD-Cluster** + **PRISMA-IPD**.

## Investigador
Percy Soto-Becerra (UPN) — autor de la evidencia peruana previa (BMJ Open 2024; BMC Nephrol 2025).

## Estructura de carpetas
- `protocol-ipd-kfre-v5.docx` — **entregable vigente**: `comprtir-final` + sección de operacionalización de variables (Tablas 1-2).
- `protocol-ipd-kfre-comprtir-final.docx` — versión compartida previa a v5. Histórico.
- `protocol-ipd-kfre-v4.docx` — waiver, encuadre epidemiológico, figuras, Gantt por país. Histórico.
- `figuras/` — figuras del protocolo: `.png` (Graphviz, ISO 5807) + `.mmd` (fuentes mermaid).
- `protocol-ipd-kfre-v3.docx` — versión previa (ética, anonimización, gobernanza, admin). Histórico.
- `protocol-ipd-kfre-v2.docx` — versión previa limpia con citas Vancouver. Histórico.
- `protocol-ipd-kfre-v1.docx` — versión previa con marcadores `(REF)`. NO editar; es histórico.
- `maestros/` — 5 documentos maestros de metodología. Fuente de verdad del contenido. Ver índice.
- `_gestion/` — memoria, índice navegable y políticas de trabajo.
- `bibliografía-previsa/` — **NO revisar**. Archivo muerto, no se usa.

## Reglas rápidas de trabajo
1. **Contenido primero**: el sustento metodológico vive en `maestros/`. Cítalos antes de redactar.
2. **Citas**: estilo **Vancouver numerado**, en orden de aparición. Ver `_gestion/MEMORIA.md`
   para la lista maestra de referencias verificadas (con DOI/PMID).
3. **No inventar referencias**. Toda cita debe estar verificada vía PubMed/Crossref. Si no se
   puede verificar, no se numera (ver `politicas/anti-alucinacion.md`).
4. **Nomenclatura de versiones**: `protocol-ipd-kfre-vN.docx`. No sobrescribir versiones previas.
5. Antes de una tarea multi-paso: revisar `_gestion/politicas/` (anti-drift, anti-sesgos, tokens).

## Índice de navegación
- Mapa de los maestros → `_gestion/INDICE_MAESTROS.md`
- Memoria del proyecto (decisiones + refs) → `_gestion/MEMORIA.md`
- Políticas → `_gestion/politicas/`
