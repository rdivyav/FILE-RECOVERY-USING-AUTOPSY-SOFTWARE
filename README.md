# FILE-RECOVERY-USING-AUTOPSY-SOFTWARE
```
Name: Divya R V
Reg no : 212223100005
```
## AIM
To use **Autopsy Digital Forensics Tool** to retrieve deleted files from a disk image.

---

## REQUIREMENTS
- **Operating System**: Windows 10/11, macOS, or Linux
- **Tool**: [Autopsy Digital Forensics](https://www.autopsy.com/)  
- **Test Data**: Disk image file (`disk.dd`, `disk.img`, `.E01`)

---

## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Install Autopsy]
    B --> C[Create New Case in Autopsy]
    C --> D[Add Data Source: Disk Image]
    D --> E["Run File System & Data Recovery Modules"]
    E --> F[Locate Deleted Files in Results]
    F --> G[Recover and Export Deleted Files]
```
## DESIGN STEPS:
### Step 1:
Open Autopsy and create a new case with appropriate case details.

### Step 2:
Add a disk image as a data source and let Autopsy analyze the content.

### Step 3:
Navigate to the "Deleted Files" section in Autopsy and examine or recover the deleted files.

## PROGRAM:
### Install Autopsy
```bash
# Download Autopsy from:
# https://www.autopsy.com/
# Install following the setup wizard.
```
### Create a New Case
```
# File → New Case
# Enter Case Name: Deleted_File_Recovery
# Choose Base Directory: C:\Cases\Deleted_File_Recovery
# Click Finish
```
### Add Disk Image
```
# Add Data Source → Disk Image or VM File
# Browse to: C:\forensics\disk.dd
# Click Next
```
### Run Ingest Modules
```# Select:
# - File System Analysis
# - Keyword Search (optional)
# - Data Recovery / Carving
# Click Finish
```
### Locate Deleted Files
```
# Navigate to 'Deleted Files' section in the tree view
# Review metadata (size, hash, timestamps)
```
### Export Deleted Files
```
# Right-click → Extract File(s)
# Save to: C:\forensics\Recovered_Files\
```

## OUTPUT:
Recovered Deleted File List and Details

<img width="1920" height="1080" alt="Screenshot 2025-09-04 104546" src="https://github.com/user-attachments/assets/89cb6343-12a0-41bb-9e40-8d96e6328fde" />

<img width="1920" height="1080" alt="Screenshot 2025-09-04 104605" src="https://github.com/user-attachments/assets/bdefc6a2-b7b4-4f81-a3a0-fd164968fef7" />

<img width="1920" height="1080" alt="Screenshot 2025-09-04 104647" src="https://github.com/user-attachments/assets/13c9abb8-7c4d-42c3-aa3d-599f3c5492c8" />

<img width="1920" height="1080" alt="Screenshot 2025-09-04 104705" src="https://github.com/user-attachments/assets/3e06e40b-da3b-4169-b0d3-1c887dc9de3d" />

<img width="1920" height="1080" alt="Screenshot 2025-09-04 104743" src="https://github.com/user-attachments/assets/0b6e4191-1c6d-47b8-b1de-de1f1efdda9f" />

<img width="1920" height="1080" alt="Screenshot 2025-09-04 104810" src="https://github.com/user-attachments/assets/5da26c41-98bc-4570-a21d-ce09657b2172" />

<img width="1920" height="1080" alt="Screenshot 2025-09-04 105439" src="https://github.com/user-attachments/assets/b208a226-802e-4f0b-bf4e-dba11d52a4e5" />

<img width="1920" height="1080" alt="Screenshot 2025-09-04 104950" src="https://github.com/user-attachments/assets/0a9aaedb-bf45-4916-bd6e-0400fe5772a6" />

<img width="1920" height="1080" alt="Screenshot 2025-09-04 105003" src="https://github.com/user-attachments/assets/982c891a-4b57-4cf0-9d17-543607da65c0" />


## RESULT:
Deleted files were successfully retrieved and analyzed using Autopsy.
