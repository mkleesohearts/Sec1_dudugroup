# Sec1_dudugroup

**Tutorial Document (README.txt)**  
**OS Optimization Simulation:**  
This program tracks the usage of applications on your computer by periodically logging the names of running processes. It analyzes the collected data to identify which applications are consuming the most time over the past 24 hours, and provides an export of the analysis in multiple formats (TXT, JSON, YAML, Markdown, XML).  

**Features**  
Logs the running applications at regular intervals (every 5 minutes).<br>
Analyzes usage data over the past 24 hours.<br>
Identifies applications exceeding a specified usage threshold (60 minutes).<br>
Visualizes the top 10 most-used applications in the last 24 hours with a bar chart.<br>
Exports the analysis results to multiple formats: <br>
- TXT  
- JSON  
- YAML  
- Markdown  
- XML  

**Requirements**  
`psutil`: For getting the list of currently running processes.<br>
`pandas`: For data manipulation and analysis.<br>
`matplotlib`: For generating the bar chart visualization.<br>
`yaml`: For exporting to YAML format.<br>
`xml.etree.ElementTree`: For exporting to XML format.<br>
`platform`: For identifying the operating system and ignoring system processes.<br>

**How to Use (on Google Colab)**  
Install the required libraries:<br>
`!pip install psutil pandas matplotlib pyyaml`<br>
Upload this Python script to your Colab environment.<br>
Run the code to start tracking app usage.<br>
Check the results and exported files after the program runs.<br>

**Configuration Settings**  
Logging Interval: 5 minutes<br>
Usage Analysis Period: 24 hours<br>
Usage Limit per App: 60 minutes<br>

**Files Created**  
`app_usage.csv` — logs app names with timestamps<br>
`app_usage.txt` — plain text report<br>
`app_usage.json` — JSON format report<br>
`app_usage.yaml` — YAML format report<br>
`app_usage.md` — Markdown format report<br>
`app_usage.xml` — XML format report<br>

**Notes**  
The program skips system processes depending on your operating system (Windows, Linux, or Mac).<br>
This script is meant for personal use on your own computer. Do not use it to track others without permission.<br>
