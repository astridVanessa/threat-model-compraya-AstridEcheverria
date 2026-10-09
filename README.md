# Modelo de amenazas - CompraYa (Tienda en línea)

Repositorio del modelo de amenazas de la plataforma de comercio electrónico **CompraYa** (caso académico ficticio), elaborado con **OWASP Threat Dragon v2** y la metodología **STRIDE por elemento**.

## Estructura

| Archivo | Contenido |
|---|---|
| `compraya-threat-model.json` | Proyecto de OWASP Threat Dragon (formato v2.3): 3 diagramas y 33 amenazas STRIDE |
| `DFD-N0-contexto.png` | DFD Nivel 0 exportado (contexto) |
| `DFD-N1-procesos.png` | DFD Nivel 1 exportado (procesos, almacenes, flujos y trust boundaries) |
| `DFD-N2-checkout-pago.png` | DFD Nivel 2 exportado (checkout y pago con tarjeta) |
| `01-DFD-Nivel0-Contexto.png` | Captura del DFD Nivel 0 en Threat Dragon v2.6.2 |
| `02-DFD-Nivel1-Procesos.png` | Captura del DFD Nivel 1 en Threat Dragon v2.6.2 |
| `03-DFD-Nivel2-Checkout-Pago.png` | Captura del DFD Nivel 2 en Threat Dragon v2.6.2 |
| `04-Modelo-importado.png` | Captura del modelo importado en Threat Dragon |
| `05-Reporte-resumen-amenazas.png` | Captura del resumen del reporte de amenazas |
| `CHANGELOG.md` | Historial de versiones del modelo |

## Cómo abrir el modelo

1. Abrir OWASP Threat Dragon (escritorio o https://www.threatdragon.com).
2. Elegir **Open an existing threat model → Import** y seleccionar `compraya-threat-model.json`.
3. El modelo contiene 3 diagramas (Nivel 0, 1 y 2) y 33 amenazas STRIDE asociadas a procesos, almacenes y flujos.
4. Para exportar capturas: abrir cada diagrama y usar **Export → PNG/SVG**; para el reporte, **Report → Print/PDF**.

## Versionado

- Cada cambio del modelo se registra en `CHANGELOG.md` y se etiqueta en Git (`git tag v1.0`).
- Convención: `MAYOR.MENOR` — MAYOR cambia con nuevos componentes o rediseños; MENOR con nuevas amenazas o ajustes de riesgo.
- El modelo se revisa en cada release o cambio de arquitectura (integración al SSDLC).

```bash
git init && git add . && git commit -m "Modelo de amenazas CompraYa v1.0"
git tag v1.0
git remote add origin <URL-de-tu-repositorio> && git push -u origin main --tags
```
