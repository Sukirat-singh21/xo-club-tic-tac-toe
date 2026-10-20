# Publish XO Club with GitHub Pages

`index.html` is the entry point for the Pages site. The game is static and has
no build step.

1. Put the contents of this folder in the root of the GitHub repository you
   want to use. Keep `index.html` at the repository root.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and the `/(root)` folder, then save.
5. After Pages finishes its first deployment, share the URL shown in the
   Pages settings. Project sites normally use
   `https://OWNER.github.io/REPOSITORY/`.

The site is publicly reachable. Players create a game and share its invite
link; opening that link joins automatically. PeerJS Cloud handles signaling
to find the other browser, then WebRTC carries the game moves directly between
players. The signaling service does not relay game moves. The game has no TURN
relay fallback, so some restricted networks may not establish a direct
connection. Internet access is required to load the PeerJS browser library
and reach the signaling service.
