# AWS Login System for Unreal Engine 5

This project provides a robust, ready-to-use authentication system integrated with **AWS Cognito** for Unreal Engine 5. It handles user registration, verification, sign-in, and password management using an API Gateway backend.

## 🚀 Features

- **User Registration**: Sign up with email and password.
- **Account Verification**: Email verification via confirmation codes.
- **Secure Login**: Authentication against AWS Cognito User Pools.
- **Password Recovery**: Support for forgot/reset password flows.
- **Modern UI**: Clean, customizable Unreal Engine UMG widgets for all auth screens.
- **Blueprint Integration**: Fully accessible and customizable via Blueprints.

## 📂 Project Structure

- **`/Content/LoginLevel.umap`**: The entry point level containing the login UI setup.
- **`/Content/LoginMenu.uasset`**: The main UMG Widget that orchestrates the auth flow.
- **`/Content/SigninTemplate.uasset`**: Sub-widget for the sign-in screen.
- **`/Content/SignUpTemplate.uasset`**: Sub-widget for the registration screen.
- **`/Content/ConfirmationTemplate.uasset`**: Sub-widget for email code verification.

## 🛠 Prerequisites

- **Unreal Engine 5.1+**
- **AWS Account** with Cognito User Pool and API Gateway configured.
- **Epic Games HTTP Request Plugin** (or equivalent) for handling API calls.

## ⚙️ Configuration

To connect this system to your AWS backend:

1.  Open the project in Unreal Engine.
2.  Navigate to the Blueprints handling the API requests (usually within `LoginMenu` or a dedicated API Service Blueprint).
3.  Update the **API Gateway Endpoint URL** to point to your deployed AWS infrastructure.
4.  Ensure your Cognito Client ID and Pool ID are correctly referenced if calling Cognito directly.

## 📖 How to Use

1.  **Launch**: Set `LoginLevel` as your startup map in Project Settings.
2.  **Logic**: The system communicates with AWS via REST API calls. On success, it returns tokens which can be stored in a `GameInstance` or `SaveGame` for session management.
3.  **Customization**: All UI elements are standard UMG widgets. You can easily modify the design in the `Content` folder.

## 📝 License

This project is part of the Metaverse repository.

---
*Created by Aptronics.*
