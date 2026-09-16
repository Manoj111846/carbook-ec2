# 🚗 CARBOOK - Car Rental Website

A modern and responsive **Car Rental Website** built with HTML, CSS, JavaScript, SCSS, and Bootstrap.  
The website is deployed on **AWS EC2 (Ubuntu)** using **Nginx** and the source code is maintained with **Git/GitHub**.

## 🌐 Live Website

**http://65.2.152.21**

> The live URL uses the EC2 public IP, so it may change if the EC2 instance is stopped and started without an Elastic IP.

---

## ✨ Features

- 🏠 Home page with car-rental booking section
- 🚘 Featured vehicles section
- 📋 Car listing and car details pages
- 🛠️ Services section
- 💰 Pricing section
- 📝 Blog and blog-single pages
- 📞 Contact page
- 📱 Responsive layout
- 🎨 Modern UI using CSS/SCSS and Bootstrap
- ☁️ Deployment on AWS EC2 with Nginx
- 🔧 Version control using Git and GitHub

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Website structure |
| CSS3 | Styling and layout |
| JavaScript | Client-side interactions |
| SCSS | Advanced CSS organization |
| Bootstrap | Responsive UI components |
| AWS EC2 | Cloud hosting |
| Ubuntu | Server operating system |
| Nginx | Web server |
| MobaXterm | SSH/SFTP and server management |
| Git | Version control |
| GitHub | Source-code hosting |

---

# 📸 Project Screenshots

## 1. 🏠 Home Page

![CARBOOK Home Page](./screenshots/home.png)

## 2. 🛠️ Services Section

![CARBOOK Services](./screenshots/services.png)

## 3. 📊 Statistics & Footer

![CARBOOK Statistics and Footer](./screenshots/stats-footer.png)

## 4. 🚘 Featured Vehicles

![CARBOOK Featured Vehicles](./screenshots/vehicles.png)

---

# ☁️ AWS EC2 Deployment

The website is hosted on an **Ubuntu EC2 instance** using Nginx.

### Deployment Architecture

```text
                    Internet
                       │
                       ▼
              EC2 Public IP
              65.2.152.21
                       │
                       ▼
                  AWS EC2
                   Ubuntu
                       │
                       ▼
                    Nginx
                       │
                       ▼
               /var/www/html
                       │
                       ▼
              CARBOOK Website
```

### Website Directory

```text
/var/www/html
```

Nginx serves the static website files from this directory.

---

# 📂 Project Structure

```text
carbook-ec2/
│
├── index.html
├── about.html
├── services.html
├── pricing.html
├── car.html
├── car-single.html
├── blog.html
├── blog-single.html
├── contact.html
├── main.html
│
├── css/
├── js/
├── images/
├── fonts/
├── scss/
│
├── .gitignore
├── prepros-6.config
├── readme.txt
└── README.md
```

---

# 🚀 Run Locally

Clone the repository:

```bash
git clone https://github.com/Manoj111846/carbook-ec2.git
```

Move into the project:

```bash
cd carbook-ec2
```

Then open:

```text
index.html
```

in a browser.

You can also serve it locally with Python:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

---

# 🔄 Git Workflow Used

The project was initialized and pushed from the EC2 instance using Git:

```bash
cd /var/www/html

git init

git add .

git commit -m "Initial commit - CARBOOK website"

git branch -M main

git remote add origin https://github.com/Manoj111846/carbook-ec2.git

git push -u origin main
```

---

# 🔧 AWS Deployment Steps

The basic deployment process was:

```text
1. Create EC2 Ubuntu instance
        ↓
2. Connect using MobaXterm
        ↓
3. Install Nginx
        ↓
4. Allow HTTP port 80 in Security Group
        ↓
5. Upload website files
        ↓
6. Store files in /var/www/html
        ↓
7. Start/enable Nginx
        ↓
8. Open EC2 Public IP in browser
        ↓
9. Initialize Git
        ↓
10. Push project to GitHub
```

---

# 🔐 Security Notes

- The EC2 security group allows HTTP traffic on port **80** for the public website.
- SSH access should preferably be restricted to a trusted IP rather than opened to everyone.
- Never upload `.pem` private keys, passwords, API keys, or other secrets to GitHub.
- `.gitignore` is included to prevent common unwanted files from being committed.

---

# 👨‍💻 Author

**Manoj**

GitHub:  
https://github.com/Manoj111846

Repository:  
https://github.com/Manoj111846/carbook-ec2

---

## 📄 License

This project is created for educational and project demonstration purposes.
