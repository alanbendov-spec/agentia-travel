# agentia. — concierge de viajes boutique

Recuperado el 2026-08-02 desde los artifacts publicados en claude.ai.
La sesión original de Claude Desktop ("Premium boutique travel agency automation",
13-jul-2026) quedó sin transcripción — el trabajo real vivía en los artifacts.

## Qué es

Agencia de viajes premium boutique operada como **agente independiente afiliado a
Archer Travel Service, Inc. (Evolution Travel)**. El diferencial es un concierge
conversacional ("AGENTIA", sobre Anthropic) que arma el itinerario en tiempo real
y luego verifica y reserva todo en 48 horas.

- **Modelo de negocio**: membresía mensual (cancela cuando quieras). La membresía
  paga el servicio; los viajes se pagan aparte con precio final a la vista y
  tarifas de red mayorista.
- **Promesa**: "La mayoría de las agencias desaparece cuando pagas. Para nosotros
  ahí empieza lo importante." Soporte 7 días en viaje, reclamos, reembolsos,
  millas y perfil de viajero que se afina con cada viaje.
- **Mercado**: Chile / LATAM (salidas SCL) + EE.UU. Sitio bilingüe ES/EN.
- **Credenciales mostradas**: agente independiente autorizado, red mayorista de
  proveedores, acreditación Archer, CLIA (cruceros).

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | Landing bilingüe con demo interactiva del chat + itinerario que se arma en vivo (Tokio/Kioto, Atenas/Santorini, NYC). Single-file, fuentes embebidas. |
| `setup-guide.html` | Guía operativa: dominio, correo corporativo, conexión con Archer/Evolution, deploy y checklist pre-lanzamiento. |
| `assets/` | Logos Evolution Travel. |

## Estado y pendientes (del setup guide)

Nada de esto está hecho todavía — es la lista de arranque:

1. Comprar dominio — recomendado `agentia.travel` (fallbacks: `agentia.com`,
   `tryagentia.com`, `agentia.io`). Auto-renew + WHOIS privacy.
2. Google Workspace (~USD 7/usuario/mes): `hello@`, `reservations@`, `support@`.
3. Actualizar la cuenta Archer/Evolution a `reservations@…` en Back Office, en
   cada portal de proveedor y en EvoTravelAgent.com. Agregar
   `HI@myworkmarket.com` a remitentes seguros (avisos de comisión ADP/WorkMarket).
   **El orden importa**: dominio → correo → registro en Archer.
4. Deploy en Vercel + dominio propio.
5. Precio de membresía definido + links de pago Stripe, WhatsApp Business,
   Calendly, y Privacy Policy / ToS revisados por abogado.

Costo estimado de arranque: ~USD 20–35/año dominio + ~USD 7/usuario/mes correo.

## Artifacts originales

- Landing: https://claude.ai/code/artifact/618cad3e-00b8-498f-84cd-bb8b4f182a48
- Setup guide: https://claude.ai/code/artifact/7811c4f7-9078-404c-9e6d-4c908d66b2a0
- Preview previo (13-jul): https://claude.ai/code/artifact/e683d4f3-f542-4222-8bd1-271129d998cc
