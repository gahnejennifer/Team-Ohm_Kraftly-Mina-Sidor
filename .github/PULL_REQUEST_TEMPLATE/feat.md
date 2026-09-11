## Vad introducerades?

Added a multi-stage Dockerfile for the frontend.

## Varför?

The frontend is built with Node and then served with nginx.
Only the built dist files are copied to the final image, so Node and node_modules are not included.

## Hur testar man?

- docker build -t kraftly-frontend .
- Build completed successfully

## Checklista

- [ ] Jag har säkerställt att featuren funkar som angivet
- [ ] Commit-meddelandet följer conventional commits
- [ ] Grenen utgår från färskt `main`
