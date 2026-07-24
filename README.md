# 🧹 Dead Entry Cleaner (BETA)

A smart utility for removing ghost entries from Aurora without affecting your games or legitimate content.

---

## 📌 About

**Dead Entry Cleaner** was developed to automatically clean Aurora's database by removing invalid entries that can cause issues such as:

* Games that appear in the library but won't launch
* Duplicate or "ghost" entries
* A cluttered or corrupted game library

The tool works directly on Aurora's **ContentItems** database, removing only invalid records based on multiple safety checks.

---

## 🖼️ Preview

### Script Selection

<p align="center">
  <img src="assets/screenshot1.png" width="800"/>
</p>

### Safety Checklist

<p align="center">
  <img src="assets/screenshot2.png" width="800"/>
</p>

### Storage Device Selection

<p align="center">
  <img src="assets/screenshot3.png" width="800"/>
</p>

### Device Confirmation

<p align="center">
  <img src="assets/screenshot4.png" width="800"/>
</p>

### Removal Confirmation

<p align="center">
  <img src="assets/screenshot5.png" width="800"/>
</p>

### Final Results (Summary)

<p align="center">
  <img src="assets/screenshot6.png" width="800"/>
</p>

---

## 🧠 Key Features

* 🧹 Removes **ghost entries (invalid ContentItems)**
* 🔍 Smart detection based on:

  * Missing directories
  * Missing executable files (`.xex`)
  * Invalid GOD content
  * Empty directories
* 🛡️ Advanced protection system to prevent accidental removal
* 👁️ Preview detected entries before deletion
* 📊 Displays a final report including:

  * Entries analyzed
  * Entries removed
  * Failed operations

---

## 🛡️ Safety

* ✔️ Does **not** remove physical files from your storage device
* ✔️ Does **not** delete games, DLCs, or Title Updates
* ✔️ Automatically protects:

  * Aurora
  * XexMenu
  * DashLaunch
  * Emulators
  * Homebrew applications
  * Plugins and system services
* ✔️ Protected error handling using `pcall`
* ✔️ User confirmation is required before any removal

> ⚠️ **Important:**
> This script only removes records from Aurora's database. It does **not** delete any actual files.

---

## 📦 When to Use

Use this script when:

* 🎮 Games appear in Aurora but won't launch
* 👻 Ghost entries are present in the library
* 🔁 You have manually moved or deleted games
* 🧱 Aurora's library has become corrupted or inconsistent
* 📂 Duplicate or invalid entries are present

---

## 📂 Backup (Recommended)

Before running the script, back up one of the following database files:

```text
Data\Databases\content.db
```

or

```text
User\Data\Databases\content.db
```

---

## ⚙️ How It Works

1. Review and confirm the safety checklist.
2. Select the storage device (required due to Aurora's limitations).
3. The script scans the entire database.
4. Invalid entries are identified through multiple validation checks.
5. A preview of the detected entries is displayed.
6. Only confirmed entries are removed.
7. A final summary is presented.

---

## 🔄 Recommendation

After the script completes:

* 🔁 Restart Aurora (the script offers this option automatically).
* ⚙️ Keep **automatic scanning enabled** so Aurora can rebuild the library correctly.

---

## ⚠️ Limitations

* Partially valid content is intentionally preserved to prioritize safety.
* Some protected entries may be skipped even if they appear to be broken.
* Library reconstruction still depends on Aurora's scanning system.

---

## 💡 Notes

* Running the script again may find additional invalid entries if Aurora's automatic scan recreates database records.
* The cleaning process is designed to be safe rather than aggressive, avoiding the removal of anything suspicious.
* Storage device selection exists due to Aurora's internal limitations, but the cleanup is applied to the database as a whole.

---

## ⚠️ Disclaimer

Use this tool only when necessary.

Direct modifications to Aurora's database may cause inconsistencies if performed outside its intended use.

---

## 📌 Status

🟡 **BETA** — Currently under testing, but fully functional and safe for regular use.

---

## 💬 Contributing

Suggestions, improvements, bug reports, and feedback are always welcome!
