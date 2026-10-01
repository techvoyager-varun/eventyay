# Issue 6046 evidence

Before captures were taken on upstream `dev` at `ee4ab2c95` before implementation. After captures show the local organiser workflows and saved relationships using a dedicated demonstration event and dummy accounts.

`before.mp4` is a 20-second captioned browser-frame walkthrough of the original forms. `after.mp4` is a 55-second captioned browser-frame walkthrough of the implemented flows. These are captured-state walkthroughs, not continuous screen recordings.

The before/after JPEGs remain available for inspecting the individual states. `css-restored.jpg` shows the styled page after restoring generated static assets.

The local CSS interruption came from the talk test fixture running `collectstatic --clear` against the development static directory while compressor entries remained cached. Generated assets were rebuilt and only stale compressor cache entries were cleared. Final test runs use a separate temporary static root.

The evidence and local helper scripts are excluded from the source commit.
