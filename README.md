# 🧹 Dead Entry Cleaner (BETA)

A smart utility that safely removes invalid Aurora database entries while preserving games, DLCs, Title Updates, homebrew, and other legitimate content.

---

## 📌 About

**Dead Entry Cleaner** was developed to automatically clean Aurora's database by identifying and removing invalid **ContentItems** that no longer point to valid content.

Unlike a simple database cleanup, the script performs multiple validation checks before considering an entry invalid. It analyzes directory existence, executable files, GOD containers, installed content structure, and several protected scenarios to ensure only genuine dead entries are removed.

Every detected entry is presented to the user before deletion, allowing the cleanup process to remain transparent, safe, and fully controlled.

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

### Invalid Entries Preview

<p align="center">
  <img src="assets/screenshot5.png" width="800"/>
</p>

### Final Results (Summary)

<p align="center">
  <img src="assets/screenshot6.png" width="800"/>
</p>

---

## 🧠 Key Features

* 🧹 Removes invalid **ContentItems (ghost entries)** from Aurora's database.
* 🔍 Smart detection using multiple validation methods.
* 📁 Detects missing or inaccessible directories.
* 🎮 Detects missing executable (`.xex`) files.
* 💿 Detects invalid or incomplete GOD installations.
* 📂 Detects empty or broken content directories.
* 🛡️ Built-in protection for system applications and homebrew.
* 👁️ Preview every detected entry before removal.
* 📊 Displays a detailed cleanup report including:
  * Entries analyzed.
  * Invalid entries detected.
  * Entries successfully removed.
  * Failed operations.
* 🔁 Optionally restart Aurora after the cleanup.
* 🛡️ Protected database operations using `pcall`.

---

## 🛡️ Safety

Dead Entry Cleaner was designed with safety as the highest priority.

Every entry must pass multiple validation checks before being considered invalid.

The script **never removes files from your storage device**. Only invalid Aurora database records are removed.

Built-in protections include:

* ✔️ Never deletes physical files.
* ✔️ Never deletes games.
* ✔️ Never deletes DLC.
* ✔️ Never deletes Title Updates.
* ✔️ Never deletes save data.
* ✔️ Automatically protects Aurora.
* ✔️ Automatically protects XexMenu.
* ✔️ Automatically protects DashLaunch.
* ✔️ Automatically protects emulators.
* ✔️ Automatically protects homebrew applications.
* ✔️ Automatically protects plugins and system services.
* ✔️ Protected database operations using `pcall`.
* ✔️ User confirmation is required before any removal.

> ⚠️ **Important:**
>
> This script only removes invalid **database records** from Aurora.
>
> No files stored on your HDD or USB device are ever modified or deleted.

---

## 📦 When to Use

Use this script when:

* 🎮 Games appear in Aurora but no longer exist.
* 👻 Ghost entries remain after deleting games manually.
* 🔁 Games were moved outside Aurora.
* 📂 Broken or invalid library entries are displayed.
* 🧹 You want to clean obsolete database entries safely.
* ⚠️ Aurora's library becomes inconsistent after manually organizing your storage.

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
2. Select the storage device (required due to Aurora's internal limitations).
3. The script scans the Aurora database and analyzes every registered ContentItem.
4. Each entry is validated using multiple safety checks to determine whether it still points to valid content.
5. A preview of all detected invalid entries is displayed before any modification is made.
6. After confirmation, only verified dead entries are removed from the database.
7. A detailed cleanup summary is displayed.
8. Optionally restart Aurora to immediately refresh the game library.

---

## 🔄 Recommendation

After the cleanup is complete:

* 🔁 Restart Aurora (the script offers this option automatically).
* 🔄 Allow Aurora to perform a new scan so any valid content can be detected again.
* 💾 If you recently moved or restored games, verify your Scan Paths before running another cleanup.

---

## ⚠️ Limitations

* Entries with partially valid data are intentionally preserved to maximize safety.
* Protected applications and system content are never removed, even if they appear to be invalid.
* The script only removes invalid database records. It does not rebuild Aurora's database or recreate missing entries.
* Aurora's library is refreshed only after restarting or performing a new scan.

---

## 💡 Notes

* Running the script again after Aurora completes a new scan may detect additional invalid entries created by previous database inconsistencies.
* The cleanup process prioritizes safety over aggressive removal, avoiding false positives whenever possible.
* Storage device selection exists because Aurora stores content references relative to the selected device, making device validation necessary before analyzing database entries.
* If no invalid entries are found, the script will simply report that the database is already clean.

---

## ⚠️ Disclaimer

Use this tool only when necessary.

Although every removal is validated through multiple safety checks, this script directly modifies Aurora's database. It is strongly recommended to create a backup before performing any cleanup.

Dead Entry Cleaner only removes invalid **ContentItems** from Aurora's database. No games, DLCs, Title Updates, save data, or other files stored on your device are ever modified or deleted.

---

## 📌 Status

🟡 **BETA** — Stable and safe for regular use, with continuous improvements planned for future releases.

---

## 💬 Contributing

Suggestions, improvements, bug reports, and feedback are always welcome!

If you encounter an issue or have ideas to improve **Dead Entry Cleaner**, feel free to open an **Issue** or submit a **Pull Request**.

Community contributions help improve the project and benefit the entire Aurora community.