## Step-by-step Quick Start for Autopsy 
### (The digital forensics tool )

### 1) Install Autopsy
•	Windows: Download the current Windows installer from the official site and run it. As of now, the site lists Autopsy 4.x with a one-click 64-bit installer. Autopsy+1

•	Linux / macOS: Autopsy 4 runs, but you install via ZIP + extra dependencies (Sleuth Kit, Java, etc.). Follow the platform notes; on macOS/Linux you typically build or install Sleuth Kit separately. Autopsyslo-sleuth.github.io
Recommended resources / prerequisites

•	System memory: 16 GB RAM recommended; you can raise Autopsy’s JVM memory later via Tools → Options → Application → Maximum JVM Memory. Sleuth Kit
 
### 2) Launch & create a case
1.	Open Autopsy → Create New Case.
2.	Fill in Case Name, choose a Base Directory, and (optionally) Case Number / Examiner.
3.	Finish to create the empty case.
A “case” can hold one or many data sources (images, drives, logical folders). Sleuth Kit
 
### 3) Add a data source
Choose Add Data Source and pick one of:
•	Disk Image / VM (E01, RAW/DD, VMDK, VHD, etc.)
•	Local Disk/Device (attached drive)
•	Logical Files (folders/files you exported elsewhere) Sleuth Kit
Point Autopsy at the file/device and proceed.
 
### 4) Select ingest modules (the analysis plug-ins)
On the Ingest Modules screen, tick what you need. Common starters:
•	Recent Activity (browser history, downloads, logins, etc.)
•	File Type Identification
•	Hash Lookup (with NSRL or your own hash sets)
•	Keyword Search (indexing for fast text search)
•	EXIF/Metadata (pictures, docs)
These modules parse files and generate artifacts while data is added/ingested. You can re-run modules later on selected data if needed. Sleuth KitGitHub
Tip: Start with Recent Activity + Keyword Search for a quick overview; add heavier modules (full hash lookups, carving) once you see where to dig.
 
### 5) Let ingest run & watch progress
You’ll see progress in the lower right. As modules finish, results appear in the left Data Sources / Views tree.
 
### 6) Explore key views (the daily workflow)
•	Results / Artifacts: consolidated findings from modules (web history, accounts, installed apps, etc.).
•	File Types / MIME: pivot by type (docs, images, archives…).
•	Keyword Hits: terms matched during indexing.
•	Timeline: sequence events across the case to see activity bursts.
These are standard Autopsy UI areas you’ll use in almost every case.
 
### 7) Search, filter, and carve
•	Use Keyword Search (indexed) for fast text queries.
•	Apply Filters (time range, file type, known/unknown files, tags).
•	Use File Search by Attributes (size/date/hash) when narrowing large sets.
(These capabilities are provided by built-in modules and UI tools.) 
 
### 8) Tag, comment, and bookmark
Right-click items → Add Tag or Add Comment to keep your findings organized. Tags drive your reports later.
 

### 9) Generate reports
Go to Tools → Generate Report and pick formats (HTML, CSV, KML, etc.) and which artifacts/tags to include. Report modules are part of Autopsy’s plug-in system. 
 
### 10) Adjust settings as your case grows
•	Raise memory (if you hit “Out of memory” or sluggish indexing): Tools → Options → Application → Maximum JVM Memory. 
•	Add/disable modules anytime from the Ingest panel if you need deeper or faster passes. 
 
### (Optional) Multi-user / bigger setups
Autopsy supports a multi-user configuration (PostgreSQL, ActiveMQ, Solr) so multiple examiners can work the same case; the docs include suggested hardware for those roles. Only set this up if you truly need collaboration at scale. Sleuth Kit+1
 
### Troubleshooting cheatsheet
•	“Can’t open image” / dependencies (macOS/Linux): confirm Sleuth Kit/Java versions per platform notes. slo-sleuth.github.io
•	Very slow ingest: start with fewer modules; add more after initial triage.
•	Search returns nothing: ensure Keyword Search ran; if not, (re)run it on the data source. 
•	Memory errors: increase JVM memory in Tools → Options. 
 
### Download & docs (official)
•	Autopsy site & downloads: official homepage and download page. 
•	User docs (cases, installation, modules): official user documentation.

