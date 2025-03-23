# 📚 WebSchool

**WebSchool** is a comprehensive management solution designed for schools, offering streamlined inventory management, classroom organization, user administration, and task management—all in a responsive and intuitive interface built with **React**, **Next.js**, and **Firebase**.

---

## ✨ Features

### ✅ Implemented
- **Inventory Requests**: Efficiently request and track school inventory.
- **Inventory Management**: Manage and monitor school assets seamlessly.
- **Classroom Management**: Organize and allocate classroom resources effectively.
- **User Management**: Robust user administration and permissions.
- **Task Archiving and Deletion**: Easy archiving and deletion of tasks for optimized workflows.

### 🚧 Planned Features
- Tools management
- Application settings panel
- QR code functionality
- Electron desktop application

---

## 🛠️ Technology Stack

- **Frontend:** React, Next.js
- **Backend:** Firebase
- **Package Manager:** Yarn

---

## 🚀 Installation & Execution

Clone and install dependencies:

```bash
git clone https://github.com/gustavofalcao1/WebSchool.git
cd WebSchool
yarn install
```

Run development server:
```bash
yarn dev
```

Build for production:
```bash
yarn build
```

Run production build:
```bash
yarn start
```

---

## 📸 Screenshots

| Authentication Screen | Home Dashboard | Add Items |
|-----------------------|----------------|-----------|
| ![Auth](./screenshots/00.png) | ![Home](./screenshots/01.png) | ![Add](./screenshots/02.png) |

---

## 🚧 Deployment

### 🐧 Tested OS
- ✔️ Ubuntu Linux
- 🚧 Arch Linux (planned)
- 🚧 Windows (planned)
- 🚧 macOS (planned)

### 🔧 Deploy on Ubuntu

Clone this repository into `/opt` and create a systemd service:

```bash
sudo nano /etc/systemd/system/webschool.service
```

Paste the following content:

```ini
[Unit]
Description=WebSchool App Service
After=network.target

[Service]
ExecStart=/usr/bin/node /opt/webschool/pages/index.js
WorkingDirectory=/opt/webschool
Restart=always
User=root
Environment=NODE_ENV=production

[Install]
WantedBy=multi-user.target
```

Start and enable the service:
```bash
sudo systemctl start webschool
sudo systemctl enable webschool
```

Check service status:
```bash
sudo systemctl status webschool
```

---

## 🤝 Contributing

We encourage contributions to enhance WebSchool:

1. Fork the repository
2. Create your branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -m 'Add feature'`)
4. Push changes (`git push origin feature/new-feature`)
5. Submit a Pull Request

---

## 📄 License

Licensed under the **MIT License**.

---

## 👤 Author
**Gustavo Falcão**  
[GitHub @gustavofalcao1](https://github.com/gustavofalcao1)  
[Project Repository](https://github.com/gustavofalcao1/WebSchool)

---
