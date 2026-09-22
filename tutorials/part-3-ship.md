---
title: "Part 3 — Ship"
description: "Put what you built somewhere other people can reach, verify it from outside, and know what to do when the deployed version behaves differently."
status: generated
version: "0.1"
---

# Part 3 — Ship

Running on your machine and running where other people can reach it are different achievements. This part is the second one.

## What you'll do

- Prepare what you built for somewhere other than your laptop
- Deploy it
- Verify it from outside, as a stranger would

## Steps

<!-- widget:stepper -->

### Prepare it

Configuration that was hardcoded becomes a setting; anything secret moves out of the files entirely. Name every value the deployed version needs.

### Deploy

> **Fill this in** with the real commands or clicks. If there is more than one supported way, pick one for the tutorial and mention the others at the end — a reader choosing between three paths mid-tutorial usually chooses none.

### Verify from outside

Open the public address from a different network or device. Your own machine has caches, sessions and DNS that a stranger does not.

### Check the unhappy path again

The error handling you wrote in part two is now handling real conditions. Try one bad input against the deployed version.

<!-- /widget -->

<!-- widget:callout type=warning -->

### Never commit secrets

Keys and tokens belong in the platform's own settings, not in the repository — and if one ever lands there, rotate it rather than deleting the commit. Deleting is slow, and the key is live the whole time.

<!-- /widget -->

## When the deployed version behaves differently

Almost always one of: a missing environment variable, a different version of a runtime, a path that only exists on your machine, or a file that was never committed. Check those four before anything else.

## What you have now

Something real, at an address you can send someone. That is the whole point of the series, and it is worth telling one person about before you go back to improving it.

## Next steps

<!-- widget:cards plain cols=2 -->

- [What next](../what-next.md) — Where to take it {compass}
- [Troubleshooting](../troubleshooting.md) — If the deploy misbehaves {life-buoy}

<!-- /widget -->
