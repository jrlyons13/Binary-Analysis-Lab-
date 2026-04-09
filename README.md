# 🔍 Binary Analysis Lab – Extracting Intelligence from Binaries

## 🎯 Overview

In real-world cybersecurity, analysts often encounter **unknown or suspicious binaries** with no source code.

This lab demonstrates how to quickly extract meaningful intelligence using basic Linux tools.

---

## 💡 Problem Scenario

A suspicious executable is discovered on a system.

You need to answer:
- What does this program do?
- Does it contain sensitive or malicious data?
- Can we extract clues without running it?

---

## 🧠 Skills Demonstrated

- Static analysis of binaries
- Data extraction using `strings`
- Targeted filtering with `grep`
- Identifying hardcoded secrets
- Analytical thinking (SOC / IR mindset)

---

## 🛠️ Tools Used

- GNU Binutils (`strings`)
- grep
- Linux CLI

---

## 🧪 Lab Workflow

```bash
chmod +x instructor_hatch_probe
file instructor_hatch_probe

strings instructor_hatch_probe | less

strings instructor_hatch_probe | grep -Ei 'hatch|code|access|unlock'

./instructor_hatch_probe
