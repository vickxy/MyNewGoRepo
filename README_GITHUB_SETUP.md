# 🚀 Setting Up a New GitHub Repo and Pushing Go Code (with a Custom GitHub Account)

This guide helps you:
- Create a local Git repository
- Push it to GitHub
- Configure a custom GitHub account for just this project
- Write and push a Hello World in Go

---

## 1️⃣ Prerequisites

- [Git](https://git-scm.com/downloads) installed
- [Go](https://go.dev/dl/) installed
- A GitHub account

---

## 2️⃣ Create and Initialize the Project

```bash
mkdir MyNewGoRepo
cd MyNewGoRepo
git init
```

---

## 3️⃣ Configure Git for This Project Only

```bash
git config --local user.name "IAmVikesh"
git config --local user.email "yadav.vikesh27@gmail.com"
git config --list --local
```
*This only affects this repo, not your global Git config.*

---

## 4️⃣ Create the Go File

```bash
touch main.go
```

Paste this code:
```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

---

## 5️⃣ Run the Program

```bash
go run main.go
```

---

## 6️⃣ Create a Repo on GitHub

- Go to [GitHub](https://github.com)
- Click **New Repository**
- Name it (e.g., `MyNewGoRepo`)
- Choose public/private
- Click **Create Repository**

---

## 7️⃣ Connect Local Repo to GitHub

Copy your repo URL, then:

```bash
git remote add origin https://github.com/YOUR-USERNAME/hello-world-go.git
git branch -M main
git add .
git commit -m "Initial commit - Hello World in Go"
git push -u origin main
```

---

## 8️⃣ Verify

- Visit your GitHub repo page
- You should see your `main.go` file!

---