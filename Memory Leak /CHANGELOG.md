# Memory Leak — Changelog

## [1.0.1] — 2026-06-21

### Multiplayer
- Reworked events to be properly multiplayer-aware. Events now run for each
  player independently instead of focusing on a single one.
- Fixed rare cases where an event could trigger in the wrong place relative to
  other players. Events now keep their distance from bystanders.

### Performance & Stability
- Fixed long hangs (and an occasional freeze) when leaving a world.
- Faster world loading when entering a world.

### Fixes
- New worlds now start fresh instead of carrying over state from a previous
  world.
- Fixed the player occasionally being placed in an unsafe spot when entering a
  world. Spawning is now back to normal, safe behavior.

### Notes
- This is a maintenance release focused on multiplayer support, performance, and
  stability. No content was removed.
