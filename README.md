**How to gather a ProcessMonitor log**
**Summary**
This article will guide you on how to gather a ProcessMonitor log. This is a tool that is useful mainly for troubleshooting what files are being opened on your computer, and what keys are being looked at in your registry.

**1. Download ProcessMonitor from here: https://download.sysinternals.com/files/ProcessMonitor.zip**
**2. https://learn.microsoft.com/en-us/sysinternals/downloads/process-explorer**
To gather a **Process Monitor** (ProcMon) log, follow these steps:

### Step 1: Download Process Monitor
1. Go to the official **Microsoft Sysinternals** website: [Process Monitor](https://learn.microsoft.com/en-us/sysinternals/downloads/procmon).
2. Download the **ProcMon** tool and extract the contents of the ZIP file.

### Step 2: Run Process Monitor
1. Right-click on **Procmon.exe** and select **Run as administrator**. Process Monitor requires administrative privileges to monitor all system processes.
2. Once opened, Process Monitor will start capturing events automatically. You’ll see a constant stream of system activity.

### Step 3: Configure Filters (Optional but Recommended)
To focus on the specific processes or activities, set filters:
1. Click on the **Filter** icon or go to **Filter > Filter...**.
2. Define the filter conditions:
   - For example, if you want to monitor a specific process like `chrome.exe`, set the filter:
     - **Condition:** `Process Name`
     - **Operator:** `is`
     - **Value:** `chrome.exe`
     - **Action:** `Include`
3. Click **Add** and then **OK** to apply the filter. This will limit the log to relevant activities.

### Step 4: Start Capturing Logs
- If you stopped the capture earlier, click on the **Capture** icon (the magnifying glass) or press **Ctrl + E** to resume the log capture.
- Reproduce the issue or behavior you want to monitor.

### Step 5: Stop the Capture
1. Once the issue has been reproduced or the required data is captured, stop the logging by pressing **Ctrl + E** or clicking the **Capture** icon again.

### Step 6: Save the Log
1. Go to **File > Save**.
2. In the **Save As** dialog, select the following options:
   - **Events to save:** All events or filtered events (based on your need).
   - **Format:** Select **Native Process Monitor Format (.PML)** to save a full detailed log or **Comma Separated Values (.CSV)** for a text-based log.
3. Choose a location to save the log and click **Save**.

### Step 7: Share the Log (if needed)
- The generated `.PML` or `.CSV` file can now be shared for further analysis.

### Additional Tips:
- **Clearing the Display:** If the screen becomes too cluttered, click **Edit > Clear Display** to start with a fresh view.
- **Auto Scroll:** Disable **Auto Scroll** if you want to review the logs while they are being captured (under **Options**).

This process will capture detailed information about file system, registry, and network activity, helping to troubleshoot issues or analyze system behavior.



















