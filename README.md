# Ex.No.5: Study of Prompt Templating Techniques for Automated Maintenance Report Generation
**Date:** 04-09-2025  
**Register Number:** 212223240068  


## 🎯 Aim
To explore and apply various prompt templating techniques to automate the generation of maintenance reports. This experiment focuses on creating a robust system that can translate raw sensor data and maintenance logs into structured, human-readable reports. By using templates, we can ensure consistency, accuracy, and efficiency in the reporting process, which is crucial for industries like manufacturing and logistics.



## ⚙️ Procedure

### 1. Define the Scenario
We focus on a manufacturing scenario where a key machine, such as a CNC (Computer Numerical Control) machine, requires regular maintenance. The system will receive data from two primary sources:  

- **IoT Sensors:** Real-time data on temperature, vibration, and energy consumption.  
- **Maintenance Logs:** Manual entries from technicians detailing repairs and part replacements.  

**Goal:** Generate a comprehensive report summarizing the machine's health, identifying potential issues, and documenting all maintenance activities.

<img width="512" height="512" alt="unnamed" src="https://github.com/user-attachments/assets/691113e3-96f8-4671-8f51-423a0258c1ec" />


### 2. Prompt Templating Techniques
We utilize three distinct prompt templating patterns to generate different sections of the maintenance report.

#### a) Single-Shot Prompting (Concise Summary)
- **Template:**  
> "Generate a one-paragraph summary of the machine's status. Include a mention of its performance, any anomalies detected, and the last maintenance date."

- **Example Input Data:**  
Performance: Stable, but vibration spike detected on [Date]. Last Maintenance: [Date].

- **Generated Report Snippet:**  
> "The CNC machine's performance has been stable, though a minor vibration spike was detected on [Date]. The last maintenance was performed on [Date]. The machine is operating within its normal parameters, but the anomaly should be monitored."





#### b) Role-Playing Prompting (Detailed Technical Analysis)
- **Template:**  
> "You are a senior maintenance engineer. Analyze the following data and write a detailed report section on the machine's health. Use technical language and provide actionable recommendations.  

Temperature Data: [Data]  
Vibration Data: [Data]  
Energy Consumption: [Data]  
Maintenance Log: [Data]"

- **Example Input Data:**  
Temperature: 75°C (normal), Vibration: 2.5 mm/s (spike detected), Energy: 15 kWh (normal), Log: [Date], Replaced bearing.

- **Generated Report Snippet:**  
> "Technical Analysis: The thermal telemetry indicates normal operating temperatures. However, the vibration sensor data shows a peak of 2.5 mm/s on [Date], which is atypical for this machine's operational baseline. This spike correlates with a recent log entry noting a bearing replacement. Further analysis of the vibration signature is recommended to prevent future component failure. Consider scheduling a follow-up inspection in one month."


![OIP (2)](https://github.com/user-attachments/assets/7c7e63f3-9ea0-4057-b30a-92ad287eb492)

#### c) Few-Shot Prompting (Tabular Log of Activities)
- **Template:**  
> "Here are a few examples of how to format maintenance activities into a table. Follow this pattern for the provided data.  

Example 1: Date: 01-08-2025, Activity: Replaced motor, Technician: John →  
| Date | Activity | Technician |  
| 01-08-2025 | Replaced motor | John |  

Example 2: Date: 05-08-2025, Activity: Calibrated sensors, Technician: Sarah →  
| Date | Activity | Technician |  
| 05-08-2025 | Calibrated sensors | Sarah |  

New Data: Date: 15-08-2025, Activity: Replaced spindle, Technician: Mark"

- **Generated Report Snippet:**  
**Recent Maintenance Log**
| Date       | Activity          | Technician |
|------------|-----------------|------------|
| 15-08-2025 | Replaced spindle | Mark       |

![1-6](https://github.com/user-attachments/assets/8625954e-f244-4a5d-bef4-ca9a42761773)



## ✅ Conclusion
The experiment demonstrates that prompt templating is a powerful technique for automating complex report generation. Different prompt patterns allow:  

- Concise summaries (Single-Shot Prompting)  
- Context-aware, expert-level analysis (Role-Playing Prompting)  
- Structured and consistent tabular logs (Few-Shot Prompting)  

This approach ensures **consistency, reduces manual effort**, and improves efficiency in industrial maintenance reporting.

![download](https://github.com/user-attachments/assets/000e6811-2629-42af-9ed1-dc166056be02)




## 🔑 Role of Prompt Templating
- **Single-Shot Prompting:** Ideal for quick, high-level summaries and dashboards.  
- **Role-Playing Prompting:** Generates detailed, technical analyses with actionable recommendations.  
- **Few-Shot Prompting:** Structures data consistently into tables or lists without extensive coding.



## 📝 Result
The study successfully demonstrated automated maintenance report generation using prompt templating. Reports were **accurate, consistent, and context-specific**, confirming the effectiveness of this technique in industrial settings.
