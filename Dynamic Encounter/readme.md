An improved encounter tables tool - DEnc was developed to support quick and easy creation of encounter tables with all of the following features:
- Multiroll encounters
- Easy to follow format
- Automatic `!battle` support
- Non-combat Encounters with rolls
- Easily handles multiple sources of tables
- Roll by Location and Tier
- View specific entries

**Works With**
- [Battle Planner Tool](https://avrae.io/dashboard/workshop/5f7eb5d2f2d59b2718720f7f)
- `!battle` by _Derixyleth#0636_ | [Avrae Development Server](http://invite.avrae.io/)

**Rolling Encounters**
`!denc [entry] <location> <tier#> [entry #]`

To roll on the Arctic Location Tier 1
EX: `!denc arctic 1`

To view a specific entry, simply add the following:
EX: `!denc entry arctic 1 24`

**Setting Tables to Use**
DEnc uses a `svar` or `cvar` named `DencEncounterSources` to assign the sources for rolling.
`!svar|cvar DencEncounterSources ["gvar1","gvar2"]`

Will always use a Personal var if available, then Server, then it's default.

**Changing the Tables**
[Template Tool](https://docs.google.com/spreadsheets/d/1_CHLNTMfkPrOxCsKnEjFK-JTQ9LbrAbpCTQa6vH1XwU/edit?usp=sharing)
[Example Output](https://avrae.io/dashboard/gvars?lookup=205a34cb-9125-46ce-a67d-b685af736b69)
The system runs on a series of JSON tables as shown in Example Output. Note, manual tables can be easily made using the format provided in the Template Tool Output.

_The Sheets:_
`Names & XP` - Contains the reference table to pull **Name Overrides** and **XP Amounts**. You should always add creatures here with their exact monster entry name, an override if they have one, and their xp value. This will allow the other tables to auto-populate.

`Example` - This is a completed example encounter table with creatures, overrides, xp, and all other features purely as a reference.

`COPY ME` - This is the blank encounter table, ready for populating. Each column header has a note on hover about what that column is for. Be careful not to modify the Name/XP columns without understanding. If you do you can always restore them by re-dragging the formula from the other rows.

`Output` - This is where the selected table sheet's information will be fully formatted and ready for copying and final format. Make sure to follow the instructions in **READ ME** and **Example GVAR Layout** as appropriate.

**Issues & Support Me**
Quick Help [Discord](https://discord.gg/HczsFcY)
You can file reports and feature requests on [GitHub](https://github.com/storytellermahkasad/Avrae-Customizations)
If you want to tip: [Ko-fi](https://ko-fi.com/storytellermahkasad)