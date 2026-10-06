# Freelance work

Two systems I built as a solo developer in 2026. Both are live, with Arabic right-to-left interfaces.

## Registration and payments platform

For a community association. People sign up for its programs and pay online, and staff approve registrations from an admin panel.

- Payments go through a Saudi bank's hosted checkout.
- Every payment and status change is recorded in an audit log.
- Automated tests check the database access rules for each type of user.

Next.js, TypeScript, Supabase, PostgreSQL, Vercel, Vitest, Playwright

## Finance platform

For an education consultancy. Staff request cash advances, attach invoices as they spend, and close each advance when it's settled. The accountant reviews the records and exports reports to Excel and PDF.

- Invoices with a ZATCA QR code are decoded directly. For the rest, a vision model reads the image, and any field it isn't sure of is flagged for the accountant.
- I chose the vision model by testing three models on real invoices, and ruled one out because it gave confident values for an invoice that couldn't be read.

Next.js, TypeScript, Supabase, PostgreSQL, Vercel
