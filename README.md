# ⚙️ Ansible – Learning & Practical Series

A hands-on journey to learning Ansible, IT automation, configuration management, and infrastructure automation through practical examples, YAML playbooks, and real-world implementations.

## 📌 About This Repository

This repository documents my complete Ansible learning journey, starting from the fundamentals of automation to advanced configuration management and infrastructure provisioning.

Each topic is organized day-wise with detailed explanations, executable commands, YAML configurations, practical examples, and hands-on exercises.

### 🎯 Learning Objectives

- ⚙️ Understand Ansible fundamentals and architecture.
- 🖥️ Manage remote servers using SSH.
- 📋 Work with Inventory and Configuration Files.
- 📜 Create and execute YAML Playbooks.
- 🧩 Understand Ansible Modules and Plugins.
- 🔄 Automate server configuration and management.
- 📦 Work with Ansible Roles and Collections.
- 🔐 Manage credentials using Ansible Vault.
- ☁️ Automate AWS and Cloud Infrastructure.
- 🚀 Integrate Ansible with CI/CD pipelines.

---

## 📖 Introduction to Ansible

**Ansible** is an open-source IT automation tool used for configuration management, application deployment, infrastructure provisioning, and task automation.

It helps automate repetitive administrative tasks across multiple servers and systems using simple, human-readable YAML files called **Playbooks**.

Ansible follows an **Agentless Architecture**, meaning it generally does not require any additional Ansible agent installation on managed Linux servers. It typically communicates with remote Linux machines through SSH.

### 🖥️ Understanding Ansible Architecture

Ansible follows a Control Node and Managed Nodes architecture.

- **Control Node:** The machine where Ansible is installed and from which automation commands are executed.
- **Managed Nodes:** Remote servers or systems that Ansible manages.
- **Inventory:** Contains information about managed hosts and their groups.
- **Playbooks:** YAML files containing automation instructions.
- **Modules:** Perform specific tasks on managed nodes.
- **Plugins:** Extend Ansible's functionality.

### 🏗️ Basic Architecture

```text
             Control Node
          (Ansible Installed)
                  |
          Ansible Playbooks
               (YAML)
                  |
              Inventory
                  |
             SSH Connection
                  |
       +----------+----------+
       |          |          |
    Server 1   Server 2   Server 3
       |          |          |
    Managed    Managed    Managed
      Node       Node       Node
```

### 🔄 How Ansible Works

1. Install Ansible on the Control Node.
2. Configure remote servers in the Inventory file.
3. Establish SSH connectivity with Managed Nodes.
4. Create YAML Playbooks containing automation tasks.
5. Execute playbooks using the `ansible-playbook` command.
6. Ansible connects to the target servers and performs the required operations.

### ⚖️ Ansible vs Traditional Manual Configuration

| Manual Configuration | Ansible Automation |
|---|---|
| Repetitive manual tasks | Automated tasks |
| Configure servers individually | Manage multiple servers |
| Time-consuming operations | Faster execution |
| Manual configuration tracking | Version-controlled playbooks |
| Difficult to maintain consistency | Desired-state configuration |

### 🔑 Important Ansible Concepts

| Concept | Description |
|---|---|
| Agentless | No Ansible agent required on typical managed Linux nodes |
| SSH | Remote communication mechanism |
| Inventory | List and groups of managed hosts |
| Playbook | YAML-based automation instructions |
| Modules | Perform specific operations |
| Roles | Organize reusable automation content |
| Idempotency | Repeated execution maintains the desired state when supported by the task/module |

---

## 🛠️ Ansible Installation

Before starting the practical lessons, Ansible must be installed and configured on your Control Node.

### Ansible Installation Guide

📦 **Ansible Installation – Step-by-Step Commands**

[DevOps Tools Installation – Ansible.md](https://github.com/byteAlok/DevOps-Tools-Installation-Commands/blob/main/DevOps%20%26%20Infrastructure/Ansible.md)

This guide contains Ansible installation instructions, setup commands, and configuration steps.

---

## 📚 Learning Structure

All learning materials are organized day-wise.

Each day contains a Markdown file documenting the topics covered, commands executed, explanations, YAML configurations, and practical results.

### 📂 Repository Structure

```text
Ansible/
│
├── README.md
│
├── Day-01-Introduction-to-Ansible.md
│
├── Day-02-Ansible-Architecture.md
│
├── Day-03-Ansible-Installation.md
│
├── Day-04-SSH-Configuration/
│   ├── README.md
│   └── examples/
│
├── Day-05-Ansible-Inventory/
│   ├── README.md
│   └── inventory.ini
│
├── Day-06-Ad-Hoc-Commands.md
│
├── Day-07-Ansible-Playbooks/
│   ├── README.md
│   └── playbook.yml
│
└── ...
```

*Note: The above structure is an example. Actual files and folders will be added as new topics are covered.*

### 📝 Documentation Naming Convention

**For theoretical topics and command-based practicals:**

```text
Day-<n>-<Topic-Name>.md
```

Examples:

```text
Day-01-Introduction-to-Ansible.md
Day-02-Ansible-Architecture.md
Day-03-Ansible-Installation.md
Day-06-Ad-Hoc-Commands.md
```

**For practical topics requiring additional files:**

```text
Day-<n>-<Topic-Name>/
│
├── README.md
├── inventory.ini
├── playbook.yml
└── additional-files/
```

Example:

```text
Day-07-Ansible-Playbooks/
│
├── README.md
├── inventory.ini
└── playbook.yml
```

### 📄 Daily Documentation Includes

- 📖 Topic Introduction
- 🧠 Conceptual Explanation
- 💻 Commands and Syntax
- 📜 YAML Configuration Examples
- 🔍 Command Execution Results
- 🧪 Hands-on Practicals
- 📌 Important Notes and Learnings

---

## 🚀 Learning Approach

This repository follows a practical, step-by-step learning approach.

1. Understand the concept.
2. Learn the required commands and YAML syntax.
3. Configure the Control Node and Managed Nodes.
4. Execute automation tasks and playbooks.
5. Observe and analyze the results.
6. Document the learning and implementation.

The goal is not just to understand Ansible theoretically, but to gain practical experience in server management, infrastructure automation, and real-world DevOps workflows.

---

## 🔗 Useful Resources

- 📘 [Ansible Official Documentation](https://docs.ansible.com/)
- 🚀 [Getting Started with Ansible](https://docs.ansible.com/projects/ansible/latest/getting_started/index.html)
- 📜 [Ansible Playbooks Guide](https://docs.ansible.com/projects/ansible/latest/playbook_guide/index.html)
- 🧩 [Ansible Roles](https://docs.ansible.com/projects/ansible/latest/playbook_guide/playbooks_reuse_roles.html)
- 🛠️ [Ansible Installation Guide](https://github.com/byteAlok/DevOps-Tools-Installation-Commands/blob/main/DevOps%20%26%20Infrastructure/Ansible.md)

---

## 👨‍💻 Author

**Alok Maurya**

- 🐙 GitHub: [@byteAlok](https://github.com/byteAlok)
- 🌐 Portfolio: [aloksde.com](https://aloksde.com)

💡 Learning | Building | Automating | Growing

---

⭐ If you find this repository helpful, consider giving it a star!
