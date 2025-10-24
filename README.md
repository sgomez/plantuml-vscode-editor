# 🪴 PlantUML Dev Container

A ready-to-use **Visual Studio Code Dev Container** for creating and previewing [PlantUML](https://plantuml.com/) diagrams using the [jebbs.plantuml](https://marketplace.visualstudio.com/items?itemName=jebbs.plantuml) extension and a local PlantUML server.

---

## Features

- Preconfigured **PlantUML server** running inside Docker (`plantuml/plantuml-server:jetty`)
- Integrated with VS Code PlantUML extension (`jebbs.plantuml`)
- Organized directory structure for source and exported diagrams
- Runs entirely in an isolated **Dev Container** environment

---

## Requirements

Before you start, make sure you have:

- [Visual Studio Code](https://code.visualstudio.com/)
- [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
- [Docker Desktop](https://www.docker.com/products/docker-desktop/) (or any Docker engine)

---

## Folder Structure

```
├── .devcontainer/
│   └── devcontainer.json   ← Dev Container configuration
├── diagrams/
│   ├── src/                ← Source .puml files
│   └── out/                ← Exported diagrams (PNG, SVG, etc.)
└── README.md
```

---

## How to Use

### 1. Open the project in VS Code

Clone or open this repository folder in **Visual Studio Code**.

### 2. Reopen in Dev Container

When prompted by VS Code, click:

> **“Reopen in Container”**

This will:
- Build and start the container defined in `.devcontainer/devcontainer.json`
- Automatically run a local PlantUML server on **port 9099**
- Install `jebbs.plantuml` extension.

## Creating and Viewing Diagrams

1.	Add your `.puml` files inside diagrams/src/
2.	Open the file in VS Code.
3.	Use one of the following:
    1. Right-click → “Preview Current Diagram”
    1. Press Alt + D (Windows/Linux) or Option + D (macOS)
    1. Or use Command Palette → “PlantUML: Preview Current Diagram”
4.	The rendered diagram will be shown in a preview panel or exported to diagrams/out/.

## License

This setup is provided for development purposes and can be freely adapted to your projects.
