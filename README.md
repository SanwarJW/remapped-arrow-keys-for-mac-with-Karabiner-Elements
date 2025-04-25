# ⌨️ Karabiner-Elements: Vim-style Arrow Keys with Modifier Passthrough

This Karabiner-Elements configuration enables **Vim-style navigation** using `Right Command + HJKL` to mimic arrow keys on macOS. It also supports **modifier passthrough**, so holding `Option`, `Left Command`, or both, in addition to `Right Command`, will perform the usual macOS shortcuts:

- `Right Command + H` → ⬅️ `Left Arrow`
- `Right Command + J` → ⬇️ `Down Arrow`
- `Right Command + K` → ⬆️ `Up Arrow`
- `Right Command + L` → ➡️ `Right Arrow`

---

### 🔁 Modifier Passthrough Support

This config supports the following enhanced behaviors:

| Keys Pressed                        | Behavior                             |
|------------------------------------|--------------------------------------|
| `Right Command + H`                | ← Move one character left            |
| `Right Command + Option + H`       | ← Move one word left                 |
| `Right Command + Left Command + H` | ← Jump to beginning of line          |
| `Right Command + Option + Left Command + H` | ← Jump to beginning of previous word |
| *(same for J, K, L as ↓ ↑ →)*      |                                      |

---

### 🧠 How It Works

Karabiner-Elements does **not** allow "modifier passthrough" by default. So this configuration creates **multiple conditions** for each key (`H`, `J`, `K`, `L`) to detect when additional modifiers like `Option` or `Left Command` are also pressed.

Each key has **four variations**:
- Plain (`Right Command`)
- With `Option`
- With `Left Command`
- With `Option + Left Command`

---

### 📂 File Structure

---

### ✅ Installation Steps

1. Make sure [Karabiner-Elements](https://karabiner-elements.pqrs.org/) is installed.
2. Open Karabiner-Elements → `Complex Modifications` → `Add Rule`
3. Import this config:
   - Either place your JSON inside `~/.config/karabiner/assets/complex_modifications/`
   - Or use the "Import More Rules from the Internet" and reference your GitHub repo
4. Enable the rule: **"Right Command + HJKL = Arrow Keys with modifier passthrough"**

---

### 👤 Author

Made with ❤️ by [Sanwar Jayswal](https://sanwar.web.app)

---
