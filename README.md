# Concert media ingestion probe

This public repository tests whether a GitHub-hosted macOS runner can prepare one full song from the official YouTube source that a Linux runner could not access. It has no credentials, does not save downloaded media as an artifact, and does not deploy a website. The downloaded files disappear with the temporary runner after the job.

Run the `Probe fresh song on macOS` workflow manually to repeat the test. The test source is the currently published `umru — Poplife` video (`QqV16bh1sZk`).

## Result — 2026-10-05

The [macOS run](https://github.com/david-cui-bruno/davidcui-ingestion-probe/actions/runs/37339732031) installed yt-dlp, Node, and ffmpeg, reached YouTube, and failed when YouTube requested a sign-in to confirm the runner was not a bot. The same source had failed on the [Ubuntu production runner](https://github.com/david-cui-bruno/davidcui-concert/actions/runs/37336068979) with HTTP 429 and the same bot challenge. Changing between these two GitHub-hosted networks did not make fresh intake work. No media was published by this probe.
