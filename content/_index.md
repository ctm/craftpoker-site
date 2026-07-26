+++
title = "Craft Poker"
description = "Craft Poker is online home poker with friends — one of the widest varieties of poker anywhere, in tournaments and ring games, all played with Fun Money that has no cash value."
template = "index.html"

# ---------------------------------------------------------------------------
# Homepage copy. Everything the homepage shows lives here so you can edit the
# words without touching the HTML template (templates/index.html loops over it).
# ---------------------------------------------------------------------------
[extra]
hero_title = "Home poker with your friends — dozens of games, no gambling"
hero_subtitle = "Craft Poker brings your home game online: one of the widest varieties of poker you'll find, in tournaments and ring games. Everyone plays with Fun Money that has no cash value — nothing to buy in, nothing to cash out."

# Primary call to action → the live game.
cta_primary_label = "Play now"
cta_primary_url = "https://friends.craftpoker.com"

# Secondary call to action → the Players' Manual (documents the game variants).
cta_secondary_label = "Explore the games"
cta_secondary_url = "https://ctm.github.io/docs/players_manual/"

# Hero graphic. Drop a real 1200x675 image at static/img/ and point here.
hero_image = "img/hero.svg"

# Feature cards. `icon` picks a built-in inline SVG: games | trophy | devices | chip.
features = [
  { icon = "games", title = "Dozens of games", body = "Hold'em and Omaha (including hi/lo), Stud, Razz and Stud-8, draw and lowball games, plus rare variants like Chowaha, Courchevel, Dramaha, Mississippi Stud and Archie. Perfect for mixed games and dealer's choice." },
  { icon = "trophy", title = "Tournaments & ring games", body = "Run structured tournaments with rebuys, add-ons, bounties and late registration — or drop into a casual ring game whenever a few friends are around." },
  { icon = "devices", title = "Play anywhere", body = "Play in any web browser, or install the native apps for macOS, Windows, iOS and Android. The desktop apps keep themselves up to date automatically." },
  { icon = "chip", title = "Fun Money, not gambling", body = "Every chip is Fun Money with no cash value. You can't buy in with real money and you can't cash out — it's about the game and the people, not the stakes." },
]
+++

<!--
  This page renders from the [extra] fields above (see templates/index.html).
  The Markdown body here is intentionally empty; edit the fields, not this text.
-->
