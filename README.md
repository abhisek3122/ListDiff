# ListDiff

A simple tool to compare two or three lists and see what's common, what's unique, and what got duplicated.

## The problem

You've got two lists (maybe emails, usernames, hostnames, IDs) and you need to find what's in both, what's only in one, what's different. There are online tools that do this, but they take your data and send it to their server. If you're working with anything sensitive (internal data, client lists, security findings) that's not something you want.

This tool runs entirely in your browser. Nothing leaves your machine.

## Features

- **2 or 3 list comparison** - paste two lists and get the diff, or add a third and get the full breakdown across all combinations
- **Editable list names** - rename List A / B / C to something meaningful before comparing
- **Smart result sections** - for 3 lists, results are grouped into: what's in all three, what's shared between each pair (inclusive), what's exclusive to each pair, and what's unique to one. Each section shows the set notation (like A ∩ B − C) so it's clear what you're looking at
- **Tooltips on every section** - hover the ? to get a plain English explanation of what that section contains
- **Duplicate detection** - items that appeared more than once in a list are flagged separately, with the list they came from, so your counts stay accurate
- **Sort toggle per section** - sort any result alphabetically before copying, without losing the original order
- **Copy per section** - copy just the items you need from any result bucket
- **Live entry count** - shows how many items are in each list as you paste
- **Lowercase normalization** - optional toggle to treat "Apple" and "apple" as the same item
- **Whitespace trimming** - always on, strips leading/trailing spaces so copy-paste artifacts don't sneak in as false mismatches

## How to use it

**Locally** - just download `index.html` and open it in your browser. No install, no setup, no server.

**Hosted** - [https://abhisek3122.github.io/ListDiff](https://abhisek3122.github.io/ListDiff) works the same way. We don't collect, log, or see any data you paste in. It's the same static file, just hosted.

## Privacy

The entire tool is a single HTML file with no external dependencies. No CDN, no analytics, no fonts loaded from anywhere. All processing happens in your browser using plain JavaScript. You can open the source and verify this yourself in under a minute.

---

*Vibecoded with Claude. Somehow it works.*
