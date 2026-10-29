# Tasterush — Next.js Storefront Starter

A responsive digital-products storefront starter built with Next.js App Router, TypeScript, and Tailwind CSS.

## Important status

- This is a **demo storefront**. The product catalog is sample data.
- No checkout, payment processing, digital file delivery, admin authentication, or Shopify integration is implemented yet.
- Product CTAs intentionally point to product detail pages; they do not claim a purchase succeeded.
- Replace demo product details, contact details, and policy copy with accurate business information before publishing.
- The policy pages are starter templates, not legal advice.

## Requirements

- Node.js 18.17+ (Node.js 20 LTS recommended)
- npm

## Run locally

```bash
npm install
npm run dev
```

Open http://localhost:3000.

## Production build

```bash
npm run build
npm start
```

## Pages

- `/` — Homepage
- `/products` — Demo product listing
- `/products/creative-starter-kit` — Product detail
- `/products/content-planner` — Product detail
- `/products/social-media-toolkit` — Product detail
- `/faq`
- `/contact`
- `/privacy`
- `/refunds`
- `/terms`

## Deploy to Vercel

1. Push this project to a GitHub repository.
2. In Vercel, select **Add New → Project** and import the repository.
3. Keep the framework preset as Next.js.
4. No environment variables are required for this demo.
5. Deploy and test the generated `.vercel.app` URL.
6. Connect `tasterush.store` only after testing the new site and deciding how to handle the existing Shopify store/domain.

## Before going live

1. Replace sample products and prices with accurate product data.
2. Add real product artwork and delivery details.
3. Update policy pages and contact information.
4. Integrate a supported checkout/payment provider securely.
5. Implement verified payment webhooks and secure digital delivery.
6. If adding an admin panel, implement server-side authentication, authorization, and database security.
7. Test checkout, mobile layouts, links, and accessibility.

## Structure

```text
app/
  faq/page.tsx
  contact/page.tsx
  privacy/page.tsx
  refunds/page.tsx
  terms/page.tsx
  products/[slug]/page.tsx
  products/page.tsx
  globals.css
  layout.tsx
  page.tsx
components/
  footer.tsx
  header.tsx
  product-card.tsx
lib/
  products.ts
```
