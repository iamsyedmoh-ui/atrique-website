# ATRIQUE — Premium Arabian Fragrance

A one-page website for ATRIQUE, a UAE fragrance brand. Customers browse the collection and place orders through WhatsApp. No checkout, no backend: it is a single static file that works on any phone, tablet or laptop.

## What's on the site
- Fragrance collection with prices (MAJD 70 AED, ZAHR 70 AED, SMOKED VANILLA 90 AED), 50ML Eau de Parfum
- Order list: customers add several fragrances and send one WhatsApp message with quantities and total
- Delivery: free on orders above 250 AED, otherwise a flat 10 AED, to all 7 emirates
- FAQ, brand story, emirates map, light and dark theme

## Files
| File | Purpose |
|------|---------|
| `index.html` | The whole website (images and styles are built in) |
| `404.html` | Sends visitors with a wrong address back to the site |
| `.nojekyll` | Tells GitHub Pages to publish the files exactly as they are |
| `README.md` | This guide |

## WhatsApp number
Orders go to WhatsApp number 971503908876. To change it, open `index.html`, find the line starting with `whatsapp:` near the top of the main script and replace the digits (country code + number, no `+` or spaces). Also check the Instagram handle on the next line (`instagram:`).

## Publish with GitHub Pages
1. Create a new public repository on GitHub.
2. Click **Add file > Upload files** and drag in `index.html`, `404.html`, `.nojekyll` and `README.md`. Commit.
3. Go to **Settings > Pages**. Under **Source** choose **Deploy from a branch**, select the `main` branch and the `/ (root)` folder, then **Save**.
4. After about a minute the site is live at `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.

To use your own domain, add it under **Settings > Pages > Custom domain** and follow GitHub's DNS instructions.

## Making changes
All of these are in `index.html`:
- **Prices, names, descriptions:** search for `CFG.products`. Each fragrance has a `price`, `desc`, `notes` and `details`.
- **Delivery fee and free-delivery amount:** search for `FREE=250,FEE=10`, and update the FAQ answer and the banner text at the top to match.
- **Top banner text:** search for `id="ab"`.
- **WhatsApp number and Instagram:** the `whatsapp:` and `instagram:` lines.

After editing on GitHub, the site updates about a minute after you commit.

## Notes
- Fonts load from Google Fonts, so they need an internet connection.
- The customer's order list is remembered in their own browser only.
