# rbx-tycoon-template
A base project for creating a Tycoon in Roblox.

## PlayerData (Data to be saved)

```text
PlayerData
├─ Version          … Structure version; a safeguard for future structural changes
├─ Resources = {}   … Dictionary with a variable number of entries (e.g., Gold, Gems) (pertains to resource modules)
├─ Base = {}        … Purchased items and slot status (pertains to base modules)
├─ Inventory = {}   … Items owned by the player (pertains to inventory modules)
├─ Progress = {}    … Rebirth count, achievements, etc. (pertains to progression modules)
└─ Settings = {}    … Player preferences (e.g., music, trade requests)
```

> Session-only state and derived/computed values are intentionally
> NOT part of PlayerData and are never saved.

When `Version` is older than the current schema, data is migrated on load.
