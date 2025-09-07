# Javascript Folder Sorter

<a href="https://www.linkedin.com/posts/anshprogrammer_your-messy-folders-have-a-solution-anyone-activity-7370431977063317504-8Y15?utm_source=share&utm_medium=member_desktop&rcm=ACoAADlrQCgBJlIdPj0s2Rx7FxIB11A0tKoryNs"> Explanation Video on linkedin </a>

Tired of having a chaotic Downloads folder? This simple Node.js script is here to help! It automatically organizes all your files into separate folders based on their extensions. It's a lifesaver for anyone who loves a clean and organized digital space.

---

## How It Works

This script uses the built-in `fs` (File System) module to scan a folder you specify. It then iterates through each file, grabs its extension (like `.pdf`, `.png`, or `.zip`), creates a new folder for that extension if one doesn't already exist, and moves the file there.

---

## How to Use It

1.  **Clone this repository** to your local machine.

2.  **Open your terminal** (like VS Code's terminal) and navigate to the project directory.

3.  **Run the script** with the command:
    ```bash
    node folders.js
    ```

4.  **Paste the folder path** you want to organize. The script will prompt you for the path. Just make sure to paste the path **without quotation marks**.

    * **Example (correct):** `C:\Users\YourName\Downloads`
    * **Example (incorrect):** `"C:\Users\YourName\Downloads"`

5.  **Press Enter** and watch the magic happen! The script will create folders like `pdf`, `jpg`, and `zip` and move your files into them.

---

## Important Notes

* **Permissions are key!** If you get a permission-denied error (`EPERM`), it's likely because you're trying to move a file or folder that's currently in use or requires administrator access. Try closing any open programs or running your terminal with administrator privileges.
* **System files**: The script organizes files based on their extensions, but it's a good idea to double-check that you're not trying to organize a folder that contains system-critical files. For instance, the `flutter_windows_3.22.2-stable` folder that some of you might have in your Downloads folder is a program, not a regular collection of files, and should be left untouched.
