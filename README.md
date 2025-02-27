
# Two-Way Switch Synchronization Blueprint

## 📖 Overview

The **Two-Way Switch Synchronization** blueprint for Home Assistant allows you to synchronize two switches so they always operate in unison. When one switch is turned on or off, the other switch will automatically mirror the action, ensuring seamless synchronization between both switches.


## 🚀 Features

- **Bidirectional Synchronization:** Both switches stay in sync regardless of which one is toggled.
- **Loop Prevention:** Built-in conditions to avoid infinite loops or unnecessary state changes.
- **Restart Mode:** Handles rapid state changes smoothly using `restart` mode.
- **Delay 3s:** A slight delay to avoid bouncing issues.
- **Simple Configuration:** Easily set up through Home Assistant's UI.


## 📦 Installation

1. Download the `two_way_switch_synchronization.yaml` blueprint file.
2. In Home Assistant, navigate to **Settings > Automations & Scenes > Blueprints > Import Blueprint**.
3. Paste the raw GitHub URL of the blueprint or upload the `.yaml` file directly.
4. Follow the setup instructions in the Home Assistant UI.


## ⚙️ Configuration

- Select two switch entities to synchronize.
- Save and activate the automation.
- Test by toggling one switch and observing the synchronized behavior.

### Example Use Case

- Synchronize a physical wall switch with a smart switch to control the same light or device.
- Mirror the state of two smart switches to simplify control of multi-zone lighting or devices.


## 🛠️ Technical Details

- **Mode:** `restart`
- **Delay:** `3s`
- **Trigger:** State changes (`on` / `off`) of either switch.
- **Condition:** Prevents state change if already synchronized.


## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.
