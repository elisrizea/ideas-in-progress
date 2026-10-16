# Sonia: an AI shop assistant in one script tag

**Live product · technical note** · Alin Rizea, DBM AI · October 2026

**Live demo:** https://demo.dbm-ai.com/ (Sonia on seven demo shops)
**Read the write-up:** https://elisrizea.github.io/ideas-in-progress/sonia-shop-assistant/
· [PDF](sonia-shop-assistant.pdf)

## What it covers

Sonia is the shop assistant in FormAI, DBM AI's product for online shops. One script tag adds two assistants to a
website: Sonia, who answers product and shop questions, and A2, who helps visitors fill in forms.

- **One Shadow DOM, two assistants.** Both live in one chat panel inside a closed Shadow DOM, so the shop's CSS and
  scripts can't break it and it can't break the shop. A2's help and microphone buttons sit beside the shop's own
  form fields; pressing "Chat" switches the shared panel to A2 mode, and each mode keeps its own messages.
- **How the search is built.** Every shop gets a store schema from its WooCommerce data (categories, attributes,
  tags, brands, price range, currency, product count). A router model turns a question like "orange leather bag
  under 300" into precise search parameters against the shop's real catalogue.
- **Search on the shopper's machine.** Some small hosts block every datacenter IP, so our server can't reach the
  shop. Then the search moves into the shopper's browser: our server plans the queries, the browser runs them in
  parallel against the shop's public Store API from the shop's own page, and our server writes the answer from the
  real results, treating them as untrusted input.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The write-up (self-contained, served by GitHub Pages) |
| `sonia-shop-assistant.pdf` | The same write-up as an A4 PDF |
| `sonia-widget.png` | Screenshot of the Sonia panel on a shop page |
| `cover.png` | Link-preview card |

The code is in private repositories. See the [main page](../) for how to get in touch.
