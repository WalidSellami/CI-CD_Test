# Flutter CI/CD with Firebase App Distribution & Hosted Download Page

This repository uses **GitHub Actions** to automate the **build and release process** for the Flutter app ensuring fast, consistent, and reliable delivery.

## ⚙️ Workflow Overview

On every **push** to the `master` branch, the workflow performs the following steps:

1. **Setup Environment**
    - The workflow installs Flutter and project dependencies.

2. **Build APK**
    - Builds a release APK.

3. **Version & Rename**
    - Automatically renames the APK with the current Git tag or commit version.

4. **Firebase App Distribution**
    - Uploads the built APK to **Firebase App Distribution**
    - Notifies testers via Firebase

5. **Hosted Download Page**
    - Publishes a simple HTML download page
    - Provides direct download links for testers or stakeholders via mail.