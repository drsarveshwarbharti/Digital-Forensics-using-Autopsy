### For your educational exploration of Autopsy on Windows, here are some excellent sources offering free forensic disk images—perfect for hands-on learning:

### 1. NIST CFReDS (Computer Forensic Reference Data Sets)

The CFReDS portal provides a variety of curated forensic images designed for education and tool testing. 
cfreds.nist.gov

A few publicly available examples include:

nps-2009-canon2 – digital camera-based file carving scenarios

nps-2009-ntfs1 – NTFS system with various file states (fragmented, compressed, encrypted)

nps-2009-domexusers – a Windows XP SP3 disk with user communication artifacts 
digitalcorpora.org

These are safe, anonymized, and ideal for educational use.

### 2. Digital Corpora – NPS Test Disk Images & Scenarios

The Digital Corpora repository includes:

The same NPS test images

Several scenario-driven sets like M57-Jean (executive laptop exfiltration scenario)

Nitroba University Harassment, M57-Patents, and more 
digitalcorpora.org

These provide rich, realistic cases that enhance learning via meaningful context.

### 3. DFIR Training Test Images

The DFIR.training site hosts terabytes of sample images, including:

USB, mobile device, cloud, network, and multimedia images

Challenge-based “CTF-style” datasets 
dfir.training

Excellent for simulating real-world investigations or class assignments.

### Quick Comparison
Source	Notable Examples	Best For
NIST CFReDS	nps-2009-* test images	Reliable, curated educational datasets
Digital Corpora	NPS + full scenarios (M57, etc.)	Scenario-based learning and practice
DFIR.training	Device, cloud, multimedia, challenge datasets	Broader exploration and higher complexity
What to Use First?

Start simple: Grab a manageable NPS image like nps-2009-ntfs1 or nps-2009-canon2.

Practice ingesting in Autopsy: Load it as a data source, run ingest modules (Recent Activity, File Types, Keyword Search), explore artifacts.

Scale up: Move on to scenario sets like M57 or Nitroba from Digital Corpora for more depth and storytelling.

Challenge yourself: Download DFIR.training challenge packs when you're comfortable and want advanced puzzles to solve.

### Quick Download Tips (Windows)

Browse to the NIST CFReDS portal and download test images via direct links.

For Digital Corpora, navigate to the “Disk Images” section and pick a scenario.

On Autopsy, choose “Add Data Source > Disk Image or VM File” and point to the downloaded .E01 or .dd file.
