# Bash Hotkeys Cheat Sheet

## 🔑 Basic Navigation
- **Ctrl + A** → Move cursor to beginning of line  
- **Ctrl + E** → Move cursor to end of line  
- **Alt + B** → Move back one word  
- **Alt + F** → Move forward one word  

---

## ✂️ Editing & Deleting
- **Ctrl + U** → Delete from cursor to beginning  
- **Ctrl + K** → Delete from cursor to end  
- **Ctrl + W** → Delete previous word  
- **Alt + D** → Delete next word  

---

## 📋 Copy / Paste (Kill & Yank)
- **Ctrl + Y** → Paste (yank) last deleted text  
- **Alt + Y** → Cycle through previous cuts  

---

## 🔄 History & Commands
- **Ctrl + R** → Search command history  
- **↑ / ↓ arrows** → Navigate command history  
- **!!** → Repeat last command  
- **!n** → Run command number *n* from history  

---

## ⚡ Process Control
- **Ctrl + C** → Cancel current command  
- **Ctrl + Z** → Suspend current process  
- **Ctrl + D** → Exit shell (EOF)  

---

## 🧠 Auto-complete
- **Tab** → Auto-complete file/command  
- **Tab (twice)** → Show suggestions  

---

## 🔧 Custom Hotkeys (Advanced)

Create a custom keybinding:
```bash
bind '"\C-x\C-e": edit-and-execute-command'
