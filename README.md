# Grandora Hotel OS — Frontend Working Demo

A polished frontend-only hotel and restaurant management demo built for live sales presentations to large hotels.

## Demo modules

- Hotel overview dashboard
- Reservations and guest check-in queue
- Room status board
- Table QR ordering
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

## Run locally

No build tools or packages are required.

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

For the customer flow open `http://localhost:8080/order.html?table=T12`.

## Demo data

The app stores demo state in browser `localStorage`. The **Reset demo** button restores the seeded data.

Because this version is frontend-only, separate devices do not share live state. The production version should use Supabase/PostgreSQL or another realtime backend.

## Production integrations planned

- Supabase/PostgreSQL realtime backend and role-based access
- WhatsApp Cloud API for order confirmation, bills and feedback
- Razorpay/Cashfree payment links, UPI intent and webhook confirmation
- Real QR URLs per table
- Authentication, audit logs and staff permissions
- Printer/KOT integration
- PMS/OTA/channel manager integration where required

## GitHub Pages

The generated QR images target the expected GitHub Pages URL for a repository named `GrandHotel-Management-Demo` under the `kautukade` account. If you publish this exact repo with GitHub Pages, the table QR URLs can resolve to the customer-order page.

---

Demo concept prepared for ITCYBER TECHNOLOGIES PVT LTD.
