# ClipStack — the latest build

One file, `latest.json`, holding the newest build number published to
TestFlight.

ClipStack reads it to decide whether to put a dot on the settings gear. It is
here rather than in the app's own repository because that one is private, and a
badge that needs a token is a badge that does not work.

**Nothing else is here and nothing else should be.** The only thing published is
a number that anybody running the app can already read in About.

`Tools/make-mas-pkg.sh --upload` writes this file after a successful upload, so
it cannot claim a build that was never delivered.
