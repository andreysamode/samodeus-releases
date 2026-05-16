# Samodeus

**A distraction-free writing temple for macOS.**

Samodeus isn't a word processor. It isn't for compiling reports or building documents — it's a place to *write*, and to tend to the thoughts that become writing. Drafting a novel, revising a manuscript, holding the shape of a half-remembered dream: each is a different mode of writing, each with its own needs. Tools for the long haul of first drafts; tools for the slow, careful pass of revision; tools for folding in feedback from beta readers; a marble board for scanning the texture of an idea without yet committing to its details.

The philosophy is minimalistic but all-inclusive. Thesaurus, dictionary, and rhymer live one keystroke away — no leaving the page to look something up. Distractions are designed out, not bolted on: a non-blinking cursor if you want one, an editor stripped of clutter, and spell-check you can switch off entirely — or dial up into deeper style checks when you want sharper feedback. Curves, color, and type can be tuned to your taste, leaning toward wabi-sabi softness rather than the linear-office severity of a Word or Google document.

A sacred space for the work of language — and for the thoughts you arrange before they become it.

> macOS only

---

## Install

1. Download the latest **`Samodeus-<version>-arm64.zip`** from the [Releases page](https://github.com/andreysamode/samodeus-releases/releases).
2. Unzip it. You'll get **`Samodeus.app`**.
3. **If you already have Samodeus installed**, delete the existing `Samodeus.app` from `/Applications` first. macOS Finder merges `.app` bundles instead of replacing them, which can break auto-updates.
4. Drag `Samodeus.app` into `/Applications`.

### First launch

Samodeus is not yet code-signed, so macOS will block it the first time you open it. The easiest fix:

- **Right-click `Samodeus.app` → Open → Open** in the confirmation dialog.

That's it for most macOS versions. On macOS Sequoia (15.x) you may need an extra step: after the first blocked launch, go to **System Settings → Privacy & Security** and click **Open Anyway**.

After the first launch the app remembers, and future updates download automatically in the background.

---

## Getting started

1. Launch **Samodeus**. The window opens to two buttons in the center: **New** and **Open**. Click **New**.
2. Pick a location and save your library as e.g. `Notes.deus`. (`.deus` files are your Samodeus library — they look like a single file in Finder.)
3. A starter **Workspace** shelf is created. Click **+** in the left sidebar to add your first **Page** (a document) or **Book** (a folder for pages).
4. Open the page and start writing.

---

## The editor

### Selecting and formatting text

When you select text, a small **dashed-circle indicator** appears at the top center of the editor. Hover it to expand into the formatting toolbar:

- **Bold** (`Cmd+B`)
- **Italic** (`Cmd+I`)
- **Strikethrough** (`Cmd+Shift+X`)
- **Link** (`Cmd+K`) — or paste a URL with text selected to apply it directly

The toolbar follows your selection, not your cursor — it stays put while you read the surrounding text.

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
- Mark (an inline annotation)

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

**How to use them:**

- Place your cursor and press **`Cmd+/`** to drop a mark there.
- Or select a range of text first, then press **`Cmd+/`** — the mark anchors to that whole range, drawn as a dashed underline.
- **Click a mark** to open its popover and write a comment, change its type, or delete it.
- **Drag a mark's icon** to extend or move the range it's anchored to.
- **Type `[todo: fix this scene]`** inline to create a todo mark from plain text. Same pattern for `[note: ...]`, `[heart: ...]`, etc.

This is how you handle a shower idea at 2am ("Sarah should be the one who finds the letter, not Mark"): drop a mark on the relevant paragraph, jot the thought, keep writing.

### Notes board — the marble grid

Insert via `/notes`. A board of sticky notes arranged in a grid, designed for the scan-don't-read mode of work — drafting beat sheets, capturing dream fragments, holding character shards before they're scenes:

- Set notes per row (1–5), uniform height, starting number
- Per-note color and texture (35 textures, plus marble mode for spherical 3D notes)
- Toggle the whole board between **open** (notes visible) and **collapsed** (a single tile)
- **Wide mode** lets the board bleed beyond the editor's width

You can collapse the board to glance at it as shape and color without being pulled into the contents — useful when you want the gestalt of the work, not the details.

### Find and replace

- **`Cmd+F`** — open the find bar
- **`Cmd+G` / `Shift+Cmd+G`** — next / previous match
- Replace one or all matches from the bar
- Toggle case-sensitive and whole-word options

### Global search

Search across every page in the current shelf:

- **`Cmd+Shift+F`**, or
- Click the **magnifying glass** in the left sidebar

---

## Wordbook — dictionary, thesaurus, rhymer

Press **`Cmd+D`** and the Wordbook opens with three tabs:

- **Thesaurus** — synonyms and antonyms
- **Dictionary** — definitions and senses
- **Rhymes** — perfect and near rhymes for a word

If you have text selected when you open the Wordbook, it's pre-loaded as the search. Close the Wordbook and your selection is preserved — you can stay in the flow without losing your place.

---

## Spelling, grammar, and style

Press **`Cmd+E`** to open the spelling and style panel — or click the **spellcheck icon** in the right sidebar. As you write, Samodeus underlines issues inline; click any underline to see the suggestion and apply or dismiss it.

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

Samodeus organizes content in three nested levels:

**Library (`.deus` file) → Shelves → Books and Pages**

- A **Library** is a single `.deus` file on disk.
- A **Shelf** is a top-level section inside a library. Every library starts with one shelf called **Workspace**.
- **Books** are folders. **Pages** are documents. Books can contain pages and other books — nest as deep as you like.

### What you can do with items

- **Create** — the `+` button in the sidebar, then pick Book or Page
- **Rename** — click the name
- **Color & icon** — pick from a palette so items are easier to spot
- **Drag & drop** — reorder, or move between books
- **Delete** — items go to the shelf's **Trash**, where you can restore or permanently delete them

### Tabs

Open pages appear as tabs above the editor. Right-click a tab to **pin** it — pinned tabs collapse to just their icon and sit at the front of the row, so the pages you always want at hand don't drift away.

- `Cmd+1` … `Cmd+9` — jump to tab 1–9
- `Cmd+R` — flip to previous tab
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

When a shelf is locked its contents are encrypted on disk and inaccessible without the password. Other shelves in the same library remain available. **Passwords are not recoverable — there is no reset.**

### Tables, code blocks, images, fieldsets

For when you need them: insert via the slash menu (`/table`, `/codeblock`, `/fieldset`) or paste/drop an image. Tables resize by dragging borders; fieldsets are collapsible sections with their own color; images resize with drag handles on the edges and corners.

### Background effects

Under **Settings → Extras**:

- **Stars** — animated starfield behind the editor; configure speed, density, color, and star size
- **Starfall** — sparkles falling like rain; tunable speed, density (up to 1200 particles), and color (single tint or rainbow)
- **Snow** — gentle snowflakes; configure speed, color, and size

Each effect can be toggled and styled independently.

---

## Keyboard shortcuts

### Writing

| Shortcut | Action |
|---|---|
| `Cmd+B` / `Cmd+I` | Bold / italic |
| `Cmd+Shift+X` | Strikethrough |
| `Cmd+K` | Add or edit a link |
| `Cmd+/` | Insert an inline mark |
| `/` | Open slash menu |
| `Tab` / `Shift+Tab` | Indent / outdent list, next / previous table cell |
| `Cmd+]` / `Cmd+[` | Indent / outdent list item |
| `Alt+↑` / `Alt+↓` | Move list item up / down |
| `Cmd+A` | Select containing block; press again to widen |

### Reference and search

| Shortcut | Action |
|---|---|
| `Cmd+D` | Open Wordbook (thesaurus / dictionary / rhymes) |
| `Cmd+E` | Spelling, grammar, and style panel |
| `Cmd+F` | Find in document |
| `Cmd+G` / `Shift+Cmd+G` | Next / previous match |
| `Cmd+Shift+F` | Search across the shelf |

### Window and tabs

| Shortcut | Action |
|---|---|
| `Cmd+1` … `Cmd+9` | Switch to tab 1–9 |
| `Cmd+R` | Previous tab |
| `Cmd+W` | Close tab |
| `Cmd+Shift+R` | Reload window |
| `Cmd+=` / `Cmd+−` | Editor zoom in / out |

---

## Updates

Samodeus checks for new versions automatically and downloads updates in the background. You'll be prompted to relaunch when one is ready. Releases land on this repo — see the [Releases page](https://github.com/andreysamode/samodeus-releases/releases) for changelogs.

---

## Troubleshooting

- **"Samodeus is damaged and can't be opened"** — Gatekeeper quarantine. Right-click → Open, or on Sequoia: System Settings → Privacy & Security → Open Anyway.
- **Auto-updates seem broken after a manual install** — make sure you fully deleted the old `Samodeus.app` before copying the new one (don't let Finder merge bundles).
- **Locked shelf, forgot password** — passwords are not recoverable. The encrypted shelf data cannot be opened without it.
