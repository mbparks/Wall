# WALL

**Exhibition Layout & Hanging Instrument**  
**Version 4.4.0**

**ROOM → WALL → WORK → SCALE → HANG → PLAN**

WALL is a local-first browser application for planning exhibitions at physical scale and turning curatorial layouts into practical installation documents.

It is designed for artists, curators, galleries, museums, collectors, schools, pop-up exhibitions, installers, and anyone who needs to lay out artwork on real walls and produce reliable hanging measurements.

WALL is not general-purpose CAD and it does not attempt to judge whether an exhibition is aesthetically "correct."

Its job is simpler:

> **Design exhibitions at actual scale. Arrange works spatially. Turn layouts into installation measurements.**

---

## Core Philosophy

WALL follows one central principle:

> **WALL measures composition. It does not judge composition.**

The application exposes measurable information such as:

- artwork size
- spacing
- alignment
- center height
- wall occupancy
- architectural conflicts
- mounting-point locations
- label placement
- installation status
- planned vs. as-installed coordinates

It deliberately avoids aesthetic scoring, automated taste judgments, or AI-generated quality ratings.

You decide what looks right. WALL makes that decision measurable, repeatable, and installable.

---

# Core Workflow

WALL supports the full exhibition-planning workflow:

1. Create an exhibition
2. Define rooms and walls
3. Record architectural features
4. Add artwork and exhibition objects
5. Arrange works at true physical scale
6. Define hanging hardware
7. Calculate mounting coordinates
8. Add labels and wall interpretation
9. Check fit, spacing, and conflicts
10. Compare alternate layouts and venues
11. Plan installation order
12. Record as-installed positions
13. Produce hanging sheets and installation documents
14. Archive the completed exhibition

---

# ROOM

Define the exhibition space.

Rooms can contain measured walls and floor-plan geometry. WALL supports spaces such as:

- rectangular galleries
- irregular rooms
- corridors
- alcoves
- temporary partitions
- freestanding walls
- pop-up spaces

The floor-plan tools are intentionally lightweight. WALL is not intended to replace architectural CAD.

---

# WALL

The wall elevation is the primary planning workspace.

Each wall can include:

- physical width and height
- floor and ceiling references
- gallery centerline
- custom guides
- named datums
- doors
- windows
- openings
- radiators
- vents
- outlets
- electrical panels
- structural objects
- restricted regions
- interpretation panels

The wall canvas is always based on real physical dimensions rather than arbitrary screen pixels.

---

# WORK

Each artwork can include:

- work ID
- inventory number
- accession number
- title
- artist
- year
- medium
- collection
- owner
- tags
- notes
- artwork dimensions
- outside frame/object dimensions
- depth
- weight
- installation clearance
- thumbnail/image
- display type
- mounting hardware
- installation status
- as-installed record

WALL distinguishes between image dimensions and the actual physical object dimensions used for layout.

---

# SCALE

WALL works in physical units.

Supported display systems include:

- inches
- feet and inches
- millimeters
- centimeters
- meters

Imperial measurements can also be displayed using architectural fractions.

Geometry is stored independently of screen zoom, so changing the browser size does not change real-world positions.

---

# HANG

Artwork can be positioned by:

- dragging
- numeric coordinates
- center point
- edge offsets
- alignment commands
- distribution commands
- keyboard nudging
- mechanical arrangement tools

Useful layout operations include:

- align left
- align right
- align top
- align bottom
- align centers
- center on wall
- equal horizontal spacing
- equal vertical spacing
- centered row
- vertical stack
- grid
- salon seed

WALL also supports multi-selection, groups, locking, snapping, guides, and measurement tools.

---

# PLAN / OUTPUT

WALL converts the layout into installation documentation.

## Exhibition Package

A broader project document containing exhibition summary information, wall layouts, work schedules, installation information, interpretation objects, and planning records.

## Wall Hanging Sheet

A field-oriented sheet for one wall showing:

- wall dimensions
- scaled elevation
- artwork locations
- centerline
- architectural objects
- hanging points
- datum references
- labels
- interpretation
- installation status
- as-installed deviations

## Work Install Card

A focused installation sheet for one artwork showing:

- work identity
- physical dimensions
- wall
- center position
- preferred datum
- mounting system
- hook/mount coordinates
- label placement
- planned position
- as-installed position
- notes

Browser printing can be used to save these outputs as PDF.

---

# Hanging Hardware

Current mount types include:

- None
- Single Hook
- Two D-Rings
- Picture Wire
- French Cleat
- Security Hanger
- Rail Hanger
- Standoffs
- Custom Mounting Points

For supported mounting types, WALL derives wall hardware positions from artwork geometry.

For example, a two-D-ring installation can calculate:

- left ring X
- right ring X
- ring height AFF
- work top
- work center
- datum-relative hook positions

These coordinates update when the artwork moves or its mounting geometry changes.

---

# Datums and Measurement

WALL provides installation references that match how work is actually installed in a gallery.

Typical references include:

- wall left edge
- wall center
- wall right edge
- finished floor
- ceiling
- gallery centerline
- door edges
- window edges
- architectural feature edges
- custom horizontal datums
- custom vertical datums

A work can use different horizontal and vertical references.

Example:

```text
WORK CENTER
42.50 in right of Entry Door — right edge
57.00 in above Finished Floor
```

The measurement tool supports persistent point-to-point dimensions including:

- horizontal delta
- vertical delta
- direct distance
- angle
- source coordinate
- destination coordinate

---

# Artwork Inventory

The Inventory view supports:

- search
- sorting
- filtering
- placed/unplaced status
- incomplete-data filtering
- thumbnails
- bulk tagging
- bulk mount assignment
- CSV import
- CSV export

Useful inventory categories include:

- All
- Placed
- Unplaced
- Incomplete

---

# Labels and Interpretation

Artwork labels can have:

- real dimensions
- left/right/above/below placement
- configurable offset
- custom content
- automatic title/artist content
- custom position

Independent interpretation objects can include:

- title panels
- section text
- introductory text
- vinyl lettering
- QR panels
- accessibility panels
- directional signage

Interpretation objects participate in collision and wall-bound checks.

---

# Architectural Features

Wall features can be placed and edited directly.

Supported examples include:

- doors
- windows
- openings
- niches
- columns
- radiators
- outlets
- electrical panels
- vents
- thermostats
- fire equipment
- permanent signage
- structural objects
- restricted areas

Features can include clearance zones and may act as installation datums.

---

# Conflict Detection

WALL can surface review items such as:

- artwork outside wall bounds
- artwork overlap
- installation-envelope overlap
- architectural-feature conflicts
- label collisions
- interpretation collisions
- mounting points outside wall bounds
- missing dimensions
- missing hanging hardware
- incomplete media configuration

Findings are planning aids rather than aesthetic judgments.

---

# Simple and Deep Modes

## Simple Mode

Focused on the essential hanging workflow:

**ADD WALL → ADD WORK → ARRANGE → HANG PLAN**

Advanced planning and metadata controls are reduced.

## Deep Mode

Exposes the complete exhibition-planning system, including:

- multiple rooms
- architectural features
- datums
- detailed mounting geometry
- labels
- interpretation
- groups
- scenarios
- fit analysis
- capacity planning
- venue tools
- visitor sequence
- sightlines
- media systems
- handling records
- installation sequencing
- revisions
- archive tools

---

# Interface

WALL v4.4 uses a canvas-first interface.

## Left Pane

Primary navigation for:

- project
- rooms
- walls
- placement status
- inventory
- planning summary

## Center Canvas

The active:

- room/floor plan
- wall elevation
- exhibition workspace

## Right Inspector

Contextual controls for the selected:

- wall
- work
- architecture
- interpretation
- planning object
- installation record

Inspector sections can be collapsed and their state is remembered.

## Unplaced Tray

A collapsible tray containing works not currently placed.

Use the **UNPLACED** command or keyboard shortcut `U` to toggle it.

---

# Toolbar

The streamlined v4.4 toolbar keeps common actions visible and moves secondary commands into menus.

Primary tools include:

- ROOM
- WALL
- SELECT
- PAN
- MEASURE
- INVENTORY
- PLANNING
- OUTPUT

## LAYOUT

Contains:

- fit wall
- fit works
- zoom selection
- alignment
- distribution
- grid
- snap

## ADD

Contains:

- guides
- datums
- architecture
- wall text / interpretation

---

# Planning Workbench

Advanced planning is grouped into four areas.

## CURATE

- Groups / Series
- Layout Scenarios
- Arrange
- Visitor Sequence

## SPACE

- Floor Plan
- FIT
- Capacity
- Sightlines
- Photo Walls
- Venue Survey

## INSTALL

- Exhibition Objects
- Media Systems
- Lighting
- Handling / Conservation
- Install Sequence

## VENUES & RECORDS

- Venue Library
- Compare Venues
- Touring
- Baselines / Revisions
- Exhibition Archive

---

# Groups and Series

Works can be grouped by:

- artist
- series
- section
- theme
- installation group
- narrative sequence
- custom group

Groups can be selected, moved together, centered, arranged, locked, and annotated without destroying the identity of individual works.

---

# Layout Scenarios

WALL supports alternate exhibition layouts such as:

- Baseline
- Chronological
- Thematic
- Salon
- Reduced Selection
- Alternate Installation

Each scenario stores its own placement state.

Scenario comparison can report:

- works placed
- walls used
- spacing
- occupancy
- conflicts

Switching scenarios restores the saved geometry for that scenario.

---

# FIT Analysis

FIT answers:

> Where could this work physically go?

Candidate walls may be classified as:

- FIT
- BLOCKED — current layout
- BLOCKED — architecture
- TOO NARROW
- TOO SHORT

FIT considers wall dimensions, artwork dimensions, installation envelopes, architectural features, feature clearances, and current placements.

---

# Capacity Planning

Capacity analysis estimates exhibition demand versus available wall supply.

It can consider:

- artwork width
- desired spacing
- edge allowance
- total wall length
- architectural obstructions
- usable wall length
- oversized works

This is a planning estimate, not an aesthetic recommendation.

---

# Venue Library

Measured venue geometry can be saved independently from an exhibition.

A venue record can preserve:

- rooms
- walls
- architecture
- clearance zones
- guides
- datums

Venue Library data can be exported and imported as JSON.

---

# Venue Comparison

WALL can compare the current exhibition against saved venue geometry using information such as:

- room count
- wall count
- raw wall length
- usable wall length
- exhibition demand
- reserve or deficit
- works that fit by physical dimensions

---

# Floor Plan

The room view provides lightweight 2D spatial planning for:

- wall relationships
- room orientation
- exhibition objects
- visitor paths
- sightlines
- installation planning

The wall elevation remains the authoritative workspace for wall-hung artwork.

---

# Visitor Sequence

Works can be assigned a curatorial sequence with:

- entry
- exit
- ordered works
- section transitions
- focal works

This is a planning aid only.

---

# Sightlines and Viewing Distance

Named viewing positions can be placed in the room.

WALL can provide lightweight geometric information about:

- visible walls
- approximate viewing relationship
- primary views
- oblique views
- viewing distance

This is not a photorealistic renderer.

---

# Photo-Calibrated Walls

A photograph of a real wall can be used as a planning background.

Typical workflow:

1. Import wall photograph
2. Identify a known real-world distance
3. Calibrate image scale
4. Adjust opacity
5. Overlay the exhibition layout

Measured wall dimensions remain authoritative.

---

# Venue Survey

Venue Survey supports field measurement and verification.

A wall can retain:

- measured geometry
- verification status
- survey notes
- timestamp

---

# Exhibition Objects

Supported display types include:

- wall-mounted work
- pedestal
- plinth
- floor object
- display case
- shelf
- monitor
- projection
- listening station
- suspended work

Spatial objects may include:

- footprint width
- footprint depth
- object height
- support height
- clearance
- position
- orientation
- rotation
- installation status
- as-installed position

---

# Media Systems

Media works can include:

- power requirement
- playback/source
- signal/interface
- networking
- projection throw distance
- screen dimensions
- audio requirements
- equipment notes

---

# Lighting Notes

Lighting records may include:

- fixture type
- fixture position
- target work
- beam note
- intensity note
- color temperature
- status
- installation note

WALL does not attempt full photometric simulation.

---

# Handling and Conservation

Optional work records can include:

- handling instructions
- orientation restrictions
- environmental notes
- security mounting
- minimum clearance
- maximum illumination
- condition reference
- crate/packing information

---

# Install Mode

Install Mode provides a focused field interface for hanging the exhibition.

Typical progression:

**LOCATE → MARK → HARDWARE → HANG → LEVEL → LABEL → VERIFY**

Statuses include:

- Not Started
- Marked
- Hardware Installed
- Hung
- Verified
- Issue
- Complete

Install Mode supports:

- previous/next work
- mounting coordinates
- datum references
- field notes
- issue flagging
- completion state
- as-installed coordinates

---

# As-Installed Records

WALL can store planned and actual positions separately.

Example:

```text
PLANNED
X 120.00 in
Y 57.00 in

AS INSTALLED
X 121.25 in
Y 57.50 in

DEVIATION
+1.25 in X
+0.50 in Y
```

This preserves the original design intent while documenting the completed exhibition.

---

# Installation Sequence

WALL can build an exhibition-wide installation plan.

Tasks can include:

- hanging wall works
- placing pedestals
- positioning floor objects
- media setup
- lighting setup
- labels
- custom installation tasks

Tasks support dependencies and statuses such as:

- Not Started
- In Progress
- Issue
- Complete

---

# Touring Exhibitions

A layout can be captured as a tour stop.

Tour stops can preserve:

- venue geometry
- wall layouts
- floor-object positions
- omissions
- local adaptations
- hardware changes
- substitution notes

---

# Baselines and Revisions

WALL can freeze layout revisions such as:

- REV A — Curatorial Layout
- REV B — Post Site Visit
- REV C — Approved Installation
- AS INSTALLED

Revision comparison can identify:

- moved works
- reassigned walls
- added works
- removed works
- hardware changes

A previous baseline can be restored.

---

# Exhibition Archive

Completed exhibitions can be archived locally.

Archive records may preserve:

- exhibition metadata
- venue geometry
- works
- layouts
- spatial objects
- installation state
- revisions
- touring information

For storage reliability, lightweight archive records may omit embedded image bytes.

Use exported Project JSON when a complete high-fidelity backup is required.

---

# Local-First and Privacy

WALL is designed to operate locally in the browser.

It does not require:

- user accounts
- cloud authentication
- a backend server
- a hosted database
- telemetry

Project data remains on the local machine unless the user deliberately exports or shares it.

Because browser storage can be cleared by the browser or operating system, important projects should also be exported to JSON.

---

# Autosave

WALL autosaves meaningful project changes locally.

The interface displays a save-state indicator such as:

- SAVING
- SAVED
- UNSAVED

Do not treat browser autosave as the only backup for important exhibition records.

---

# Project Import and Export

## Project JSON

Use Project JSON for complete WALL project portability.

It can include:

- exhibition metadata
- rooms
- walls
- works
- placements
- groups
- labels
- interpretation
- hardware
- installation state
- scenarios
- spatial objects
- touring data
- revisions
- settings

Imported data is validated before replacing the current project.

## CSV

Artwork inventory can also be imported/exported using CSV for bulk data exchange.

---

# Fresh Start

**FRESH START** creates a genuinely empty project.

It does not automatically reload sample data.

Use **LOAD SAMPLE EXHIBITION** separately when demonstration data is wanted.

---

# Sample Exhibition

The included sample project demonstrates:

- multiple rooms
- multiple walls
- architectural features
- artwork of different sizes
- several hanging systems
- labels
- interpretation
- unplaced work
- conflicts
- installation status
- planning tools

Sample data should not be confused with a new blank exhibition.

---

# Undo and Redo

Typical keyboard shortcuts:

- `Ctrl/Cmd + Z` — Undo
- `Ctrl/Cmd + Shift + Z` — Redo

---

# Other Keyboard Shortcuts

Useful shortcuts include:

- Arrow keys — nudge selected object
- Shift + Arrow — larger nudge
- `I` — Install Mode
- `T` — add wall text in Deep Mode
- `U` — toggle Unplaced tray
- Escape — cancel/clear current interaction
- Delete/Backspace — remove selected object where allowed

Locked works and groups resist movement commands.

---

# Themes

WALL supports:

- Light
- Dark
- System

Print output uses a light, high-contrast presentation regardless of the active application theme.

---

# Responsive Use

## Desktop

Best for:

- exhibition layout
- wall editing
- inventory
- planning
- scenario comparison

## Tablet

Suitable for:

- installation
- wall browsing
- measurement review
- work inspection
- placement adjustments

## Mobile

Optimized primarily for:

- Install Mode
- work details
- hanging measurements
- checklists
- field notes

The full drafting workspace remains desktop-oriented.

---

# Installation / Deployment

WALL is a no-compile static web application.

No Node.js, npm, build process, backend, or database is required.

## Basic Deployment

Copy:

```text
index.html
```

to any normal static web host.

Then open the page in a modern browser.

## Local Use

For the most consistent behavior, serve WALL from a local static web server rather than relying on `file://` URLs.

The application does not require internet access after deployment.

---

# Browser Support

WALL is intended for modern browsers with current JavaScript, browser storage, file input, SVG/canvas, and print support.

Chromium-based browsers are the primary target.

Other current browsers should generally work, but print behavior and local-file handling can vary between browser engines.

---

# Data Safety

Recommended practice:

1. Allow autosave to protect normal editing
2. Export Project JSON at meaningful milestones
3. Create revision baselines before major layout changes
4. Export a final project at installation approval
5. Capture an AS INSTALLED baseline after installation
6. Keep exported JSON with the exhibition's other records

Browser storage can be lost if site data is manually cleared.

---

# Performance

WALL is designed for substantial exhibitions, but browser performance depends on:

- number of works
- number and resolution of embedded images
- number of rooms/walls
- interpretation objects
- spatial objects
- browser/device memory

Reducing embedded image resolution can significantly improve performance and storage use for very large projects.

---

# Troubleshooting

## WALL Opens With a Blank Project

A new project is intentionally empty.

Use:

- Create Exhibition
- Load Sample Exhibition
- Import Project

as appropriate.

## My Previous Project Is Missing

Check whether:

- browser/site data was cleared
- the application moved to a different domain/path
- private/incognito browsing was used
- a different browser profile is active

If you exported Project JSON, use **Import Project** to restore it.

## An Artwork Will Not Move

Check whether:

- the work is locked
- its group is locked
- WALL is in PAN or MEASURE mode
- another scenario is active

Switch to SELECT mode and unlock the object/group if necessary.

## Snapping Is Preventing Precise Placement

Turn SNAP off or adjust the grid/guides.

## Mounting Coordinates Look Wrong

Verify:

- outside frame/object dimensions
- artwork center position
- selected mounting type
- hardware offsets
- ring spacing
- top offset
- preferred horizontal datum
- preferred vertical datum

Mount coordinates are derived from these values.

## Printed Output Is Cut Off

Use browser print preview and verify:

- paper size
- orientation
- margins
- scale

Final pagination is handled by the browser's print engine.

## Wall Photo Is Misaligned

Recheck photo calibration using a known physical measurement.

The photograph is only a visual background. Entered wall geometry remains authoritative.

---

# Startup Recovery

WALL includes a startup error boundary intended to avoid a completely blank page after an initialization failure.

If startup fails, WALL should preserve browser project storage where possible and provide recovery-oriented information rather than intentionally clearing the project.

If a serious issue occurs, export recovery/project data before clearing browser storage.

---

# File Structure

The standard WALL distribution is intentionally simple:

```text
WALL/
├── index.html
└── README.md
```

The application itself is self-contained in `index.html`.

---

# Version

Current release:

```text
WALL v4.4.0
```

Schema migrations are handled inside the application so older WALL project data can be upgraded where supported.

---

# Development History

## v0.x — Core Exhibition Wall

- wall elevation
- artwork inventory
- scaled layout
- hanging geometry
- architecture
- datums
- labels
- Install Mode

## v1.x — Advanced Planning

- curatorial groups
- scenarios
- FIT
- capacity
- arrangement tools
- venue library
- venue comparison

## v2.x — Spatial Planning

- floor plan
- visitor sequence
- sightlines
- viewing distance
- calibrated wall photos
- venue survey

## v3.x — Exhibition Objects

- pedestal/floor works
- media
- lighting
- handling/conservation
- installation sequence

## v4.x — Exhibition Lifecycle

- touring exhibitions
- revisions/baselines
- as-installed records
- archive
- v4.4 UI/UX streamline

---

# Design Rule

The most important rule in WALL remains:

> **WALL does not decide what looks right. It makes what you decided measurable, repeatable, and installable.**
