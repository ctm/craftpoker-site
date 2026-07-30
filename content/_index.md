+++
title = "Craft Poker"
description = "Craft Poker: online poker with friends — perhaps the widest varieties of poker anywhere, played with Fun Money (no cash value)."
template = "index.html"

# ---------------------------------------------------------------------------
# Homepage copy. Everything the homepage shows lives here so you can edit the
# words without touching the HTML template (templates/index.html loops over it).
# ---------------------------------------------------------------------------
[extra]
hero_title = "Welcome"
hero_subtitle = "This page is placeholder. The game server, however, is being tested daily by around a hundred people. <i>You're welcome to join us</i>, but don't expect to learn much about the site from this particular page. Mission, Blog, Contact and Play are all correct.<br/><br/>Craft Poker deals <a href=\"https://ctm.github.io/docs/players_manual/games.html\">dozens of variants</a> of poker. It's all <a href=\"https://ctm.github.io/docs/players_manual/fun_money.html\">Fun Money</a> that has no cash value but allows you to keep score if you want to."

# Primary call to action → the live game.
cta_primary_label = "Play now"
cta_primary_url = "https://friends.craftpoker.com"

# Secondary call to action → the Players' Manual (documents the game variants).
cta_secondary_label = "Explore the games"
cta_secondary_url = "https://ctm.github.io/docs/players_manual/games.html"

# Hero graphic. Drop a real 1200x675 image at static/img/ and point here.
hero_image = "img/hero.svg"

# Feature cards. `icon` picks a built-in inline SVG: games | trophy | devices | chip.
features = [
  { icon = "games", title = "Dozens of games", body = "Hold'em, Omaha, Stud, Razz and \"normal\" draw and lowball games, as well as obscure variants like Chowaha, Courchevel, Dramaha, Mississippi Stud and Archie. Both fixed mixed games that can rotate by hand count or by level as well as some dealer's choice games where the players interactively choose which games from a menu." },
  { icon = "trophy", title = "Tournaments & nascent ring games", body = "Run structured tournaments with rebuys, add-ons, bounties and late registration — or drop into a casual ring game whenever a few friends are around. TBH, the ring game support is in its infancy." },
  { icon = "devices", title = "Play anywhere", body = "Play in any web browser, or install the native apps for macOS or Windows, (iOS and Android coming soon)." },
  { icon = "chip", title = "Fun Money", body = "Keep realistic score, with no real money involved." },
]
+++

<!--
  This page renders from the [extra] fields above (see templates/index.html).
  The Markdown body here is intentionally empty; edit the fields, not this text.
-->
