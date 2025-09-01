
# Experiment-1: Evidence Acquisition Using FTK Imager

**Course / Lab:** Digital Forensics Lab  
**Experiment No.:** 1  
**Title:** Evidence Acquisition Using FTK Imager  

---

## Aim
To capture RAM data and create a forensic disk image using FTK Imager.

---

## Requirements
- FTK Imager  
- Windows operating system  

---

## Description
- FTK Imager is a forensic acquisition tool used to create exact copies (disk images) of storage devices.  
- It allows capturing RAM data, entire drives, or specific partitions without altering original evidence.  
- Investigators use it to preview, preserve, and export data for further forensic analysis.  

---

## Part A — Acquiring Volatile Memory (RAM) Using FTK Imager

**Step-1:** Right click on the FTK Imager tool and select **Run as administrator**.  

https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.55_983ae60c.jpg
**Step-2:** On the top menu bar, click **File** and select **Capture Memory** from the drop-down list.  

https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.56_3c886fdd.jpg
**Step-3:** A dialog box will appear. Select the destination path to your file and provide the file name with `.mem` extension. (Pagefile and AD1 file options are optional.)  

https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.56_6e410aaa.jpg
**Step-4:** Click the **Capture Memory** button to start acquisition of memory.  

https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.56_6ec5cadd.jpg
**Step-5:** A progress bar in green colour will indicate the capture status. The time taken to capture RAM depends on the system’s RAM size. After completion, the captured memory file will be available in the chosen destination folder.  

https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.57_87d83979.jpg

---

## Part B — Acquiring Non-Volatile Memory (Disk Image) Using FTK Imager

**Step-1:** On the top right menu bar, click **File** and select **Create Disk Image** from the drop-down menu.  

https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.56_3c886fdd.jpg
**Step-2:** In the dialog box, choose the source evidence type like **Physical Drive, Logical Drive, Image File, or Contents of a folder**.  

https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.57_61f840f9.jpg
**Step-3:** Select the drive you want to image and click **Finish**.  

https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.57_56ce71b2.jpg
**Step-4:** In the **Create Image** dialog, click **Add** to define image type. 

https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.58_0a038f70.jpg

**Step-5:** Select the image type from the dialog box (Raw / SMART / E01 / AFF). Among all, **E01 is recommended**. 
https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.57_56ce71b2.jpg
**Step-6:** Fill in the case information (Case Number, Evidence Number, Examiner Name, Unique Description, Notes) and click **Next**.  

https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.58_0a038f70.jpg
**Step-7:** Choose the destination folder and give a file name for the image.  
https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.57_a329330e.jpg
**Step-8:** Set options like compression, splitting size, and click **Finish**. After that, click **Start** to begin the imaging process.  

https://github.com/99230040236-byte/DF/blob/c0bfb139841542aacf47cd3a54b630f6464b46e1/exp1/WhatsApp%20Image%202025-09-01%20at%2022.47.58_ba2291db.jpg

FTK Imager will display progress along with hash values. The imaging process may take time depending on the drive size. After completion, FTK Imager verifies the hash values automatically to maintain forensic integrity. Finally, the hash values should match.  

---

  

