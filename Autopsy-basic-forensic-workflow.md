### Windows-focused step-by-step to get Autopsy up and running for educational / learning use.

### 🚀 Autopsy basic forensic workflow

### 1. Download & Install

Go to the official Autopsy download page

Grab the latest Windows 64-bit installer (MSI).

Run the installer → follow the wizard (it includes Sleuth Kit & required dependencies).

No extra setup needed on Windows.

After install, launch Autopsy from the Start Menu.

### 2. Create Your First Case

Autopsy opens with the Case Wizard.

Click “New Case”.

Enter:

Case Name (e.g., EduDemo)

Base Directory (where case files are stored, e.g., C:\AutopsyCases)

Case Number & Examiner Name (optional, for reports).

Click Finish → you now have an empty case.

### 3. Add a Data Source

For learning, you can:

Use a sample disk image (e.g., .E01, .dd, .img) → many free forensic images are online for training.

Or add a simple folder of files you want to analyze.

Steps:

In the wizard → choose “Disk Image or VM File” OR “Logical Files”.

Browse and select your file/folder.

Click Next.

### 4. Choose Ingest Modules

Autopsy asks which modules (plug-ins) to run. For educational use, start with:

✅ Recent Activity → pulls browser history, logins, downloads.

✅ File Type Identification → sorts files by type.

✅ Keyword Search → makes everything searchable.

✅ EXIF Metadata → extracts photo metadata.

(You can tick more later, but these run quickly and give good results.)

### 5. Let Autopsy Process

Autopsy will start “ingest” (analysis).

Progress is shown in the bottom right.

As results come in, the left Tree View fills up.

### 6. Explore the Results

In the left panel, you’ll see:

Data Sources (the drives/files you added)

Results → artifacts from modules:

Web History

Accounts

Installed Programs

File Types → sorted docs, images, archives

Keyword Hits → matches from the index

Double-click to open items; right-click → View in Explorer, Extract, or Tag.

### 7. Tag & Comment

Right-click any file → Add Tag → choose category (e.g., “Interesting”).

Add notes for later reporting.

### 8. Generate a Report

Go to Tools → Generate Report.

Pick a format (HTML is easiest for learning).

Choose what to include (e.g., tagged files, web history).

Open the generated HTML file in your browser.

### 9. Adjust for Classroom Use

If your PC has ≥16 GB RAM, increase Autopsy’s memory:

Tools → Options → Application → Maximum JVM Memory.

Use sample forensic images (like the famous “NIST CFReDS” datasets) for safe practice.

### 10. Done 🎉

#### You’ve just gone through the basic forensic workflow:

#### Create Case

#### Add Data

#### Run Modules

#### Explore & Tag

#### Report
