
# 🚀 Mi-Stack: The Sri Lanka's First Automated Unified Hosting Platform

Mi-Stack is a developer-focused, one-click deployment platform that radically simplifies hosting for full-stack, frontend, and backend applications. Built to compete with major cloud providers, Mi-Stack abstracts infrastructure management and empowers you to deploy apps with just a ZIP file or GitHub URL.

**⚠️ Mobile access is currently unsupported.**
Use Mi-Stack from a desktop or laptop for full functionality!!!

---

## 🌟 Key Features

* 🖥️ Code to Cloud in one click — No VPS, no setup, no DevOps needed
* ⚙️ Automatic build and deployment pipeline for supported languages
* 📦 Upload `.zip` files or paste GitHub repository URLs
* 💡 Supports popular stacks: Node.js, Python (Flask/Django), Go, PHP, Ruby (Sinatra), Java (Spring Boot), and static websites
* ☸️ Built on Kubernetes-based isolated environments
* 👤 Dynamic experience based on login status

---

## 📂 Supported App Structures

**All apps must listen on PORT 8080** (except Static and PHP apps, which are served on PORT 80).

---

### 📦 Node.js

**Required Structure:**

project.zip
├── server.js
├── package.json
└── public/
  ├── index.html
  ├── style.css
  └── script.js

* Must include `package.json` with `"start": "node server.js"`
* `node_modules` will be automatically installed

---

### 🐍 Python (Flask / Django)

**Flask Example:**

project.zip
├── app.py
├── requirements.txt
└── static/
  ├── index.html
  ├── style.css
  └── script.js

**Django Tips:**

* Include the Django project folder, `manage.py`, and `requirements.txt`
* Run `python manage.py collectstatic` before zipping
* Do **not** include `venv/` or `db.sqlite3` unless needed

---

### 🌐 Static Websites (HTML / CSS / JS)

**Required Structure:**

project.zip
├── index.html
├── styles.css
├── script.js
└── assets/
  ├── images/
  ├── fonts/
  └── other/

* `index.html` must be at the root
* Include all CSS, JS, and assets your site needs
* Do not include `node_modules` or source folders
* For React/Vue/Next.js, run the build and upload the contents of the `build` or `dist` folder
* Hosted using NGINX on port 80

---

### 🐘 PHP

**Required Structure:**

project.zip
├── index.php
├── config.php
├── includes/
├── public/
└── vendor/ ❌ (do not include this)

* `index.php` must be at the root
* Organize includes inside `includes/`
* Use `public/` for JS, CSS, and images
* Do not include `vendor/`, editor config files, or caches
* Served by Apache on port 80

---

### ☕ Java (Spring Boot / Micronaut / Quarkus)

**Required Structure:**

project.zip
├── app.jar
├── config/
├── logs/
└── README.md

* Use `mvn clean package` or `./gradlew bootJar` to build a runnable fat JAR
* Only upload the JAR — no source code or `.class` files
* Ensure `Main-Class` is set in `MANIFEST.MF`
* App must listen on port 8080
* Test locally using `java -jar app.jar`

---

### 🐹 Go

**Required Structure:**

project.zip
├── main.go
├── go.mod
├── go.sum
├── handlers.go
└── assets/
  ├── css/
  ├── js/
  └── images/

* `main.go` must include `func main()`
* Use Go modules (`go.mod`, `go.sum`)
* Exclude build artifacts, IDE folders, and vendor/
* Hosted on port 8080 after automatic build

---

### 💎 Ruby (Sinatra)

**Required Structure:**

project.zip
├── app.rb
├── Gemfile
├── public/
└── views/

* Use Sinatra or a compatible minimal framework
* Do not include `vendor/` or IDE/editor configuration files

---

## 💡 How Mi-Stack Works

1. **Choose App Type:** Select from supported frameworks using toggle buttons (checkbox UI)
2. **Upload App:** Provide a `.zip` file or paste your GitHub repo URL
3. **Automated Process:** Mi-Stack builds, installs, and deploys your app inside a Docker container
4. **Instant Launch:** Your app is served live and logs are available

---

## 🧑‍🚀 About Mi-Stack

Mi-Stack was created by **Missari** to radically simplify app hosting — especially for frontend, backend, and DevOps users.

Instead of managing complex cloud servers, Mi-Stack offers a streamlined, one-click deployment experience that abstracts away infrastructure.

Our platform builds, packages, and runs your apps inside automatically — so you can focus on **coding**, not **server operations**.

Mi-Stack aims to compete with providers like AWS by delivering fast, affordable, and easy hosting for everyone.

🔗 [Visit our LinkedIn](https://www.linkedin.com/company/mi-stack/)

---

## 📢 Tagline (Dynamic)

* **If logged in:** No VPS, No server setup, just pure code-to-cloud simplicity.
* **If visitor:** Deploy Your Backend & Frontend Apps in One-Click

---

## 🛑 Mobile Access Not Supported

Mi-Stack is designed for desktops and laptops only. Its advanced developer features and UI require a larger screen for optimal functionality.

---

## 📬 Need Help?

If you have any questions or need support, connect with us on [LinkedIn](https://www.linkedin.com/company/mi-stack/).

We’re here to help you deploy faster 🚀

---

