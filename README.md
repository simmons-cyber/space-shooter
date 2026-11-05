# Void Runner

A standalone canvas space shooter. Open `index.html` in a modern browser, or upload it to any static hosting service. All styles, graphics, and game code are included in that file. No dependencies, external assets, API keys, or build step are required, and the game works offline.

## Play

Launch with the on-screen button or Enter. Move with WASD or arrow keys, hold Space to shoot, and press P or Escape to pause. On touch screens, hold and drag in the arena to move and fire; lift your finger to stop. Losing focus automatically pauses the game.

Each destroyed enemy earns 100 points. Every 12 kills advances the wave, increasing enemy speed and spawn frequency. Later waves introduce armored ships. Enemy shots, collisions, and enemies escaping the sector damage your hull. Three hits end the mission; you have brief invulnerability after each hit. Restart with Enter or the on-screen button.

Your best score is saved as you play when browser storage is available. The game remains playable if storage is blocked.

## Deploy

Upload `index.html` as the root page on a static host such as GitHub Pages, Netlify, or Cloudflare Pages. No build command is needed. You can also embed it in an iframe or share the HTML file directly. No server-side application is required.

## Local development

For local HTTP development:

```sh
cd /workspace/space-shooter
python3 -m http.server 8000 --bind 0.0.0.0
```

To validate changes, check launch, keyboard movement and firing, touch movement and automatic firing, pause/resume, collisions and wave progression, game over/restart, best-score persistence, and narrow-screen layouts. Confirm that the browser reports no JavaScript errors and makes no external asset requests.
