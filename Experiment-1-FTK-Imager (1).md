# 🧪 Lab Exercise 1: Collecting Evidence with FTK Imager

**Subject:** Digital Forensics Laboratory  
**Experiment ID:** 01  
**Topic:** Evidence Acquisition through FTK Imager  

---

### 🎯 Objective
To acquire live (volatile) memory and create a forensic image of a storage device using FTK Imager.

---

### 🛠️ Tools & Environment
- **Software:** FTK Imager  
- **Platform:** Windows OS  

---

### 📘 Overview
FTK Imager is a widely used forensic utility that enables investigators to capture system memory and generate exact disk images.  
- It helps preserve original data without modifications.  
- Analysts can preview, save, and later examine the extracted content during investigations.  

---

## Part A — Capturing Volatile Memory (RAM)

**Step 1:** Launch FTK Imager with administrator rights.  

![Step 1](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.55_983ae60c.jpg?raw=true)

**Step 2:** From the top menu, navigate to **File → Capture Memory**.  

![Step 2](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.56_3c886fdd.jpg?raw=true)

**Step 3:** A window will pop up. Specify the storage location, choose a filename ending in `.mem`, and optionally include pagefile or AD1 output.  

![Step 3](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.56_6e410aaa.jpg?raw=true)

**Step 4:** Press **Capture Memory** to begin the process.  

![Step 4](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.56_6ec5cadd.jpg?raw=true)

**Step 5:** A green progress bar will display the acquisition status. Duration depends on total RAM size. Once finished, the `.mem` file appears at the selected destination.  

![Step 5](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.57_87d83979.jpg?raw=true)

---

## Part B — Imaging Non-Volatile Storage (Disk Acquisition)

**Step 1:** Go to **File → Create Disk Image**.  

![Step B1](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.56_3c886fdd.jpg?raw=true)

**Step 2:** Select the evidence source type (e.g., Physical Drive, Logical Drive, Image File, or Folder).  

![Step B2](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.57_61f840f9.jpg?raw=true)

**Step 3:** Pick the drive you wish to capture and click **Finish**.  

![Step B3](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.57_56ce71b2.jpg?raw=true)

**Step 4:** In the next window, press **Add** to choose an image format.  

![Step B4](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.58_0a038f70.jpg?raw=true)

**Step 5:** Select the image type (Raw / SMART / E01 / AFF).  
> Recommendation: **E01** is commonly preferred.  

![Step B5](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.57_56ce71b2.jpg?raw=true)

**Step 6:** Provide case details (Case ID, Evidence ID, Examiner, Description, Notes), then click **Next**.  

![Step B6](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.58_0a038f70.jpg?raw=true)

**Step 7:** Choose a storage path and set a filename for the image.  

![Step B7](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.57_a329330e.jpg?raw=true)

**Step 8:** Configure options (compression, split size, etc.), then press **Finish** and afterwards **Start**.  

![Step B8](https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.58_ba2291db.jpg?raw=true)

During imaging, FTK Imager calculates and verifies hash values. If acquisition is successful, the verification hashes will match, proving integrity of the evidence.  

---
