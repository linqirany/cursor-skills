# Cursor Skills

A collection of Cursor Skills for Rockchip Linux, RTOS, Android and embedded development.

> A growing collection of practical Cursor Skills focused on Rockchip platform development and embedded Linux debugging.

---

# Overview

This repository contains a set of reusable Cursor Skills that I use during daily embedded Linux development.

The goal is to accumulate debugging experience into reusable workflows, allowing Cursor to better understand Rockchip SDKs, Linux drivers, RT-Thread, AMP architecture and project handoff documentation.

---

# Current Skills

| Skill | Description |
| ------- | ----------- |
| rk-debug | General debugging assistant for Rockchip Linux / Android / RTOS |
| rk-handoff | Automatically generate project handoff documentation |

---

# Repository Structure

```text
cursor-skills
├── README.md
├── LICENSE
└── skills
    ├── rk-debug
    └── rk-handoff
```

---

# Features

Current focus includes:

- Rockchip SDK analysis
- Linux Driver debugging
- DTS & DeviceTree analysis
- UART / RS485 debugging
- CAN debugging
- I2C / SPI debugging
- GPIO debugging
- AMP (Linux + RT-Thread)
- Boot log analysis
- Project handoff generation

---

# Installation

Clone this repository:

```bash
git clone https://github.com/linqirany/cursor-skills.git
```

Copy the desired Skill into your Cursor Skills directory.

Example:

```text
~/.cursor/skills/
```

or

```text
%USERPROFILE%\.cursor\skills\
```

Restart Cursor after copying.

---

# Roadmap

- [x] rk-debug
- [x] rk-handoff
- [ ] rk-sdk
- [ ] dts-debug
- [ ] amp-debug
- [ ] rs485-debug
- [ ] can-debug
- [ ] linux-driver-debug
- [ ] git-workflow

---

# Philosophy

Rather than writing isolated prompts, this repository aims to build reusable engineering workflows.

Each Skill should:

- Solve a real engineering problem
- Be reusable across multiple projects
- Follow practical debugging methodology
- Continuously evolve with development experience

---

# License

MIT License.
