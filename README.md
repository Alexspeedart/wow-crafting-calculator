# WoW Forever Crafting Profit Calculator

A free, independent crafting profit calculator for World of Warcraft Forever, intended for Windows users. The current version runs locally in a browser and requires no installation. It is not affiliated with Blizzard Entertainment or ForeverDB.

## Current features

- Enter and edit reagents, quantities and prices in separate gold, silver and copper fields.
- Calculate total crafting costs, net sale after the Auction House cut, profit per item, margin, break-even sale price and bulk profits.
- Search Tailoring recipes via a type-ahead dropdown (matches starting with the search term first, then other matches alphabetically).
- Import reagent names and quantities from an included offline starter dataset of **13 Tailoring bag recipes**.
- Optionally expand cloth bolts to their raw cloth requirements.
- Save inputs locally in your browser, reusing recorded reagent prices where possible.

## Try it

Download [index.html](index.html) and double-click it to open the calculator in a modern desktop browser. The current HTML version works offline. The standalone Windows executable is a separate packaging step.

## Recipe database

The [starter Tailoring dataset](data/tailoring-bags.json) contains 13 bag recipes. This is **not yet a complete Tailoring database**. The new search interface is designed to accommodate further recipes, including gear, shirts and other categories as they are added.

## ForeverDB API access request

We are seeking permission to use the ForeverDB API to retrieve **public Tailoring recipe information only**: recipe names and IDs, categories, reagents and quantities, and source game-build/version metadata. We want to:

1. Build a local, searchable Tailoring recipe database, so the calculator works offline.
2. Allow users to import reagent names and quantities without entering them manually.
3. Add a voluntary “Check for recipe updates” action that identifies newly added, changed and removed recipes.
4. Credit ForeverDB visibly and follow all applicable API usage rules, including rate limits and attribution requirements.

Users will enter their own current Auction House prices. **No access to character profiles, Battle.net credentials or other account information is required for the calculator.** API access has not yet been granted or implemented. No private API keys will be stored in this public repository.

## Currency and profit calculations

WoW currency: 100 copper = 1 silver, and 100 silver = 1 gold. The calculator deducts the configured Auction House sale cut. Successful-sale deposits are assumed refunded.

## Project status

Early working prototype. The initial scope is Tailoring. Search and calculation are implemented with 13 starter bag recipes; full-catalog import, update checking, native Windows packaging and expanded categories are planned.

## Disclaimer

World of Warcraft and its related names belong to Blizzard Entertainment. This community project is unofficial.
