# Clear Harvest Market

Upgraded website and commerce-first first pass for **Clear Harvest Market** in Truckee / Lake Tahoe.

This version preserves and builds on the current live brand footprint:
- existing business name and positioning
- Truckee, California focus
- cold-pressed juice
- artisan sourdough and fresh baked goods
- phone number and social channels
- Hotplate ordering path

## Pages
- `index.html` — premium homepage with Tahoe/Truckee visitor messaging
- `order.html` — stronger ordering hub with Hotplate, preorders, bundles, and product categories
- `recipes.html` — $1 recipe shop and recipe micro-products
- `partners.html` — catering, hiring, local vendor, retail shelf, and business partnerships
- `about.html` — fuller family brand story
- `juice.html` — expanded live-menu juice page
- `contact-us.html` — cleaner contact and routing page
- `checkout.html` — general checkout scaffold for future store use
- `thank-you.html` — post-purchase / follow-up page
- `admin/index.html` — owner admin dashboard
- `superadmin/index.html` — top-level superadmin dashboard

## APIs
- `api/create-checkout-session.js` — cart-based Stripe scaffold
- `api/create-recipe-checkout.js` — simple $1 recipe product checkout scaffold
- `api/send-order-email.js` — order follow-up scaffold
- `api/send-vendor-inquiry.js` — partner / hiring / vendor inquiry scaffold
- `api/subscribe.js` — newsletter and opening updates scaffold
- `api/admin-status.js` — admin package status/config feed
- `api/admin-session.js` — admin/superadmin role-check scaffold
- `api/marketing-command.js` — marketing automation action router scaffold
- `api/lead-intake.js` — lead classification and funnel recommendation scaffold

## Real brand details integrated
- Phone: `530-813-5262`
- Facebook: `https://www.facebook.com/clearharvestmarket`
- Instagram: `https://www.instagram.com/clearharvestmarket`
- TikTok: `https://www.tiktok.com/@clearharvestmarket`
- Current external ordering path: `https://www.hotplate.com/clearharvest/52863552-bd03-4edc-a29d-1bc4e35894e5`

## What this build adds
- stronger Tahoe / Truckee visitor-friendly copy
- richer market, bakery, and juice merchandising
- local-travel content framing for visitors entering the basin
- recipe shop with $1 recipe micro-checkout concept
- better partner / vendor / catering growth lanes
- stronger setup notes for long-term success, not just a contact form
- admin/superadmin marketing package scaffolding
- role-based automation model for campaigns, SEO, video, autoposting, lead gen, funnels, and payments
- config + API structure ready for deeper backend integration
