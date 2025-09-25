# Welcome to SlashOS's Pacman Repository

![Logo](https://skyline.be/skylicons/duotone/Package_Duo_Light.png)

## 📦 Overview

Welcome to the SlashOS Pacman repository! This repository provides access to a collection of software packages for Arch-based distributions, such as SlashOS. 

## 🚀 Getting Started

To add our repository to your Pacman sources and install packages, follow these steps:

### 1. Add the Repository and install the Key

Open a terminal and run the following commands:

```bash
grep -q "\[slashos\]" /etc/pacman.conf && echo "Repository already exists" || (echo -e "\n[slashos]\nSigLevel = Optional TrustedOnly\nServer = https://slashos.github.io/pacman-repo/\$arch" | sudo tee -a /etc/pacman.conf > /dev/null && echo "Repository added successfully")
```

### 2. Update Package Index

Update your package index to include packages from the new repository:

```bash
sudo pacman -Sy
```

### 3. Install Packages

Install any available package from our repository:

```bash
sudo pacman -S your-package
```

## 💬 Support

If you encounter any issues or have questions, please reach out to us:

- **Email:** [mauro.druwel@gmail.com](mailto:mauro.druwel@gmail.com)
- **Issues Tracker:** [GitHub Issues](https://github.com/SlashOS/pacman-repo/issues)
- **Community Forum:** [Forum Link](https://slashos.github.io)

Thank you for using SlashOS's Pacman Repository!


---
