# Oracle APEX Schools Application

## Overview
The **Oracle APEX Schools Application** is designed as a part of MLH Dataweek Hackathon to help manage school-related data, including students, teachers, classes, and schedules. It is built using Oracle APEX and requires minimal setup to get started. This application also includes push notification capabilities and other shared components.

---

## Features
- Manage student and teacher records.
- Class scheduling and organization.
- Integrated navigation menus.
- Push notifications support (requires configuration).
- A responsive, easy-to-use interface.

---

## Installation Instructions

### Prerequisites
- **Oracle APEX Version**: 24.1.5 or higher.
- **Database**: Oracle Database 12c or higher.
- APEX workspace with the required parsing schema.

### Steps to Install
1. **Clone or Download the Repository**:
   - Clone the repository:
     ```bash
     git clone https://github.com/Mariaasla/oracle-apex-schools.git
     ```
   - Or download the repository as a ZIP file.

2. **Log in to Oracle APEX**:
   - Open your Oracle APEX workspace.

3. **Import the Application**:
   - Navigate to **Application Builder > Import/Export > Import**.
   - Upload the `NYCSchools.zip` file from this repository.
   - Follow the prompts:
     - Use **Reuse Application ID** unless there's a conflict.
     - Assign the parsing schema to the one in your workspace (e.g., `WKSP_MARIAAPPS`).

4. **Configure Push Notification Credentials**:
   - After importing, navigate to **Shared Components > Web Credentials**.
   - Locate `App 270978 Push Notifications Credentials`.
   - Enter your own Key Pair credentials.

5. **Set Up Database Objects** (if required):
   - If additional `.sql` scripts are needed for database objects, run them in your schema.

6. **Run the Application**:
   - After setup, click **Run Application** to test and use the application.

---

## Post-Installation Steps
1. **Replace Placeholder Credentials**:
   - Update any placeholder values for credentials or other required settings.
   - Documentation for placeholder replacement is in the comments of the `install.sql` file.

2. **Test Functionality**:
   - Ensure all pages, menus, and notifications work as expected.
   - Verify that the push notifications are functioning after configuring the credentials.

---


---

## Known Issues
- Ensure the Oracle APEX version matches the exported version to avoid compatibility issues.
- Push notifications will not work until credentials are configured.

---

