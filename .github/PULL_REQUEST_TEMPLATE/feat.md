## Vad introducerades?

Added a separate image job to CI that builds the Docker image with docker build and displays the image size in the CI log.

Also updated the CI workflow so it runs on pushes to main.

## Varför?

This fulfills the M3 requirement that docker build runs as its own CI job and that the image size is visible in the CI log.

Running CI on main allows us to verify that the Docker image build is green after the changes are merged.

## Hur testar man?

docker build -t kraftly-frontend .
Check that the Docker build completes successfully.
Check that the image job is green in GitHub Actions.
Check that docker image ls kraftly-frontend displays the image size in the CI log.

## Checklista

- [ X] Jag har säkerställt att featuren funkar som angivet
- [X ] Commit-meddelandet följer conventional commits
- [ ] Grenen utgår från färskt `main`
