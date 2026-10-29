# Bodega Naturisa — Balanceado

Pantalla web de las bodegas de balanceado: saldos SAP en vivo, saldo y plan de AP1, despachos de proveedor por ingresar
y sugerido de ingreso por día. Reemplaza los Excel REPORTE ISLAS, Balanceado y Planificación 701.

## Secciones
- **Balanceado** — matriz bodega × tipo de balanceado: stock SAP, cuadre con AP1 (✓/✗) y hasta cuándo alcanza según el plan.
- **Reporte** — sacos y días de cobertura por campamento, ocupación de la bodega y montacargas; se copia como imagen para WhatsApp.
- **Planificado** — plan y consumo real de AP1 por semana (3 atrás, la presente y 1 adelante) con stock, ingresos y saldo al domingo.
- **Sugerido ingreso** — ingreso sugerido por día hasta el domingo de la semana siguiente según plan (o consumo promedio de 7 días),
  cobertura mínima/objetivo, capacidad de la bodega, gabarras completas en islas (Cargill y Haid por separado) y sin carga el domingo; editable.
- **Configuración** — capacidad en pallets, montacargas, sector y notas por bodega (D1, se guarda con el usuario AP1).

## Uso
Requiere Python 3. Doble clic en `bodega/iniciar-bodega.bat` (abre http://localhost:3011).
El ingreso es con el usuario y contraseña de AP1. `comun/server.py` hace de proxy local al gateway de Naturisa.
