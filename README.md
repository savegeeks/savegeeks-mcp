# SaveGeeks Price Finder (MCP server)

A free, hosted MCP server that finds the lowest current price on Amazon.com for anything a shopper describes.

- **Endpoint:** `https://savegeeks.com/mcp` (Streamable HTTP, no sign-in, no API key)
- **Website:** https://savegeeks.com
- **Tool:** `find_lowest_price`

## What it does

Give it what the shopper wants in plain words, with an optional top price. It checks up to 120 Amazon.com listings, leaves out cases, cables, refills and spare parts, checks the cheapest color, and returns the three lowest prices that really match, each with title, price, picture and link.

## Tool: `find_lowest_price`

| Input | Type | Notes |
|---|---|---|
| `query` | string | What the shopper wants, for example "air fryer" |
| `max_price` | number | Optional top price in US dollars |
| `prime` | boolean | Optional. Only Prime items |
| `free_shipping` | boolean | Optional. Free-shipping items only (this is the default) |
| `four_stars` | boolean | Optional. Only items rated 4 stars and up |

## Connect

Add a remote MCP server with the URL `https://savegeeks.com/mcp`.

## Good to know

- Prices are read live from Amazon.com (United States) at the time of the request, and can change.
- Links are Amazon affiliate links. SaveGeeks may earn a commission, at no extra cost to the shopper.
- SaveGeeks is independent and is not run by Amazon.
- Contact: hello@savegeeks.com
