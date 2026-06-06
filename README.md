# 📦 Microsoft Office Deployment Tool (ODT) Guide

## 🔗 Required Downloads & Links

### 📖 Official Documentation

https://learn.microsoft.com/en-us/microsoft-365-apps/deploy/overview-office-deployment-tool

### ⬇️ Download Office Deployment Tool

https://www.microsoft.com/en-us/download/details.aspx?id=49117

### ⚙️ Office Configuration Generator

https://config.office.com/deploymentsettings

---

## 🚀 Installation Steps

### 1️⃣ Download and extract Office Deployment Tool

Download ODT from Microsoft and extract it to:

```cmd
C:\Office 365
```

### 2️⃣ Create Configuration File

Use the Office Customization Tool to generate and save:

```text
configuration.xml
```

inside:

```text
C:\Office 365
```

### 3️⃣ Open Command Prompt

Run Command Prompt as Administrator.

### 4️⃣ Go to ODT Folder

```cmd
cd C:\Office 365
```

### 5️⃣ Install / Configure Office

```cmd
setup.exe /configure configuration.xml
```

⏳ Wait for Office installation to complete.

---

## 🛠️ Useful Commands

### 📥 Download Office Files Only

```cmd
setup.exe /download configuration.xml
```

### 📦 Install Office from Downloaded Files

```cmd
setup.exe /configure configuration.xml
```

### ❌ Remove Office

```cmd
setup.exe /configure remove.xml
```

---

## 📌 Notes

* ✅ Use Administrator Command Prompt.
* ✅ Keep `setup.exe` and `configuration.xml` in the same folder.
* ✅ Internet connection is required for downloading Office files.
* ✅ LTSC, Microsoft 365 Apps, and Visio/Project can all be deployed using ODT.
