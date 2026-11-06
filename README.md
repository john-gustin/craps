# Craps Live

Live two-player craps with chat. No accounts, no sign-in.

Play: https://john-gustin.github.io/craps/

1. Open the page, enter your name, and click **Open a table**.
2. Send your friend the invite link (e.g. in Google Chat).
3. They open it and join your table live. You both bet against the house with $1,000 of play money, and the dice pass between you.

Messages are relayed through several free public MQTT brokers at once (EMQX, HiveMQ, Mosquitto, shiftr.io), so if one is down or blocked the others carry the game. `mqtt.min.js` is bundled. The host's tab holds the game: if the host closes it, reopening the same link resumes the table.
