# Grandora Hotel OS — Frontend Working Demo

A polished frontend-only hotel and restaurant management demo built for live sales presentations to large hotels.

## Demo modules

- Hotel overview dashboard
- Reservations and guest check-in queue
- Room status board
- Table-wise QR ordering
- Customer WhatsApp-number capture
- Digital restaurant menu, cart and reorder flow
- Online payment / pay-at-counter simulation
- Restaurant order management
- Kitchen Display System (KDS)
- Billing and POS demo
- Housekeeping board
- Inventory
- Staff and shifts
- Reports and analytics
- Hotel settings and production integration roadmap

## Customer QR flow

1. Open **Table QR** in the hotel dashboard.
2. Each table gets its own QR/link, for example `order.html?table=T12`.
3. Customer enters a 10-digit WhatsApp number and optional name.
4. Customer adds dishes to cart and places the order.
5. Customer chooses **Online payment** or **Pay at table/counter**.
6. Online payment is simulated in the frontend demo.
7. The order is stored in browser `localStorage` and appears in Orders, Kitchen and Billing when both pages are used in the same browser/origin.
8. Customer can order more from the same table.

The dashboard renders table QR images dynamically using a public QR image endpoint. For an offline sales demo, use the **Open** table button instead of scanning.

## Run locally

No build tools or packages are required.

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

Customer flow example: `http://localhost:8080/order.html?table=T12`.

## Demo data

The app stores demo state in browser `localStorage`. **Reset demo** restores seeded hotel data.

Because this version is frontend-only, different phones/laptops do not share realtime order state. The production version should use a realtime backend such as Supabase/PostgreSQL.

## Production integrations planned

- Supabase/PostgreSQL realtime backend and row-level permissions
- Secure staff authentication and audit logs
- WhatsApp Cloud API for order confirmations, payment links, invoices and feedback
- Razorpay/Cashfree/UPI payment flow with webhook verification
- Permanent QR URLs per restaurant table
- KOT / thermal printer integration
- PMS, OTA and channel-manager integration where required
- Multi-property support, cloud backup and analytics

## Deployment

The project is static and can be deployed directly on GitHub Pages, Netlify, Cloudflare Pages or any static hosting service.

---

Demo concept prepared for ITCYBER TECHNOLOGIES PVT LTD.
