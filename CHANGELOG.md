## In development
### New features
- The color used to indicate speed ranges is now configurable
- The settings dialog has been reworked

### System compatibility
- Drag Ruler's Generic SpeedProvider is now aware of good default values for the lancer game system (thanks to Grygon)

### API changes
This release introduces a new API that is incompatible with the old API. The new API offers more flexibility for users and Speed Providers alike and allows to add new features in the future without breaking compatibility again. The old API will continue to function, but to profit from any of the features below Speed Providers need to switch to the new API. For more details check out the API documentation.

The following things have changed with the new API:
- Colors used by speed providers can now be changed by the user via configuration
- Speed Providers can now offer settings to the user that will be integrated into Drag Ruler's settings menu


## 1.2.2
### Translation
- Added japanese translation (thanks to touge)

## 1.2.1
### Compatiblity
- Drag Ruler is now compatible with Hex Token Size Support. For compatibility Hex Token Size Support Version 0.5.4 or higher is required. Thanks to Ourobor for helping making this possible.

## 1.2.0
### New features
- Right click and spacebar can now be swapped, allowing to place waypoints with right click and removing them with spacebar
- The module can now be configured use a fixed color instead of the player color for the first speed range
- On gridless maps the ruler will now change it's color to indicate the different speed ranges
- As an alternative to right click (or spacebar, if you have swapped right and spacebar behavior) waypoints can now also be deleted with the `X` key

### Bugfixes
- Disabling snap to grid with shift now works as expected
- Fixed a bug where the ruler would sometimes jump to a different target location when deleting a waypoint

## 1.1.1
### Bugfixes
- Fixed a bug where tokens wouldn't be moved to the corect end position on gridless maps
- Ruler now appears immediately when the token is being dragged
- On gridless maps the ruler will always start measuring at the center of the token
  - This change has no impact on the distance that is being measured
  - In addition to the cosmetical aspect this also fixes a bug that allowed players to glitch through walls

## 1.1.0
### New features
- The drag ruler will now be colored for other players than the dragging player as well (only if they have at least observer permissions for that token)
- The drag ruler won't be shown to other players if they cannot see the dragged token

### Bugfixes
- Fixed a bug where Drag Ruler wouldn't work at all on some windows installations (specificially where the `foundry.js` has `CRLF` line endings)

## 1.0.1
### Bugfixes
- The GM can now move tokens through walls
- It is now possible to move multiple tokens with Drag Ruler enabled
