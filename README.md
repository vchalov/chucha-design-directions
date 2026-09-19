# ChuCha — design directions (throwaway prototype)

Live: <https://vchalov.github.io/chucha-design-directions/>

A throwaway research prototype from Phase 0. It shows one session workflow —
the adult prepares a session, the child's screen waits, a reaction is confirmed,
the reward plays, the session ends — in two renderings of the adult bar:

- **Direction A** — dark bar with light labels.
- **Direction B** — cream bar with orange outlines and dark labels.

Everything else is identical in both. The point of the prototype is to let the
team's specialist choose between two of her own drawings.

This is not the product and not product code. The interface is Russian.

## What it does and does not do

- It **records nothing**. The microphone, if it is switched on, is analysed live
  and the frames are discarded. There is no recorder, no buffer and no upload.
- It makes **no network request at runtime**. Everything it needs is in the
  page.
- It holds **no personal data**: no names, no children, no real targets. The
  target labels are placeholders («цель 1» … «цель 4») and the reward windows
  show generated stills, not anyone's video.
- The only thing it keeps on your device is which direction you last looked at.

## Use it

- The `≡` tab in the top-right corner opens a simulator: direction, stage,
  target count, every state, and the build number.
- `?dir=a` or `?dir=b` picks a direction directly.

## Source

This repository holds built output only. The source lives in the private ChuCha
repository under `.scratch/design-directions/`, which git ignores, together with
the report, the decisions and the review notes.
