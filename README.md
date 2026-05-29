# Samodeus

**A distraction-free writing temple.**

Samodeus isn't a word processor for compiling reports or building documents — it's a place to *write*, and to tend to the thoughts that become writing. Drafting a novel, revising a manuscript, holding the shapes of sudden ideas and half-remembered dreams: each is a different mode of writing with its own needs. Tools for the long haul of first drafts; tools for the slow, careful pass of revision; tools for folding in feedback from beta readers; a marble board for scanning the texture of an idea without yet committing to its details.

The philosophy is minimalistic but all-inclusive. Thesaurus, dictionary, and rhymer live one keystroke away — no leaving the page to look something up. Distractions are designed out, not bolted on: a non-blinking cursor if you want one, an editor stripped of clutter, and spell-check you can switch off entirely — or dial up into deeper style checks when you want sharper feedback. Curves, color, and type can be tuned to your taste, leaning toward wabi-sabi softness rather than the linear office severity of a Word or Google document.

A sacred space for the work of language — and for the thoughts you arrange before they become it.

> macOS only

---

## Install

1. Download [**`Samodeus.zip`**](https://github.com/andreysamode/samodeus-releases/releases/latest/download/Samodeus.zip) (always points to the latest release).
2. Unzip it. You'll get **`Samodeus.app`**.
3. **If you already have Samodeus installed**, delete the existing `Samodeus.app` from `/Applications` first. macOS Finder merges `.app` bundles instead of replacing them, which can break auto-updates.
4. Drag `Samodeus.app` into `/Applications`.

### First launch

Samodeus is not yet code-signed, so macOS will block it the first time you open it. Open **Terminal** and run:

```bash
xattr -cr /Applications/Samodeus.app
```

This clears the quarantine flag macOS attaches to downloaded files. Then double-click `Samodeus.app` normally.

After the first launch the app remembers, and future updates download automatically in the background.

---

## Getting started

Samodeus organizes everything in four nested levels — keep this picture in mind:

**Library → Shelf → Book → Page**

A **library** is a single `.deus` file on disk. Inside it are one or more **shelves** (top-level sections, like separate workspaces). Each shelf holds **books** (folders) and **pages** (documents), nested as deep as you like.

1. Launch **Samodeus**. The window opens to two buttons in the center: **New** and **Open**. Click **New**.
2. Pick a location and save your **library** as e.g. `Writing.deus`.
3. A starter **Workspace** **shelf** is created inside the library. Click **+** in the left sidebar to add your first **book** (a folder) or a **page** (a document).
4. Open the page and start writing.

---

## The editor

### Selecting and formatting text

When you select text, a small **dashed-circle indicator** appears at the top center of the editor. Hover it to expand into the formatting toolbar:

- **Bold** (`Cmd+B`)
- **Italic** (`Cmd+I`)
- **Strikethrough** (`Cmd+T`)
- **Mark** — drop an inline comment on the selection (details [below](#marks--annotations-for-revision)); also insertable via the `/` slash menu or `Cmd+/`
- **Inline code** — or select text and press `` ` ``, or wrap text with backticks (`` `like this` ``)
- **Link** — paste a URL with text selected to apply it directly

### Slash menu

Press `/` anywhere to open the command menu. Type to filter, ↑/↓ to navigate, Enter to insert:

- Heading 1, 2, 3
- Bulleted list
- Numbered list
- Checklist
- Quote
- Code block
- Table
- Fieldset (a collapsible section)
- Notes board (a marble grid of stickies)
- Mark (an inline annotation — details [below](#marks--annotations-for-revision))

### Lists and tasks

- **Tab / Shift+Tab** — indent / outdent
- **Alt+↑ / Alt+↓** — move an item up or down
- **Enter on an empty item** — exit the list
- **Hold a task checkbox** — pick a marker style (box, heart, checkmark, and more)

### Marks — annotations for revision

Marks are the spine of the editing workflow. A mark is a small inline icon that anchors to a span of text and carries a rich-text comment of its own. They're how you keep track of revisions, beta-reader notes, and the half-formed ideas you don't want to lose.

There are five mark types — each one a different colored icon — for different intents:

- **Note** — observations, thoughts, references
- **Todo** — something you'll come back to
- **Done** — something you finished but want to remember why
- **Heart** — passages you love
- **Mark** — a generic highlight

**How to insert a mark — three ways:**

- **Selection toolbar** — select text, then click the mark button in the dashed-circle toolbar.
- **Slash menu** — type `/mark` and press Enter.
- **Keyboard** — press **`Cmd+/`** with your cursor in place, or with a range of text selected so the mark anchors to that whole range (drawn as a dashed underline).

**Working with marks:**

- **Click a mark** to open its popover and write a comment, change its type, or delete it.
- **Drag a mark's icon** to extend or move the range it's anchored to.
- **Type `[todo: fix this scene]`** inline to create a todo mark from plain text. Same pattern for `[note: ...]`, `[heart: ...]`, etc.

This is how you handle a shower idea at 2am ("Sarah should be the one who finds the letter, not Mark"): drop a mark on the relevant paragraph, jot the thought, keep writing.

### Notes board

Insert via `/notes`. A board of sticky notes arranged in a grid, designed for the scan-don't-read mode of work — drafting beat sheets, capturing dream fragments, holding character shards before they're scenes:

- Set notes per row (1–5), uniform height, starting number
- Per-note color (with optional texture in marble mode — see below)
- Toggle the whole board between **open** (notes visible) and **collapsed** (a single tile)
- **Wide mode** lets the board bleed beyond the editor's width

You can collapse the board to glance at it as shape and color without being pulled into the contents — useful when you want the gestalt of the work, not the details.

#### Marbles — the title-first variant

Switch the board into **marble mode** to turn each sticky into a small, colored, textured marble that shows only the note's **title**. Click a marble to expand it and read the body.

Marbles are for the kind of jotting where you don't need to see the whole entry — you just need to see *what it's about*. A dream diary is the canonical example: dreams are a rich source for writing, but a wall of dream transcripts is unreadable at a glance. As marbles, each dream becomes a few-word title in a constellation you can scan; clicking one opens the full account when you want it.

- Each marble keeps its own color and texture, independent of the others
- The board still toggles open/collapsed and supports wide mode

### Find and replace

- **`Cmd+F`** — open the find bar
- **`Cmd+G` / `Shift+Cmd+G`** — next / previous match
- Replace one or all matches from the bar
- Toggle case-sensitive and whole-word options

### Global search

Search across every page in the current shelf:

- Click the **magnifying glass** in the left sidebar or press **`Cmd+Shift+F`**

---

## Wordbook — dictionary, thesaurus, rhymer

Press **`Cmd+D`** and the Wordbook opens with three tabs:

- **Thesaurus** — synonyms and antonyms
- **Dictionary** — definitions and senses
- **Rhymes** — perfect and near rhymes for a word

If you have text selected when you open the Wordbook, it's pre-loaded as the search. Close the Wordbook and your selection is preserved — you can stay in the flow without losing your place.

Dictionary and Thesaurus are imported from your Mac's Dictionary app.

---

## Spelling, grammar, and style

Click the **spellcheck icon** in the right sidebar or press **`Cmd+E`** to open the spelling and style panel. As you write, Samodeus underlines issues inline; click any underline to see the suggestion and apply or dismiss it.

This isn't just a spell-checker. Samodeus bundles a stack of writing-quality rule sets so it can catch the patterns that actually weaken prose: **clichés, weasel words, passive voice, hedge words, wordiness, jargon, redundancy, biased and exclusive language**, and overall **readability** scoring. Under **Settings → Spellcheck & Grammar** you can mix and match rule sets:

- **Samodeus** — house defaults tuned for fiction and long-form
- **Vale** — core grammar and consistency rules
- **Proselint** — clichés, redundancies, weasel words, common writing sins
- **Google** developer style
- **Microsoft** writing style
- **Write Good** — clarity, passive voice, wordiness
- **Readability** — Flesch-Kincaid and friends
- **Alex** — inclusive, considerate language

You can add words to a **personal whitelist** so proper nouns and invented names stop getting flagged, and you can disable any individual rule or point to your own custom Vale rule files.

---

## Organizing your work

Samodeus content is organized in four nested levels:

**Library → Shelf → Book → Page**

- A **Library** is a single `.deus` file on disk.
- A **Shelf** is a top-level section inside a library. Every library starts with one shelf called **Workspace**.
- **Books** are folders that live inside a shelf. They can contain pages and other books — nest as deep as you like.
- **Pages** are documents. They can sit directly in a shelf, or inside a book.

### What you can do with items

- **Create** — the `+` button in the sidebar, then pick Book or Page
- **Rename** — click the name
- **Drag & drop** — reorder, or move between books
- **Delete** — items go to the shelf's **Trash**, where you can restore or permanently delete them

### Tabs

Open pages appear as tabs above the editor. Right-click a tab to **pin** it — pinned tabs collapse to just their first letter or icon and sit at the front of the row, so the pages you always want at hand don't drift away.

- `Cmd+1` … `Cmd+9` — jump to tab 1–9
- `Cmd+R` — flip back to the previously active tab; press it again to flip back. Useful for ping-ponging between two tabs — for example, a draft and a tab of beta-reader feedback you're working through.
- `Cmd+W` — close current tab

---

## Settings (quick tour)

Click the **gear icon** in the top bar.

- **Theme** — Dawn, Day, Pink, Night
- **Font** — typeface and weight for the UI and editor, configurable independently
- **Editor width** — narrow column or full width
- **Zoom** — separate UI and editor zoom
- **Letter spacing & line height** — fine-tune readability
- **Caret** — blinking or static (the non-distracting option)
- **Curves** — how rounded the UI feels, the dial that takes it from clinical to soft

All settings are **per-shelf** — each shelf can have its own theme, fonts, and look.

---

## Advanced features

### Multiple shelves

A library can hold any number of shelves — think of them as separate workspaces inside the same `.deus` file (novel, journal, dream log…). Switch between shelves from the shelf icon in the top bar. Each shelf has its own settings, trash, and open tabs.

### Per-shelf encryption

Any shelf can be protected with a password.

1. Open the **shelf settings** (gear next to the shelf name)
2. Set a password and an **auto-lock timeout** (Never, 5 min, 15 min, 30 min, or 1 hour)

When a shelf is locked its contents are encrypted on disk and inaccessible without the password. **Passwords are not recoverable if forgotten.**

### Tables, code blocks, images, fieldsets

For when you need them: insert via the slash menu (`/table`, `/codeblock`, `/fieldset`) or paste/drop an image. Tables resize by dragging borders; fieldsets are collapsible sections with their own color; images resize with drag handles on the edges and corners, and for the time being are only referenced, NOT imported into the library.

### Background effects

Under **Settings → Extras**:

- **Stars** — animated starfield behind the editor; configure speed, density, color, and star size
- **Snow** — gentle snowflakes; configure speed, color, and size

Each effect can be toggled and styled independently.

---

## Keyboard shortcuts

### Writing

| Shortcut            | Action                                                     |
| ------------------- | ---------------------------------------------------------- |
| `Cmd+B` / `Cmd+I`   | Bold / italic                                              |
| `Cmd+T`             | Strikethrough                                              |
| `` ` ``             | Wrap selection in inline code (or surround with backticks) |
| `Cmd+/`             | Insert an inline mark                                      |
| `/`                 | Open slash menu                                            |
| `Tab` / `Shift+Tab` | Indent / outdent list, next / previous table cell          |
| `Cmd+]` / `Cmd+[`   | Indent / outdent list item                                 |
| `Alt+↑` / `Alt+↓`   | Move list item or table cell up / down                                   |
| `Cmd+A`             | Select containing block; press again to widen              |

### Reference and search

| Shortcut                | Action                                          |
| ----------------------- | ----------------------------------------------- |
| `Cmd+D`                 | Open Wordbook (thesaurus / dictionary / rhymes) |
| `Cmd+E`                 | Spelling, grammar, and style panel              |
| `Cmd+F`                 | Find in document                                |
| `Cmd+G` / `Shift+Cmd+G` | Next / previous match                           |
| `Cmd+Shift+F`           | Search across the shelf                         |

### Window and tabs

| Shortcut          | Action               |
| ----------------- | -------------------- |
| `Cmd+1` … `Cmd+9` | Switch to tab 1–9    |
| `Cmd+R`           | Previous tab         |
| `Cmd+W`           | Close tab            |
| `Cmd+Shift+R`     | Reload window        |
| `Cmd+=` / `Cmd+−` | Editor zoom in / out |

---

## Updates

Samodeus checks for new versions automatically and downloads updates in the background. You'll see a red dot next to the settings icon to install & relaunch when an update is ready. Releases land on this repo — see the [Releases page](https://github.com/andreysamode/samodeus-releases/releases) for changelogs.

---

## Troubleshooting

- **"Samodeus is damaged and can't be opened"** — Gatekeeper quarantine. Open Terminal and run `xattr -cr /Applications/Samodeus.app`, then launch the app normally.
- **Auto-updates seem broken after a manual install** — make sure you fully deleted the old `Samodeus.app` before copying the new one (don't let Finder merge bundles).
- **Locked shelf, forgot password** — passwords are not recoverable. The encrypted shelf data cannot be opened without it.
