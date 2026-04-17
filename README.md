# Brute Force Detection using Windows Event Logs

## 📌 About this Project

In this project, I simulated a brute force login scenario on my local Windows machine and analyzed the generated logs using Event Viewer.

The goal was to understand how failed login attempts are recorded and how such patterns can indicate suspicious activity.

---

## 🛠️ What I Used

- Windows OS (Local Machine)
- Event Viewer

---

## 🔍 What I Did

- Entered incorrect passwords multiple times on the lock screen
- Opened Event Viewer and navigated to Security logs
- Filtered logs using Event ID 4625 (failed login attempts)
- Analyzed multiple log entries to identify patterns

---

## 📊 What I Observed

- Multiple failed login attempts were recorded within a short time frame
- All attempts showed **Logon Type 2**, indicating interactive login
- The failure reason was due to incorrect password
- Repeated login failures for the same system indicate suspicious behavior

---

## 🚨 What This Means

This pattern is consistent with a potential brute force attack, where multiple password attempts are made in a short period of time.

Even though this was a simulated scenario, it reflects how real-world attacks can be identified using log analysis.

---

## 📸 Screenshots

### Filtered Logs (Event ID 4625)
![Filtered Logs](screenshots/filtered_logs.png)

### Multiple Failed Login Attempts
![Multiple Failures](screenshots/multiple_failures.png)

### Event Details View
![Event Details](screenshots/event_details.png)

---

## 🧠 What I Learned

- How Windows logs failed login attempts using Event ID 4625
- How to identify suspicious patterns based on frequency and timing
- The importance of log analysis in detecting unauthorized access attempts

---

## 🎯 Next Step

I will continue building more SOC-focused projects, including network traffic analysis and SIEM-based monitoring.
