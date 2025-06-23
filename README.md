Here’s a professional `README.md` tailored for your **GitHub Pages-based APT repository** for `gocrafter`, assuming you're hosting your `.deb` packages under a URL like:

```
https://ErebusAJ.github.io/aptrepo
```

---

## 🧾 `README.md` for GitHub APT Repo

````markdown
# 🐧 Gocrafter APT Repository

Welcome to the official APT repository for **Gocrafter** — a CLI tool to scaffold and bootstrap Go projects quickly and efficiently.

This repo allows you to install `gocrafter` via `apt` on any Debian-based Linux system (Ubuntu, PopOS, Mint, etc).

---

## 📦 What is Gocrafter?

> Gocrafter is a CLI tool to initialize new Go projects with optional components like:
> - `go mod` and project structure
> - `sqlc`, `goose` for SQL tooling
> - Dockerfile and Magefile generation
> - YAML-based configuration support
> - Clean, interactive progress feedback

🔗 [Project Repo →](https://github.com/ErebusAJ/gocrafter)

---

## 📥 How to Install via APT

### 1. Add the GPG Public Key

```bash
curl -fsSL https://ErebusAJ.github.io/aptrepo/gocrafter-pubkey.gpg | \
sudo gpg --dearmor -o /usr/share/keyrings/gocrafter-archive-keyring.gpg
````

### 2. Add the APT Source

```bash
echo "deb [signed-by=/usr/share/keyrings/gocrafter-archive-keyring.gpg] https://ErebusAJ.github.io/aptrepo stable main" | \
sudo tee /etc/apt/sources.list.d/gocrafter.list
```

### 3. Update & Install

```bash
sudo apt update
sudo apt install gocrafter
```

---

## ✅ Verify Installation

```bash
gocrafter --help
```

---

## 💡 Want to Contribute?

Contributions are welcome! Please check the [`CONTRIBUTING.md`](https://github.com/ErebusAJ/gocrafter/blob/main/CONTRIBUTING.md) in the main repo.

---

## 🛡 License

This repository is licensed under the **GPL-3.0** license.

---

## 🔗 Links

* 📦 [Main Project Repo](https://github.com/ErebusAJ/gocrafter)
* 🧰 [Gocrafter Docs](https://github.com/ErebusAJ/gocrafter#readme)
* 🔐 [Public GPG Key](https://ErebusAJ.github.io/aptrepo/gocrafter-pubkey.gpg)

