# Modelo de amenazas - CompraYa (Tienda en línea)

Repositorio del modelo de amenazas de la plataforma de comercio electrónico **CompraYa** (caso académico ficticio), elaborado con **OWASP Threat Dragon v2** y la metodología **STRIDE por elemento**.

## Estructura

```
threat-model-compraya/
├── README.md
├── CHANGELOG.md
├── model/
│   └── compraya-threat-model.json        # Proyecto OWASP Threat Dragon (v2.3)
├── diagrams/
│   ├── DFD-N0-contexto.png / .svg
│   ├── DFD-N1-procesos.png / .svg
│   ├── DFD-N2-checkout-pago.png / .svg
│   └── capturas-threat-dragon/           # Capturas tomadas en Threat Dragon v2.6.2
│       ├── 01-DFD-Nivel0-Contexto.png
│       ├── 02-DFD-Nivel1-Procesos.png
│       ├── 03-DFD-Nivel2-Checkout-Pago.png
│       ├── 04-Modelo-importado.png
│       └── 05-Reporte-resumen-amenazas.png
└── docs/
    └── Tarea2_Modelo_Amenazas_CompraYa.docx   # Informe (reemplazar por el PDF final)
```

## Cómo abrir el modelo

1. Abrir OWASP Threat Dragon (escritorio o https://www.threatdragon.com).
2. Elegir **Open an existing threat model → Import** y seleccionar `model/compraya-threat-model.json`.
3. El modelo contiene 3 diagramas (Nivel 0, 1 y 2) y 33 amenazas STRIDE asociadas a procesos, almacenes y flujos.
4. Para exportar capturas: abrir cada diagrama y usar **Export → PNG/SVG**; para el reporte, **Report → Print/PDF**.

## Versionado

- Cada cambio del modelo se registra en `CHANGELOG.md` y se etiqueta en Git (`git tag v1.0`).
- Convención: `MAYOR.MENOR` — MAYOR cambia con nuevos componentes o rediseños; MENOR con nuevas amenazas o ajustes de riesgo.
- El modelo se revisa en cada release o cambio de arquitectura (integración al SSDLC).

Agregar aquí el PDF del informe y el reporte PDF de Threat Dragon en la carpeta `docs/` antes de publicar.

```bash
git init && git add . && git commit -m "Modelo de amenazas CompraYa v1.0"
git tag v1.0
git remote add origin <URL-de-tu-repositorio> && git push -u origin main --tags
```
