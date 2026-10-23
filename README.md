# IKEA BILRESA – All-in-One Blueprint (Buttons + Scrollwheel)

This blueprint enables full use of the **IKEA BILRESA scroll wheel remote**
in **Home Assistant** via **Matter / event.* entities**.

It combines **all features in a single blueprint**:
- 3 buttons (Button 2 & 3 optional)
- Scrollwheel right / left **per button**
- Multi-clicks
- Hold to dim
- No cover functions (intentionally left out)

---

## ✨ Features

### Buttons (Button 1–3)
- **1× click** (`multi_press_1`)
- **2× click** (`multi_press_2`)
- **3× click** (`multi_press_3`)
- **Hold / Release**
  - `long_press` → dim
  - `long_release` → stop

Buttons **2 and 3 are optional**.  
If no event entity is selected, they are simply ignored.

---

### Scrollwheel
Configurable **separately for each button**:

- Right rotation → increase or decrease brightness
- Left rotation → increase or decrease brightness
- Takes `totalNumberOfPressesCounted` into account
- Separate step size per direction
- Separate target light per button possible

The Button 2 & 3 scrollwheel entities are also **optional**.

---

## 🧩 Requirements

- **Home Assistant Core ≥ 2024.x**
- IKEA **BILRESA scroll wheel remote**
- Integration that creates **`event.*` entities** (e.g. Matter)
- Dimmable light (`light` domain)

⚠️ This blueprint is **not** intended for ZHA/Zigbee action sensors,  
but explicitly for **event-based Matter entities**.

---

## 📥 Installation

### Direct import (recommended)
Click this link:

https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/sharkovich/ikea-bilresa-blueprint/main/blueprints/automation/ikea_bilresa_all_in_one.yaml

---

## 🙏 Credits

The original blueprint was created by [tomv79](https://github.com/tomv79) –
see [tomv79/ikea-bilresa-blueprint](https://github.com/tomv79/ikea-bilresa-blueprint).  
This repository is an English translation of it.
