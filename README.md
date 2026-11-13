# Faculty Board Meeting Manager
### Kandy Uni — Faculty Board Meeting Management System

---

## සිංහල විස්තරය

Kandy Uni Faculty Board රැස්වීම් කළමනාකරණය සඳහා නිර්මාණය කළ web-based tool එකක්. Cover Letter, Agenda, Attendance List සහ Minutes ඇතුළත් PDF ලේඛන ස්වයංක්‍රීයව generate කරනවා.

---

## English Description

A single-file web application for managing Kandy Uni Faculty Board meetings. Fill in meeting details, attendance, agenda, and minutes — then generate professionally formatted PDFs that match the official Kandy Uni document style.

---

## Features / විශේෂාංග

### 📋 Tabs / Tabs
| Tab | Description |
|-----|-------------|
| **Meeting Details** | Meeting number, date, time, venue, chairperson |
| **Cover Letter** | Letter date, previous meeting details, signatory |
| **Formal Agenda** | Numbered agenda items with sub-points |
| **Matters Arising** | Items from previous meeting (auto-numbered from prev. meeting no.) |
| **Attendance** | Main members (33) + Optional members (17) with P/P*/E/A status |
| **Minutes** | Meeting minutes with section codes and responsibility column |

### 📄 PDF Generation / PDF ලේඛන
Three separate PDFs can be generated from the top bar:

| Button | Contents |
|--------|----------|
| **📄 Matters** | Cover Letter only |
| **📋 Agenda** | Cover Letter + Formal Agenda list |
| **📝 Minutes** | Cover Letter + Attendance + Minutes table |

All PDFs include the official **Kandy Uni logo**, navy/orange header stripe, and proper formatting.

### 💾 Save & Load / Save සහ Load
- **💾 Save** — Downloads a `.json` file with all meeting data (filename includes meeting number and timestamp)
- **📂 Load** — Upload a previously saved `.json` file to restore all data
- **Auto-save** — Data is automatically saved to browser localStorage; reopening the page restores your last session

### 🗑 Clear
Clears all data and resets to defaults (also clears localStorage).

---

## Attendance Status Codes / Attendance Status Codes

| Code | Meaning |
|------|---------|
| **P** | Present — රැස්වීමේ 50%කට වැඩි කාලයක් සහභාගි වූ |
| **P\*** | Present less than 50% of the time — 50%ට අඩු කාලයක් සහභාගි වූ |
| **E** | Excused — සමාවෙනසේ නොපැමිණි |
| **A** | Abstained — ඡන්දයෙන් වැළකී සිටි |

---

## Members / සාමාජිකයින්

### Main Members (33) / ප්‍රධාන සාමාජිකයින්
Default list pre-loaded from the 34th Faculty Board Minutes.

### Optional Members (17) / විකල්ප සාමාජිකයින්
Special invitees, student representatives, and guests.

---

## How to Use / භාවිත කරන ආකාරය

### සිංහලෙන්

1. **`index.html`** browser ගේ open කරන්න
2. **Meeting Details** tab ගේ meeting number, date, time, venue fill කරන්න
3. **Cover Letter** tab ගේ letter date, previous meeting details, signatory fill කරන්න
4. **Formal Agenda** tab ගේ agenda items add කරන්න
5. **Matters Arising** tab ගේ previous meeting ගේ matters add කරන්න
6. **Attendance** tab ගේ members ගේ P/P*/E/A status mark කරන්න
7. **Minutes** tab ගේ minutes sections සහ items add කරන්න
8. Top bar ගේ **📄 Matters**, **📋 Agenda**, හෝ **📝 Minutes** button click කරලා PDF generate කරන්න
9. Browser print dialog ගේ **"Save as PDF"** select කරන්න

### In English

1. Open **`index.html`** in a browser
2. Fill in **Meeting Details** (number, date, time, venue, chairperson)
3. Fill in **Cover Letter** details (letter date, previous meeting info, signatory)
4. Add items in **Formal Agenda** tab
5. Add items in **Matters Arising** tab (auto-numbered from previous meeting no.)
6. Mark attendance status (P/P*/E/A) in **Attendance** tab
7. Add minutes sections and items in **Minutes** tab
8. Click **📄 Matters**, **📋 Agenda**, or **📝 Minutes** in the top bar to generate PDFs
9. In the browser print dialog, select **"Save as PDF"**

---

## Save / Load Data / Data Save කිරීම

### Save
1. Top bar ගේ **💾 Save** click කරන්න
2. JSON file eka automatically download වෙනවා
3. File name: `35_FacultyBoard_20261113_0945.json` (meeting no + date/time)

### Load
1. Top bar ගේ **📂 Load** click කරන්න
2. Previously saved `.json` file eka select කරන්න
3. All data restored — edit කරලා නැවත save කරන්න

---

## Technical Details / තාක්ෂණික විස්තර

- **Single HTML file** — no server, no installation required
- **Pure HTML/CSS/JavaScript** — works offline
- **localStorage** — auto-saves data in browser
- **Web Crypto API** — used for password hashing (if applicable)
- **PDF generation** — uses browser's built-in print-to-PDF function
- **Logo** — Kandy Uni logo embedded as base64 (no external dependencies for logo)
- **Fonts** — Inter (Google Fonts)
- **Compatible browsers** — Chrome, Edge, Firefox, Safari

---

## GitHub Pages

If hosted on GitHub Pages:
```
https://<username>.github.io/<repository>/
```

Upload `index.html` to the repository root and enable GitHub Pages from **Settings → Pages → Branch: main**.

---

## Repository / Repository

**GitHub:** [alawatugoda/KU-FacultyBoardMeeting](https://github.com/alawatugoda/KU-FacultyBoardMeeting)

---

## License / බලපත්‍රය

Internal use only — Kandy Uni Faculty Board.

---

*Developed for Kandy Uni Faculty Board Meeting Management | 2026*
