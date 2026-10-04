# Trick or Treat .io (web build)

The browser build of **Trick or Treat .io**, a Halloween .io game: lead a line of
trick-or-treaters, grab candy to grow it, and make other gangs' leaders bump into
your line so they scatter into candy. Solo with bots or online rooms (up to 8
players) through the Wayside relay. Served by GitHub Pages at
https://perhapsjohn.github.io/TrickOrTreatIo/ and played in the Scareathon arcade.

One page, two packs: phones load `index.mobile.pck` (no desktop-only music
layers, lighter 3D); desktops load `index.pck`. `?pack=mobile|desktop` forces one.
At midnight the game posts `{type: "PLAYER_DIED", score}` (the night's candy) to
the page around it.

This repo holds only the exported files (Godot 4.6 web export); the game's source
lives elsewhere and publishes here with `tools/publish_web.sh`.
