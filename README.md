# 🌐 Metaverse: Premium Simulator Game (Login System)

Welcome to the core authentication module of **Metaverse**, a state-of-the-art simulator game designed for immersive learning and professional training. 

This repository houses the **AWS-powered Login System**, which serves as the primary authentication gateway to the entire Metaverse ecosystem.

---

## 🔗 Project Ecosystem & Integration

The **Metaverse** is part of a larger, high-performance educational infrastructure designed for real-time synchronization and tracking:

*   **Simulator Game (Metaverse)**: [https://github.com/aptronics-master/metaverse.git](https://github.com/aptronics-master/metaverse.git)
*   **Learning Management System (Nexus LMS)**: [https://github.com/aptronics-master/nexus.git](https://github.com/aptronics-master/nexus.git)

### 🔄 Nexus LMS & SCORM Synchronization
The Metaverse simulator is fully integrated with **Nexus LMS** for seamless educational tracking and reporting:

*   **SCORM Compliance**: The system leverages **SCORM** (Sharable Content Object Reference Model) standards, or **SCORMing**, to ensure high-fidelity communication between the simulator and the LMS.
*   **Real-time Score Sync**: Every score and performance metric obtained by the user within the **Metaverse** simulator is automatically synchronized and displayed within the **Nexus LMS**.
*   **Performance Monitoring**: Instructors can monitor student progress and performance in real-time, directly from the Nexus dashboard.

---

## 🚀 Login System Features

As the foundational module for the Metaverse, the **AWS Login System** provides:

-   ✨ **Seamless Registration**: High-performance signup flow with email and password.
-   🔒 **Secure Verification**: Robust email verification via AWS Cognito confirmation codes.
-   🏎️ **High-Security Login**: State-of-the-art authentication against AWS Cognito User Pools.
-   🛠️ **Password Management**: Integrated forgot/reset password workflows for maximum user reliability.
-   🎨 **Premium UI**: Sleek, modern Unreal Engine UMG widgets designed for a premium "Metaverse" aesthetic.
-   🔌 **Blueprint-First Architecture**: Fully customizable logic for Unreal Engine developers, optimized for simulator integration.

---

## 📂 Project Structure (Login Module)

-   **`/Content/LoginLevel.umap`**: The entry point level containing the login UI setup.
-   **`/Content/LoginMenu.uasset`**: The main UMG Widget orchestrating the auth flow.
-   **`/Content/SigninTemplate.uasset`**: Sub-widget for the sign-in screen.
-   **`/Content/SignUpTemplate.uasset`**: Sub-widget for the registration screen.
-   **`/Content/ConfirmationTemplate.uasset`**: Sub-widget for email code verification.

---

## 🛠 Prerequisites

- **Unreal Engine 5.6+**
- **AWS Account** with Cognito User Pool and API Gateway configured.
- **Required Plugins**:
    - **HttpBlueprint** (Epic Games HTTP Request Plugin)
    - **VaRest** (JSON and REST API handling)
    - **MasterHttpRequest**
    - **VaRestX**

---

## ⚙️ Configuration

To connect this system to your AWS backend:

1.  **Open Project**: Launch the project in Unreal Engine.
2.  **API Setup**: Navigate to the Blueprints handling API requests.
3.  **Endpoint Configuration**: Update the **API Gateway Endpoint URL** to point to your deployed AWS infrastructure.
4.  **Credential Management**: Ensure your Cognito Client ID and Pool ID are correctly referenced.

---

## 📖 How to Use

1.  **Launch**: Set `LoginLevel` as your startup map in Project Settings.
2.  **Logic**: The system communicates with AWS via REST API calls. On success, it returns tokens which can be stored in a `GameInstance` or `SaveGame` for session management and LMS sync.
3.  **Customization**: All UI elements are standard UMG widgets. Design can be modified in the `Content` folder.

---

## 📝 License & Attribution

This project is a critical component of the [Metaverse Simulator](https://github.com/aptronics-master/metaverse.git).

---
*Developed by Aptronics.*
