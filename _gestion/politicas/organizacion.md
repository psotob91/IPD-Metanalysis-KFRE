# Política de organización de carpetas y archivos

## Estructura
```
IPD-Metanalysis-KFRE/
├── CLAUDE.md                     # instrucciones y memoria de entrada
├── protocol-ipd-kfre-v2.docx     # entregable vigente
├── protocol-ipd-kfre-v1.docx     # histórico (no editar)
├── maestros/                     # 01–05 metodología (fuente de verdad)
├── _gestion/
│   ├── INDICE_MAESTROS.md        # mapa navegable
│   ├── MEMORIA.md                # decisiones + referencias verificadas
│   └── politicas/                # anti-drift, anti-alucinación, anti-sesgos, tokens, organización
└── bibliografía-previsa/         # NO usar (archivo muerto)
```

## Reglas
1. **Versionado explícito**: `protocol-ipd-kfre-vN.docx`. Nunca sobrescribir una versión previa;
   crear la siguiente y anotar el cambio en `MEMORIA.md`.
2. **Nombres**: minúsculas, sin espacios, con guiones. Prefijo numérico para orden (`01_…`).
3. **Separar gestión de contenido**: metadatos y políticas en `_gestion/`; contenido en `maestros/`
   y en los `.docx`.
4. **No tocar** `bibliografía-previsa/` ni `protocol-ipd-kfre-v1.docx`.
5. **Entregables finales** siempre en la raíz del proyecto, visibles para el usuario.
6. Archivos temporales/scratch fuera del proyecto; solo el resultado final se guarda aquí.
