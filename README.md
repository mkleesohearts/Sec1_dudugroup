# Sec1_dudugroup

Tutorial Document (README.txt)
OS Optimization Simulation: 
This program tracks the usage of applications on your computer by periodically logging the names of running processes. It analyzes the collected data to identify which applications are consuming the most time over the past 24 hours, and provides an export of the analysis in multiple formats (TXT, JSON, YAML, Markdown, XML).
Features
Logs the running applications at regular intervals (every 5 minutes).
Analyzes usage data over the past 24 hours.
Identifies applications exceeding a specified usage threshold (60 minutes).
Visualizes the top 10 most-used applications in the last 24 hours with a bar chart.
Exports the analysis results to multiple formats: 
TXT
JSON
YAML
Markdown
XML.
Requirements
psutil: For getting the list of currently running processes.
pandas: For data manipulation and analysis.
matplotlib: For generating the bar chart visualization.
yaml: For exporting to YAML format.
xml.etree.ElementTree: For exporting to XML format.
platform: For identifying the operating system and ignoring system processes.
How to Use (on Google Colab)
Install the required libraries:
 !pip install psutil pandas matplotlib pyyaml
Upload this Python script to your Colab environment.
Run the code to start tracking app usage.
Check the results and exported files after the program runs.
Configuration Settings
Logging Interval: 5 minutes
Usage Analysis Period: 24 hours
Usage Limit per App: 60 minutes
Files Created
app_usage.csv — logs app names with timestamps
app_usage.txt — plain text report
app_usage.json — JSON format report
app_usage.yaml — YAML format report
app_usage.md — Markdown format report
app_usage.xml — XML format report
Notes
The program skips system processes depending on your operating system (Windows, Linux, or Mac).
This script is meant for personal use on your own computer. Do not use it to track others without permission.
