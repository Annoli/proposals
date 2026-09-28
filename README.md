# Proposal template: how to use it

## Make one for a new prospect (2 ways)
1. **Fastest:** host this once on Vercel, then add details to the link:
   `https://your-proposal.vercel.app/?company=Sunshine%20Roofing&short=Sunshine&city=Orlando&owner=Jake&ownerfull=Jake%20Smith&phone=(407)%20555-0100&domain=sunshineroofing.com&hero=IMAGE_URL&site=LIVE_SITE_URL`
2. **Per-client copy:** edit the `CONFIG` block at the top of `index.html` (client name, city, phone, hero image, prices) and deploy it as its own Vercel project.

`hero` = a screenshot of the site you built for them. If blank, a styled mock of their site is shown.

## On the sales call
- Open the link with `?rep=1` added (or press **Shift + E**) to show **Edit pricing** and **Undo**. The client never sees these buttons on their link.
- **Edit pricing** → pick a revenue preset (e.g. "$1M–$3M" = $15K setup, $10K one-time offer) or type your own numbers, set free bonus months, toggle paid add-ons → **Confirm**.
- When they ask about price or payment plans, click **See today's one-time offer**. It shows the discount, free months and total savings.
- They sign in the Client box and hit **Accept proposal**. Add your payment link in `CONFIG.paymentLink` to show a "Pay setup" button.

## Before your first call
- Swap the agency name/logo (`CONFIG.agency`). "Ironclad Contractor Agency" is a placeholder, so check the name and domain are free.
- Add your photo (`agency.photo`) and your terms link.
- Add real testimonials to `CONFIG.testimonials` as you get them; that section stays hidden until you do.
- Review the value-stack prices and the guarantee wording so they match what you'll really deliver.

## Deploy to Vercel
Drag the `proposal-template` folder into vercel.com/new, or run `npx vercel` inside the folder.
