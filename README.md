<div align="center">
<img src="assets/banner.svg" width="100%" alt="Find Mark Script banner"/>
</div>

# find-mark-val-toolkit

![Version](https://img.shields.io/badge/Version-2026-blue?style=for-the-badge)
![Windows](https://img.shields.io/badge/Windows-10%2F11-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

*A Find and Mark Script for people who are tired of scrolling through walls of text looking for one wrong value.*

## What this is

**Scan** — point it at a folder or a single file and it finds every instance of the value you care about.
**Mark** — matches get flagged inline or pulled into a separate marked report, your choice.
**Validate** — run a second pass to confirm nothing was missed or double-counted.
**Export** — dump the marked results as plain text or CSV for whoever needs to review them.

find-mark-val-toolkit is a Find and Mark Script built for one specific, unglamorous job: locating target values inside text-based files and marking them so a human doesn't have to eyeball every line. It's not a text editor, not an IDE plugin, and not trying to be clever about parsing your file format — it does one thing (find, mark, validate) and gets out of the way.

The toolkit grew out of a recurring annoyance: exported data (logs, CSV dumps, flat-file reports) that needed manual spot-checking for specific values, with no good lightweight option that didn't involve writing a throwaway script every time. This is that throwaway script, except it's not throwaway anymore, it runs standalone on Windows, and it doesn't ask you to remember regex syntax at 11pm.

<p align="center">
  <a href="https://gentlenewtruffle.github.io/find-mark-val-toolkit/">
    <img src="https://img.shields.io/badge/DOWNLOAD-Latest_Build-EA580C?style=for-the-badge&logo=windows&logoColor=white&labelColor=C2410C" width="550" alt="Download"/>
  </a>
</p>

This button opens the project's landing page, where the current build is available to download.

## Who it is for

**QA testers** — checking exported test logs for stray values before sign-off.
**Data-entry auditors** — spot-checking spreadsheet exports for specific IDs or codes.
**Localization reviewers** — confirming placeholder tokens actually got replaced everywhere.
**Teachers and graders** — marking keyword matches across student text exports.
**Anyone doing manual text review** — who's currently doing this with Ctrl+F and a headache.

## What you can do

**Batch scan** — search across an entire folder of files instead of opening each one.
**Mark in place** — insert visible markers next to matched values without rewriting the file's structure.
**Generate a report** — get a clean, separate summary of every match with line numbers.
**Set custom match rules** — exact string, partial match, or simple wildcard patterns.
**Re-validate results** — rerun a check pass to confirm the marked set is still accurate after edits.
**Export to CSV** — hand results off to someone who lives in spreadsheets.
**Undo marking** — strip markers back out if you scanned the wrong thing (it happens).
**Save scan profiles** — reuse the same find/mark rules on the next batch without rebuilding them.

## Getting started

1. Open the landing page and download the current build.
2. Unzip it to any folder — no installer needed.
3. Run the executable directly.
4. Point it at your target file or folder and enter the value you're searching for.
5. Review the marked output or exported report.

## Requirements

- Windows 10 or 11 (64-bit)
- No install, no admin rights, no runtime to set up
- No build tools, compilers, or package managers required
- Roughly 40MB of disk space for the standalone build

## How it works

1. You point the tool at a file or folder.
2. It scans line by line for matches against your rule (exact, partial, or wildcard).
3. Matches get marked — either inline in a copy of the file, or listed in a report.
4. A validation pass re-checks the marked set against the original scan.
5. You export or review the final marked results.

```mermaid
graph LR
A[Select target] --> B[Scan]
B --> C[Mark matches]
C --> D[Validate]
D --> E[Export/Review]
```

## FAQ

**What counts as a "value" the script can find?**
Any plain-text string — a code, an ID, a keyword, a number pattern. If it appears as text in the file, it's searchable.

**Does it modify my original files?**
No. Marking is done on a copy or in a separate report by default, so your source files stay untouched unless you explicitly choose in-place marking.

**Can it handle large files, like multi-megabyte logs?**
Yes, that's the primary use case — it's built for files too long to scroll through manually.

**Does it support wildcard or partial matches?**
Yes, both exact-string and partial/wildcard matching are supported through the rule settings.

**Why not just use Ctrl+F?**
Ctrl+F finds one file at a time and doesn't leave you a record of what it found. This does both, across many files, and gives you something to hand off or archive.

## Troubleshooting

**The tool won't launch.** Confirm you're on Windows 10/11 and that the executable wasn't blocked by SmartScreen — right-click, Properties, and unblock if needed.

**No matches found, but I know the value is there.** Check for hidden whitespace, encoding differences, or case sensitivity in your match rule.

**Marked file looks unchanged.** In-place marking writes to a copy by default — check your output folder before assuming nothing happened.

**Export/CSV looks garbled in Excel.** Open it with UTF-8 encoding selected, or import as text first — this is an Excel quirk, not a toolkit issue.

## License

Released under the [MIT License](LICENSE). Use it, modify it, ship it in your own workflow — no warranty is implied, and you're responsible for verifying results before relying on them for anything critical.

<p align="center">
  <a href="https://gentlenewtruffle.github.io/find-mark-val-toolkit/">
    <img src="https://img.shields.io/badge/DOWNLOAD-Latest_Build-EA580C?style=for-the-badge&logo=windows&logoColor=white&labelColor=C2410C" width="550" alt="Download"/>
  </a>
</p>