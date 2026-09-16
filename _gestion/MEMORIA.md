# Memoria del proyecto

## Estado
- **2026-07-16**: Configurado scaffolding (CLAUDE.md, índice, políticas). Creado
  `protocol-ipd-kfre-v2.docx`: versión limpia, sin marcadores `(REF)`, con citas
  Vancouver numeradas (15 referencias verificadas).
- **2026-07-16**: Creado `protocol-ipd-kfre-v3.docx` — **entregable vigente**. Añade:
  ética descentralizada (comité que cada site elija; aprobación previa a compartir datos);
  anonimización (seudonimización SHA-256 + HMAC/sal en origen, trazabilidad intra-cohorte,
  PPRL con filtros de Bloom [ref 16]); países Chile/Perú/Uruguay + invitación por correo a
  Colombia; sección de gobernanza (Comité de Dirección en marco SLANH; Perú=centro coordinador
  de datos); aspectos administrativos (cronograma 24 meses + presupuesto fondo UPN ~S/20 000
  ≈ USD 5 900). 16 referencias. 3 tablas.

- **2026-07-16**: Creado `protocol-ipd-kfre-v4.docx` — **entregable vigente**. Añade:
  encuadre explícito como **epidemiología clínica / prevención secundaria** (base legal del waiver);
  **solicitud de exención de consentimiento** con 6 criterios (impracticabilidad, valor social,
  riesgo mínimo, privacidad, no afectación de derechos, decisión del comité); tabla de **marco
  normativo por país** (Perú Ley 29733; Chile Ley 20.120 y 19.628; Uruguay Ley 18.331 y Decreto
  158/019); armonización según **Maelstrom** + calidad **Kahn** (conformidad/completitud/plausibilidad);
  gobernanza ampliada (dupla investigador de sitio + coordinador de sitio, según CaTaLiNA);
  **Figuras 1 y 2** (flujogramas ISO 5807, páginas horizontales) y **Figuras 3-5** (Gantt por país:
  Perú 1 mes ética, Uruguay y Chile 3 meses). 21 referencias, numeración automática por orden
  de aparición. Fuentes de figuras en `figuras/` (.png + .mmd mermaid).

- **2026-09-14**: Creado `protocol-ipd-kfre-v5.docx` a partir de `protocol-ipd-kfre-comprtir-final.docx`
  (sin tocar el resto del texto). Añade sección **Operacionalizacion de variables** (tras Criterios de
  elegibilidad) adaptada de refs 5 y 8 (EsSalud): KFRE 4 variables no norteamericano (S0 2a=0,9832; 5a=0,9365),
  CKD-EPI 2009 sin raza (2021 en sensibilidad), ACR mg/g winsorizado p1,5-p98,5, falla renal por registro de
  diálisis/CIE-10 (N18.5, N18.6, Z49.1, Z49.2, Z99.2, Z94.0), muerte SINADEF/RENIEC. **Tabla 1** (variables de
  paciente) y **Tabla 2** (jerarquía geográfica/administrativa por país: ubigeo/CUT/INE, red EsSalud/Servicio de
  Salud/prestador SNIS, IPRESS/DEIS, nivel de atención, subsector). Tablas previas renumeradas 1→3 y 2→4.
  Sin referencias nuevas.

## Decisiones clave
- **Flexibilidad operativa (v5, pedido del investigador)**: las definiciones de los estudios peruanos son de
  *referencia*; NO fijar a priori ventanas creatinina–ACR, tipo de muestra urinaria, exclusión de uPCR/tira,
  winsorización, transferencia de fechas ni códigos de comorbilidad. Se identifican en el perfilado de cada base,
  se deciden tras verlo, se documentan en el diccionario común y se evalúan en sensibilidad. Priorizar incluir
  cohortes con variaciones razonables. Correspondencias Chile/Uruguay de Tabla 2 son candidatas.
- Guía de reporte: **TRIPOD-Cluster** (diseño de datos agrupados) + **PRISMA-IPD** (búsqueda).
- KFRE de **4 variables**, horizontes 2 y 5 años. Validación estricta con coeficientes originales antes de recalibrar.
- Análisis IPD en **dos etapas** (transportabilidad + heterogeneidad); una etapa como sensibilidad.
- Calibración jerárquica (in-the-large / débil / moderada) + **DCA** para utilidad clínica.
- Riesgo competitivo (muerte) incorporado explícitamente.

## Lista maestra de referencias (Vancouver, verificadas — DOI/PMID)
Obligatorias del encargo marcadas con ★.
1. Tangri N, et al. JAMA. 2011;305(15):1553-9. PMID 21482743 — KFRE original.
2. Tangri N, et al. JAMA. 2016;315(2):164-74. PMID 26757465 — KFRE multinacional (IPD).
3. Collins GS, et al. BMJ. 2015;350:g7594. PMID 25569120 — TRIPOD.
4. ★ Bravo-Zúñiga J, Chávez-Gómez R, Soto-Becerra P. BMJ Open. 2024;14(1):e076217. PMID 38184316 (PMC10773413).
5. ★ Larrarte C, et al. Int J Nephrol. 2024;2024:1282664. PMID 38405300 — Colombia.
6. ★ WCN24-1069, Uruguay. Kidney Int Rep. 2024;9(4 Suppl). PII S2468-0249(24)00273-0.
7. ★ Bravo-Zúñiga J, Soto-Becerra P, et al. BMC Nephrol. 2025;26(1):688. — biomedcentral 1471-2369/26/688.
8. Riley RD, et al. BMJ. 2016;353:i3140. PMID 27334381 — validación externa big data/IPD.
9. Debray TPA, et al. BMJ. 2023;380:e071018. PMID 36750242 — TRIPOD-Cluster checklist.
10. Debray TPA, et al. BMJ. 2023;380:e071058. PMID 36750236 — TRIPOD-Cluster E&E.
11. Vickers AJ, Elkin EB. Med Decis Making. 2006;26(6):565-74. PMID 17099194 — DCA.
12. Van Calster B, et al. J Clin Epidemiol. 2016;74:167-76. PMID 26772608 — jerarquía de calibración.
13. Wolff RF, et al. Ann Intern Med. 2019;170(1):51-8. PMID 30596875 — PROBAST.
14. Milders J, et al. J Am Soc Nephrol. 2024;35(3):367-80. PMID 38082484 — scoping review nefrología.
15. Hahn Lundström U, et al. Nephrol Dial Transplant. 2024;39(12):2079-87. PMID 38486367 — KFRE acceso vascular.
16. Schnell R, Bachteler T, Reiher J. Privacy-preserving record linkage using Bloom filters. BMC Med Inform Decis Mak. 2009;9:41. PMID 19706187 — PPRL/seudonimización.
17. Fortier I, et al. Maelstrom Research guidelines for rigorous retrospective data harmonization. Int J Epidemiol. 2017;46(1):103-5. PMID 27272186 — armonización retrospectiva (5 pasos).
18. Kahn MG, et al. A harmonized data quality assessment terminology and framework for the secondary use of EHR data. EGEMS. 2016;4(1):1244. PMID 27713905 — conformidad/completitud/plausibilidad.
19. Tassé AM, Kirby E, Fortier I. Developing an ethical and legal interoperability assessment process for retrospective studies. Biopreserv Biobank. 2016;14(3):249-55. PMID 27115199 — waiver e interoperabilidad ético-legal.
20. Solis Pazmino P, et al. (CaTaLiNA). BMJ Open. 2025;15(6):e093471. PMID 40545306 — red multipaís LatAm; Percy es coautor (estadístico).
21. ISO 5807:1985 — simbología de diagramas de flujo.

## Nota sobre figuras
- Mermaid se validó OK, pero no se puede rasterizar aquí (puppeteer/Chromium bloqueado; cairosvg no
  soporta foreignObject). Las figuras del docx se renderizan con **Graphviz** (ISO 5807, alta resolución);
  las fuentes **mermaid equivalentes** están en `figuras/*.mmd` por si se prefieren.
- Ancho natural de los flujogramas ~31-34 cm → van en **páginas horizontales** (texto efectivo ~7-8 pt).

## Por verificar / pendientes (para v3)
- Referencia de carga epidemiológica de ERC (GBD) — aún no citada; conseguir cita verificada.
- PRISMA-IPD (Stewart LA, et al. JAMA 2015) — mencionada en prosa; añadir cita numerada verificada.
- Sample size: Riley/Snell 2021 (validación externa) — añadir cita específica si se desea.
