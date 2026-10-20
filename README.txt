XO CLUB — ONLINE TIC-TAC-TOE

QUICK START

1. Open https://sukirat-singh21.github.io/xo-club-tic-tac-toe/ or open
   TicTacToe.html in a recent browser. Both players need an internet
   connection.
2. One player clicks “Create game,” then shares the invite link.
3. The friend opens the link. They join automatically as O; no reply code is
   needed. Keep the creator’s page open until the match ends.

HOW IT CONNECTS

PeerJS Cloud handles the short signaling step that helps the browsers find
each other. After that, WebRTC sends game moves directly between the two
browsers. PeerJS Cloud does not relay the game moves. The room ID in the
invite link is temporary; anyone with the link can try to join the room.

Some school, work, mobile, or firewalled networks block direct peer
connections. This version has no TURN relay fallback, so try another network
if the direct connection fails. Internet access is also needed to load the
PeerJS browser library and reach its signaling service.

FILES

TicTacToe.html  The game, for local play or GitHub Pages hosting.
index.html      The GitHub Pages entry point.
README.txt      These quick-start instructions.
