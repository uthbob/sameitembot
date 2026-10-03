# SameItemBot

SameItemBot is a small, non-commercial research crawler operated by Upendra Rai.
It finds the same product across Indian shopping sites (Amazon.in, Flipkart, Croma, Myntra)
for a product-matching demo project.

## Identification
User agent: `SameItemBot/0.1 (+https://github.com/<your-username>/sameitembot; upendrabit235@gmail.com)`

## What it fetches
- Sitemaps and category/listing pages, to build an index of product URLs
- Individual product pages, to read product details and price

## What it never does
- Fetch anything disallowed by robots.txt
- Use site search, stock, pincode or other disallowed endpoints
- Log in, solve CAPTCHAs, or use proxies to avoid blocks
- Collect personal data

## How it behaves
- Checks robots.txt before every request
- At most about 1 request per second per site; backs off on errors
- Stops for a site if it is blocked

## How to block it
Add this to your robots.txt:

    User-agent: SameItemBot
    Disallow: /

Or email upendrabit235@gmail.com, and requests will be honoured promptly.

## Data kept
Product URLs, product attributes and prices only. No personal data.

Last updated: 03/10/2026
