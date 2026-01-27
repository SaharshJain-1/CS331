# Software Requirements Specification (SRS)

**Project:** Intelligent Chatbot with Task Execution Automation  
**Module:** CS331 Software Engineering Lab

---

## 1. Functional Requirements (FR)
Functional requirements define the specific behaviors and functions the system must support.

### 1.1. User Authentication & Security
* **FR-1.01:** The system shall require users to authenticate using a unique email address and password before granting access to the main dashboard or assistant features.
* **FR-1.02:** The system shall provide a secure registration interface allowing new users to create an account by providing a valid email ID and a secure password.
* **FR-1.03:** The system shall maintain a local database or file system to securely store user credentials and profile settings.

### 1.2. User Interface (UI) & Interaction
* **FR-2.01:** The system shall provide a Graphical User Interface (GUI) featuring a chat log, a dynamic avatar display, and status indicators for system activity (e.g., "Listening," "Processing").
* **FR-2.02:** The system shall support multi-modal input, allowing users to interact via voice commands (using speech-to-text) or text input (via keyboard).
* **FR-2.03:** The system shall provide multi-modal output, responding to the user via synthesized speech (text-to-speech) and visual text displayed in the chat window.
* **FR-2.04:** The system shall allow users to customize the interface, including changing the assistant's voice (Male/Female), speech rate, and UI themes (Light/Dark mode).

### 1.3. Web Data Retrieval & Automation
* **FR-3.01:** The system shall be capable of scraping real-time data from the web to provide current weather conditions and news headlines upon user request.
* **FR-3.02:** The system shall integrate with third-party APIs or libraries to fetch and summarize information from Wikipedia.
* **FR-3.03:** The system shall automate web navigation tasks, specifically opening YouTube videos and visualizing locations on Google Maps based on voice commands.
* **FR-3.04:** The system shall provide an automated communication interface to send emails and WhatsApp messages by taking the recipient's details and message content via voice input.

### 1.4. System Control & Task Automation
* **FR-4.01:** The system shall have privileges to execute Operating System (OS) level commands, including capturing screenshots, adjusting system volume, and retrieving battery/system status.
* **FR-4.02:** The system shall be capable of launching local applications (e.g., Notepad, Calculator) and managing application windows (minimize, maximize, switch tabs).
* **FR-4.03:** The system shall include file management automation, allowing the user to create specific file types (HTML, Python, Java) through voice commands.

### 1.5. Utilities & Computational Features
* **FR-5.01:** The system shall perform mathematical computations, including basic arithmetic, trigonometric functions, and number system conversions (binary/hexadecimal).
* **FR-5.02:** The system shall provide auxiliary utilities including a language translator, a smart dictionary for definitions, and a programmable countdown timer.

---

## 2. Non-Functional Requirements (NFR)
Non-functional requirements define the system qualities such as performance, security, and usability.

* **NFR-01 (Security & Privacy):** User passwords shall be stored in a hashed format (not plain text) to ensure the security of user credentials.
* **NFR-02 (Performance):** The system shall process voice commands and generate a response within a reasonable latency period (typically under 2-3 seconds for local tasks) to ensure a fluid conversational experience.
* **NFR-03 (Reliability):** The system shall handle network errors gracefully; if the device is offline, it must alert the user rather than crashing when attempting web-based tasks.
* **NFR-04 (Usability):** The interface shall provide clear visual cues (e.g., changing icons or text labels) to indicate when the system is in "Listening" mode versus "Processing" mode.
* **NFR-05 (Extensibility):** The system architecture shall be modular, allowing for the addition of new skills (e.g., new automation scripts) without altering the core main loop.
