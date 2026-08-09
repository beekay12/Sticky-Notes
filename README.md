# 📝 Sticky Notes Board

A modern, interactive **Sticky Notes Board** built with pure **HTML, CSS, and JavaScript**.

The project recreates the feel of a physical corkboard covered with sticky notes while adding useful digital features such as searching, filtering, dragging, pinning, completion tracking, colour customization, keyboard shortcuts, and automatic browser storage.

---

## ✨ Features

### 📌 Sticky Notes

* Create unlimited sticky notes
* Drag and reposition notes around the board
* Notes have a randomized rotation for a natural physical-board appearance
* Notes can be opened in a focused/expanded view
* Maximum of **225 characters per note**
* Character counter displayed on every note
* Creation date and last-edited time displayed
* Notes automatically receive unique IDs

### 🏷️ Categories

Notes can be organized into:

* 🟥 **Work**
* 🟨 **School**
* 🟩 **Personal**
* 🟦 **Shopping**
* 🟧 **Other**

You can filter the board by category or display all notes.

### 🎨 Customization

Each note can have its own colour.

Changing a note's category automatically applies the category's default colour, while the built-in colour picker allows you to customize it further.

### ✅ Task Management

Notes can be marked as completed.

Completed notes:

* Become visually faded
* Display their text with a strikethrough
* Update the dashboard's completed-note count

### 📌 Pinning

Notes can be pinned using the pushpin at the top of each note.

Pinned notes are visually indicated with a highlighted pin.

### 📋 Duplicate Notes

The duplicate button creates a copy of an existing note while offsetting the new note slightly so both notes remain visible.

### 🗑️ Delete Notes

Notes can be deleted directly using the trash icon.

The keyboard `Delete` key can also be used when a note is active.

---

## 🔎 Search

The built-in search bar allows you to search through note content in real time.

Search can also be opened quickly using:

`Ctrl + F`

The search works together with the category filters, allowing you to narrow down your notes quickly.

---

## 📊 Live Dashboard

A floating dashboard at the bottom of the screen displays:

| Statistic      | Description                               |
| -------------- | ----------------------------------------- |
| 📝 Notes       | Total number of notes                     |
| ✍️ Characters  | Total characters across all notes         |
| 🏷️ Categories | Number of categories currently being used |
| 📌 Pinned      | Number of pinned notes                    |
| ✅ Completed    | Number of completed notes                 |

The dashboard updates automatically whenever the notes change.

---

## 💾 Data Persistence

The application uses the browser's **Local Storage API** to save notes.

Your notes are stored under:

```text
sticky_notes_data
```

This means your notes remain available after refreshing or reopening the page in the same browser.

No external database or backend is required.

---

## ⌨️ Keyboard Shortcuts

| Shortcut   | Action                     |
| ---------- | -------------------------- |
| `Ctrl + N` | Create a new note          |
| `Ctrl + S` | Save notes                 |
| `Ctrl + F` | Focus the search bar       |
| `Delete`   | Delete the active note     |
| `Esc`      | Close an active note/modal |

A keyboard-shortcuts modal is also available directly inside the application.

---

## 🖥️ Interface

The interface consists of:

* Top control bar
* New Note button
* Search field
* Keyboard shortcuts button
* Category filters
* Full-screen sticky-note board
* Live statistics dashboard
* Focused-note overlay
* Keyboard shortcuts modal
* Save notification/toast

The board uses a textured brown background to imitate a physical corkboard.

---

## 🛠️ Technologies Used

### HTML5

Used to structure the application interface and note components.

### CSS3

Used for:

* Responsive positioning
* Sticky-note styling
* Animations
* Shadows
* Transitions
* Modal overlays
* Corkboard texture
* Note rotations
* Hover effects
* Focused-note mode

### JavaScript

Used for:

* Note creation
* Note deletion
* Note duplication
* Drag-and-drop positioning
* Search
* Filtering
* Pinning
* Completion status
* Colour customization
* Local Storage
* Dashboard statistics
* Keyboard shortcuts
* Date/time tracking

---

## 📁 Project Structure

The current project is intentionally contained in a single HTML file:

```text
sticky-notes-board/
│
└── index.html
```

The HTML file contains:

```text
HTML
├── Interface structure
│
├── CSS
│   ├── Board styling
│   ├── Sticky notes
│   ├── Controls
│   ├── Dashboard
│   ├── Modals
│   └── Animations
│
└── JavaScript
    ├── Note management
    ├── Local Storage
    ├── Search
    ├── Filtering
    ├── Dragging
    ├── Categories
    ├── Pinning
    ├── Completion
    ├── Duplication
    └── Keyboard shortcuts
```

---

## 🚀 Getting Started

### 1. Download or clone the project

```bash
git clone <your-repository-url>
```

### 2. Open the project

Navigate into the project folder:

```bash
cd sticky-notes-board
```

### 3. Launch the application

Simply open:

```text
index.html
```

in a modern web browser.

No installation, server, database, or build process is required.

---

## 🌐 Browser Compatibility

The application is designed for modern browsers supporting:

* HTML5
* CSS3
* JavaScript ES6+
* Local Storage API
* Pointer Events
* CSS `backdrop-filter`

Recommended browsers:

* Google Chrome
* Microsoft Edge
* Mozilla Firefox
* Safari

---

## 🔐 Privacy

This project does **not require an account or external server**.

Notes are stored locally in the user's browser using `localStorage`.

Your notes are therefore not automatically uploaded to a remote database.

Clearing the browser's site data may remove saved notes.

---

## 🎯 Project Goals

The goal of the project is to combine the simplicity of physical sticky notes with useful digital productivity features.

Instead of creating a traditional list-based task manager, the application provides a visual workspace where users can freely arrange their notes.

---

## 🔮 Possible Future Improvements

Potential features that could be added in future versions:

* [ ] Dark/light board themes
* [ ] Import/export notes
* [ ] JSON backup files
* [ ] Cloud synchronization
* [ ] User accounts
* [ ] Note titles
* [ ] Due dates
* [ ] Reminders
* [ ] Sorting options
* [ ] Note resizing
* [ ] Rich-text formatting
* [ ] Markdown support
* [ ] Image attachments
* [ ] Multiple boards
* [ ] Undo/redo
* [ ] Mobile-specific controls
* [ ] Touch gesture improvements
* [ ] Accessibility settings
* [ ] Offline PWA support
* [ ] Custom category creation

---

## 🧑‍💻 Development

This project intentionally uses vanilla web technologies without frameworks.

There are no external JavaScript dependencies or package installations required.

The main application state is maintained through a JavaScript `notes` array and persisted to browser storage.

Notes contain information such as:

```javascript
{
    id,
    content,
    category,
    color,
    pinned,
    completed,
    createdAt,
    updatedAt,
    posX,
    posY,
    posZ,
    rotFront,
    rotBack
}
```

---

## 📜 License

You are free to modify and use this project for personal or educational purposes.

If you publish a modified version, giving credit to the original project is appreciated.

---

## ⭐ Credits

Built with:

**HTML • CSS • JavaScript**

No framework.
No backend.
No database.
Just a browser and some JavaScript.

---

### 💡 Made to feel like a real desk — without the paper everywhere.
