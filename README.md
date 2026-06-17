# Emberkeep — Character Rigger

A standalone, zero-dependency 2D character rigging + animation studio for the
[Emberkeep](https://github.com/novativeai/emberkeep-game) dragon game.

- **`index.html`** — rig builder: upload layer PNGs, align them, set
  parent/child rotation pivots (Anchor) and in-layer deform pins (Puppet), then
  export a self-contained `rig.json` (layer transforms, z-order, anchors, pin
  chains, embedded images).
- **`animator.html`** — preview animation presets (idle, hover, celebrate, roar,
  stretch, walk) against a rig. Auto-loads the red dragon
  (`assets/dragon/rig/dragon-red.rig.json`); the engine adaptively resolves each
  motion through anchor → pin-chain → bare-layer so rigs with missing joints
  still animate.

Open either file directly, or serve the folder statically.

Built with [Claude Code](https://claude.com/claude-code).
