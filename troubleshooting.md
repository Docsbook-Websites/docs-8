---
title: "Troubleshooting"
description: "Find the cause of the errors this series actually produces, in the order they usually happen, with the check that confirms each one."
status: generated
version: "0.1"
---

# Troubleshooting

Work down the list. Each entry says how to confirm it is your problem before you change anything, because the fastest way to make a small problem confusing is to apply three fixes at once.

<!-- widget:accordion -->

### Command not found

The tool is not installed, or not on your path. Confirm with the version command from [part one](tutorials/part-1-setup.md). If the version command works in one terminal and not another, it is your path, not the install — reopen the terminal first.

### Wrong version

Confirm the installed version against the one in [Before you start](before-you-start.md). A major version released after this series was written is the single most common cause of a step that "used to work".

### Permission denied

You are writing somewhere you may not, or running as the wrong user. Resist the temptation to escalate privileges to make it go away — that turns a clear error into a file only an administrator can edit later.

### It works locally but not deployed

Almost always a missing environment variable, a different runtime version, a path that only exists on your machine, or a file that was never committed. Check those four before anything else. See [part three](tutorials/part-3-ship.md).

### Nothing happens at all

Check you are running it from the directory you think you are, and that the file you edited is the file being read. Both are embarrassing and both are extremely common.

### An error message you cannot parse

Read the *last* line first, then the first. The middle of a stack trace is usually somebody else's code. Search the exact text, in quotes, before reasoning about it.

<!-- /widget -->

<!-- widget:callout type=tip -->

### Change one thing at a time

Then re-run the check from part one. Two changes and one improvement means you now have two candidate explanations and no way to choose between them.

<!-- /widget -->

## Still stuck

> **Fill this in:** where to ask, and what to include — the command, the exact error text, the version, and what you already tried.

## Next steps

<!-- widget:cards plain cols=2 -->

- [Command reference](reference/commands.md) — Check the syntax {terminal}
- [Questions people ask](faq.md) — If it is not an error but a doubt {message-circle-question}

<!-- /widget -->
