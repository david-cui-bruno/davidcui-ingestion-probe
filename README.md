# Concert media ingestion probe

This public repository tests whether a GitHub-hosted macOS runner can prepare one full song from the official YouTube source that a Linux runner could not access. It has no credentials, does not save downloaded media as an artifact, and does not deploy a website. The downloaded files disappear with the temporary runner after the job.

Run the `Probe fresh song on macOS` workflow manually to repeat the test. The test source is the currently published `umru — Poplife` video (`QqV16bh1sZk`).
