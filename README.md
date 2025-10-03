# STPC COORDS PICKER  
*(with Objective JSON Editor)*

**V1.1**

---

## TAGLINE
Pick world coordinates (X, Y, Z) directly on a map. No need to enter the game to read altitude.

## NOTE
Preconfigured for the Sakhal map. No map/image setup required.

---

## WHAT IT DOES
- Double-click to place a marker/waypoint.
- Altitude (Y) fills automatically and updates when you move a marker.
- Saved Points panel to group and organize markers (AIPatrol, AICamp, TreasureHunt, or your own folders).
- Patrol lines connect waypoints that belong to the same patrol group.
- One click to open the Objective JSON Editor (form-based editing, no raw JSON).
- Optional “Enable Markers Dragging” for precise placement.

---

## QUICK START
1. Open **STPC Coords Picker** (Sakhal loads ready to use).
2. Pan with **Middle Mouse Button** (hold and drag). Zoom with **Mouse Wheel**.
3. **Double-click** to add a point (or **Right-click → Add new marker/waypoint**).
4. Organize and rename points in the **Saved Points** panel (drag & drop).
5. Click **“JSON Editor…”** to finalize objective details.

---

## OBJECTIVE JSON EDITOR (GENERAL FEATURES)
- No raw JSON required: edit via clean, user-friendly forms.
- Pre-populated dropdowns and class lists pulled from your Profile copy (e.g., item/weapon classnames).
- Helpful tooltips and input hints throughout (IDs, texts, time limits, distances, etc.).
- Consistent layouts and sensible defaults to speed up editing.

---

## DEFINITIONS
- **App Root** = the folder where this application resides.  
- **Profiles area** = `App Root\Profiles\`

---

## CONFIGURATION: PROFILES (LOCAL COPY FOR THE EDITOR)

**Goal**  
Make a local copy of your server’s `profiles` and `mpmissions` so the editor can read classnames and related data.

**Steps**
1. Create a new subfolder under:  
   `App Root\Profiles\<profilename>\`
2. Copy **both** of these from your server into that new folder:  
   - `profiles`  
   - `mpmissions`
3. Final structure example:

    App Root\Profiles\sakhal\profiles...
    App Root\Profiles\sakhal\mpmissions...
    
**Notes**
- Keep this local copy updated when your server changes (so dropdowns/class lists stay current).
- The JSON Editor reads classnames and related data from this local `Profiles\<profilename>\profiles` copy.

---

## CONFIGURATION: OBJECTIVES (STAGING WORKFLOW)

**Concept**  
Objectives are edited in a dedicated **staging** folder inside the App Root to avoid accidental edits to live server files.

**Import existing objectives (choose one source)**
- **From your server:**  
Copy **all** folders from:  %serverroot%\profiles\ExpansionMod\Quests\Objectives

Paste into:  

App Root\Objectives\

- **From your local profile copy (if already mirrored as above):**  
Copy from:  
App Root\Profiles<profilename>\profiles\ExpansionMod\Quests\Objectives

Paste into:  
App Root\Objectives\

**Editing**
- Open the JSON Editor and edit objectives directly from `App Root\Objectives\` (staging).
- Use forms, pre-filled dropdowns, and hints. No raw JSON is needed.

**Publish back to server (manual)**
- When finished, copy the edited folders from:  
App Root\Objectives\

Back to:  
%serverroot%\profiles\ExpansionMod\Quests\Objectives

- Back up or merge as appropriate for your workflow.

**Reminder**
- Staging prevents accidental changes to live files. Only published copies affect your server.

---

## CONTROLS
- **Pan:** Hold Middle Mouse Button and drag  
- **Zoom:** Mouse Wheel  
- **Add Marker:** Double-click the map  
- **Context Menu:** Right-click  
- **Precise Adjust:** Toggle “Enable Markers Dragging” and move markers (Y auto-updates)  
- **Sidebar:** Collapse/expand the Saved Points panel  

---

## PERSONALIZATION (SETTINGS)
- Marker visuals: crosshair size, dot diameter  
- Labels: font size, X/Y offsets, fill color, outline color  
- Zoom feel: base step, minimum zoom, maximum zoom  
- ID length: choose how short/long new marker IDs are  

---

## INCLUDED COMPONENTS
- **STPC Coords Picker** (map, markers, patrol lines, Saved Points)
- **Objective JSON Editor** (form-based editing, pre-filled dropdowns, tooltips)
- Built-in short docs and hints

---

## CLOSING
Build objectives faster and pick precise coordinates without booting the game.
