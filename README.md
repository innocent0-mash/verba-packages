# 🚀 Verba Packages

The official package repository for the **Verba programming language**.

Verba Packages provides a collection of lightweight, reusable modules designed to extend the functionality of Verba and simplify development through a clean and modular ecosystem.

---

## ✨ Features

* 📦 **Centralized Package Repository**
* ⚡ **Lightweight & Fast Modules**
* 🔗 **Alias-Based Installation System**
* 🧩 **Modular Architecture**
* 🌍 **GitHub-Based Distribution**
* 🔄 **Registry-Driven Package Management**

---

## 📁 Project Structure

```
/verba-packages
 ├── packages/
 │   ├── <package-name>/
 │   │   ├── index.vrb
 │   │   └── meta.json
 │
 ├── registry/
 │   └── index.json
 │
 ├── docs/
 └── README.md
```

---

## ⚙️ How It Works

1. Each package is stored in its own folder
2. Metadata is defined in a `meta.json` file
3. All packages are registered in a central `index.json`
4. Users install packages using **alias names**

---

## 📦 Installation (Concept)

```bash
verba install <alias-name>
```

Example:

```bash
verba install data
```

---

## 🧠 Package Format

Each package should follow this structure:

```
<package-name>/
 ├── index.vrb
 ├── meta.json
```

### Example `meta.json`

```json
{
  "name": "data",
  "version": "1.0.0",
  "alias": "data",
  "description": "Basic data utilities for Verba"
}
```

---

## 🌐 Registry System

The registry connects alias names to actual package sources.

Example `registry/index.json`:

```json
{
  "data": {
    "repo": "https://github.com/verba/packages/data",
    "version": "1.0.0"
  }
}
```

---

## 🚀 Goals

* Create a scalable package ecosystem
* Enable simple and fast package installation
* Keep modules lightweight and efficient
* Support community-driven development

---

## 🤝 Contributing

We welcome contributions from developers!

### Steps:

1. Fork the repository
2. Create your package inside `/packages`
3. Add metadata and documentation
4. Register it in `registry/index.json`
5. Submit a pull request

---

## 📜 License

MIT License

---

## 💡 Vision

Verba Packages aims to become a powerful ecosystem where developers can easily discover, install, and build with modular components—making Verba fast, scalable, and developer-friendly.
