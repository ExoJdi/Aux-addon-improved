## Extended & Fixed Version (WotLK 3.3.5a)

This fork adds multiple quality-of-life, safety, and stability improvements to the original **Aux** addon, while keeping full compatibility with its core logic and saved data.

---

### Added / Improved Features

#### Options Window (`/aux`)
- `/aux` now opens an in-game options window instead of chat-only configuration
- All original slash-command options are available as checkboxes
- UI scale slider (0.50 → 2.00) with numeric input
- Added **Clear item cache** button (UI alternative to `/aux clear item cache`)

<!-- Screenshot: Options Window -->

---

#### Tooltip Price Priority (ElvUI Compatibility)
- Tooltip output order adjusted to prioritize **Value (daily)** over **Historical**
- External UI addons (e.g. ElvUI crafting cost calculation) now correctly prefer daily prices
- Historical price is used automatically as fallback when daily data is unavailable

<!-- Screenshot: Tooltip Price Order -->

---

#### Multi Buyout Safety
- Fixed and restored safe **multi-buyout protection**
- Prevents accidental mass buyouts at extreme prices
- Warning / confirmation shown when price exceeds safe thresholds

<!-- Screenshot: Multi Buyout Warning -->

---

#### Fast Scan Improvements
- Improved fast scan stability
- Fixed crash and disconnect issues during rapid scanning
- Safe interruption handling

---

#### Full Scan Stability
- Full auction scans can be interrupted safely
- Switching between fast scan and full scan no longer corrupts scan state

---

#### Post Tab Enhancements
- Item insertion via **Alt-click** and **Shift-click**
- Full **Drag & Drop** support into the Post item slot
- Correct handling of itemID and suffix variants

<!-- Screenshot: Post Tab Drag & Drop -->

---

#### General Stability Fixes
- Removed unsafe global calls
- Fixed multiple nil-reference crashes in GUI and Post tab
- Reliable slash-command handling (`/aux` always opens options)

---

