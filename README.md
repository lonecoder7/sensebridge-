# Sensebridge Image Dataset
---

## 1. Document & Dataset Metadata
* **Project Reference:** Sensebridge
* **Dataset Size:** 1.26 GB (1,354,176,060 bytes)
* **Total Records:** 1,135 Image Files
* **Asset Formats:** `.jpg`, `.jpeg`, `.png`, `.heic`
* **Version:** 1.0.0
* **Storage Engine:** Git Large File Storage (LFS) v3.x

---

## 2. Directory Integrity & Web Interface Notice
This repository stores the structural integrity of the primary dataset using tracking hashes. 

Please note a structural behavioral trait of the GitHub web interface layout:
* **Web Browser Constraints:** The GitHub web graphical user interface (UI) enforces a native visualization ceiling of 1,000 files per subdirectory. 
* **Truncation Status:** For directories exceeding this threshold, the UI appends the warning: *"Sorry, we had to truncate this directory to 1,000 files. 135 entries were omitted from the list."*
* **Verification:** This is strictly a browser rendering limitation. All 1,135 image files are fully tracked, hashed, and preserved cryptographically within the Git system tree. Local initialization or cloning (`git clone`) pulls the complete, un-truncated database.

---

## 3. Supplementary High-Availability Data Mirror
For review environments requiring rapid local access, bulk downloads, or testing outside of a Git version-controlled pipeline, a certified secondary distribution mirror is maintained below. 

The integrity of the files hosted on this mirror matches the cryptographic states of the assets tracked within this repository.

🔗 **[Access Primary Dataset File Mirror (https://drive.google.com/drive/folders/1jwadtEZZ3nCE4HqcyuXjVQWupoG8mSVo?usp=sharing)]**

---

## 4. Technical Architecture & Environment
The dataset is tracked via standard configuration policies to guarantee version permanence.

### 4.1 Large File Configuration (`.gitattributes`)
Binary image data tracking is explicitly managed to decouple large payload distribution from textual system trees:
```ini
*.jpg filter=lfs diff=lfs merge=lfs -text
*.jpeg filter=lfs diff=lfs merge=lfs -text
*.png filter=lfs diff=lfs merge=lfs -text
*.heic filter=lfs diff=lfs merge=lfs -text
```

### 4.2 Local Reconstitution Instructions
To pull down the complete, untruncated 1,135-file baseline locally for audit confirmation, execute:
```bash
git lfs install
git clone https://github.com
```
