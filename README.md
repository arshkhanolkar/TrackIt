# **📚 TrackIt: The Customizable Study Time Tracker**

TrackIt is a modern, cross-platform desktop application designed to help you efficiently log, track, and visualize the time you spend on various subjects or activities. Built with Python and the CustomTkinter framework, it offers a clean user interface and powerful data management tools.

## **✨ Features**

* **Subject-Based Time Logging:** Easily record your time against custom-defined subjects (e.g., Math, Physics, Project A).  
* **Daily Goal Tracking:** Set a target daily study duration and monitor your progress in real-time.  
* **Historical Data View:** Review your logged sessions and total time spent over different periods.  
* **In-Depth Visual Analytics:** Leverage Matplotlib to generate a **variety of detailed and insightful charts** including Pie Charts for time distribution, Bar Charts for daily performance, and Line Graphs for long-term trend analysis. **This variety is TrackIt's core strength for actionable insights.**  
* **Persistent Storage:** All tracking data is saved securely to a local CSV file, ensuring your history is always preserved.  
* **Customizable UI:** A modern, customizable look and feel using CustomTkinter.

## **💻 Requirements**

To run TrackIt from the source code, you must have Python installed, along with the required libraries.

### **Prerequisites**

* **Python 3.x**  
* **pip** (Python package installer)

### **Installation**

Clone the repository and install the dependencies:

\# Assuming you have the TrackIt 4.3.py file in a directory  
\# Or, if it's a repository:  
\# git clone \<your-repo-url\>  
\# cd \<your-repo-directory\>

\# Install required Python packages  
pip install customtkinter  
pip install matplotlib  
pip install pillow

## **🚀 Usage**

### **Running the Application**

You can start the application directly from the source file:

python "TrackIt 4.3.py"

### **Key Workflow**

1. **Subject Management:** Go to the **Settings** or **Configuration** section to define the subjects or activities you want to track (e.g., "History," "Coding," "Reading").  
2. **Set Your Daily Goal:** Define your target daily minutes for tracking (e.g., the default is set to 690 minutes, or 11.5 hours).  
3. **Start/Stop Tracking:** On the main screen, select your current subject and press the **Start** button. When you finish your session, press **Stop**. The time will be recorded.  
4. **View Statistics:** Navigate to the **Stats** or **Reports** tab to see your cumulative progress and access the in-depth visual reports.

## **📊 Detailed Visual Analytics (Your Key to Insight)**

TrackIt's true power lies in its deep, customizable visual reporting, ensuring you move beyond simple time logs to understand *how* you use your time. The application provides several distinct graphical views to deliver actionable insights:

### **1\. Subject Distribution (Pie Chart)**

This chart breaks down your total logged time across all your defined subjects. It offers an immediate, proportional view of where your effort is concentrated, helping you visualize resource allocation and identify under- or over-prioritized areas.

### **2\. Daily Performance vs. Goal (Bar Chart)**

A powerful daily summary chart compares the total time you logged against your **Daily Goal**. It's perfect for quickly seeing when you hit your targets, providing motivating, day-by-day feedback on your consistency.

### **3\. Long-Term Trends (Line Graph)**

Track your study habits over weeks or months. This view uses line graphs to show patterns and progress, allowing you to easily spot trends—whether your focus is increasing, decreasing, or if you have specific days of the week where you are more productive.

### **4\. Subject Comparison**

Allows you to visually select and compare the cumulative time spent between any two chosen subjects. This is ideal for ensuring balanced effort across complex projects or multiple course loads.

## **🗄️ Data Management**

### **Data Location**

All your tracked data is automatically managed in a local file. This file contains the complete history of your logging sessions.

* **Data File:** tracking\_data.csv (The application will create this file in the same directory it runs from).

### **Debugging and Logging**

The application includes an internal logging system for error reporting and debugging. If you encounter any issues, please refer to this file:

* **Log File:** trackit\_debug.log

## **⚙️ Configuration & Customization**

The core configuration settings are managed within the application's interface, but the underlying source file contains the defaults:

| Constant | Description | Default Value | Notes |
| :---- | :---- | :---- | :---- |
| DEFAULT\_SUBJECTS | Initial subjects available for tracking. | \["Math", "Physics", "Chemistry"\] | Can be edited in the app's settings panel. |
| DEFAULT\_DAILY\_GOAL | Target study time in minutes. | 690 minutes (11.5 hours) | Adjust this to reflect your personal goals. |

You can modify these default values directly in the TrackIt 4.3.py file before running, or you should be able to update them via the in-app settings.

## **📦 Building an Executable**

TrackIt is designed to be easily packaged into a standalone executable (for Windows, macOS, or Linux) using tools like **PyInstaller**. This is why the code includes logic for handling resources like the icon file.

**To build your own executable:**

1. Install PyInstaller: pip install pyinstaller  
2. Run the build command (example for a single-file build):  
   pyinstaller \--onefile \--windowed "TrackIt 4.3.py"  
