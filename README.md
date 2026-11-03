# rbx-tycoon-template
A base project for creating a Tycoon in Roblox.

PlayerData (Data to be saved)
├─ Version          … Structure version; a safeguard for future structural changes
├─ Resources = {}   … Dictionary with a variable number of entries (e.g., Gold, Gems)
├─ Base = {}        … Purchased items and slot status (pertains to base modules)
├─ Inventory = {}
├─ Progress = {}    … Rebirth count, achievements, etc.
└─ Settings = {}