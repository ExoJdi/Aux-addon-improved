📘 README (User Documentation)
Aux – Extended Version (WotLK 3.3.5a)

This is a modified and extended version of Aux for
World of Warcraft 3.3.5a (Wrath of the Lich King).

The addon keeps full compatibility with the original Aux database and logic,
while improving usability, stability, and compatibility with modern UI packs such as ElvUI.

Commands
/aux

Opens the Options window.

Options Window
Options

All original Aux settings are available as checkboxes:
- Ignore owner
- Post bid
- Tooltip value
- Tooltip historical
- Tooltip merchant buy
- Tooltip merchant sell
- Tooltip disenchant value
- Tooltip disenchant distribution

Scale
- Slider range: 0.50 → 2.00
- Numeric input (2 decimal precision)
- Applied instantly to the Aux window

Cache Management
- Clear item cache button
- UI alternative to /aux clear item cache

Tooltip Price Behavior
- Value (daily) always has priority over Historical
- If both prices exist:
- - external addons (e.g. ElvUI crafting cost) use Value
- If daily Value is missing:
- - Historical price is used as fallback

Auction Features

Multi Buyout (Safe Buyout)
- Supports multi-item buyout with price safety check
- Prevents accidental buyouts at extreme prices (e.g. 2000%+)
- Confirmation is required when price exceeds historical thresholds

Fast Scan
- Optimized auction scan mode
- Designed for quick market refresh
- Reduced query overhead to avoid disconnects

Full Scan
- Complete auction house scan
- Can be interrupted safely
- Data is stored incrementally without corrupting history

Post Tab Improvements
- Item insertion via Alt-click and Shift-click
- Full Drag & Drop support into the Post item slot
- Correct handling of itemID and suffix variants

Compatibility
- World of Warcraft 3.3.5a
- Compatible with ElvUI (WotLK)
- No external libraries required