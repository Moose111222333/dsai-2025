
## 🧭 Lab 4 Focus Recap

### 🌐 What Happens:

**Lab 4** advances the agent from making **confidence-only decisions** to making **context-aware decisions**. It introduces **external sensors and environmental rules** to influence actions.

| Step       | Role in Lab 4                                                                                   |
| ---------- | ----------------------------------------------------------------------------------------------- |
| **Sense**  | Read both classifier output *and* environment (e.g. temperature, deck rules, time, light level) |
| **Plan**   | Combine confidence + external factors to decide if action should be taken                       |
| **Act**    | Trigger output (LED, buzzer, GPIO) *only if conditions are met*                                 |
| **Log**    | Output decision reasoning to Serial or screen                                                   |
| **Repeat** | Continue loop and re-evaluate on each input                                                     |

---

### 🧠 Key Agent Behavior:

* **Multi-source decision-making**
  → Decisions depend on both the model output *and* the current **environmental state**

> 🔄 Example:
> Classifier says "YES" to placing a block,
> but temperature sensor reads 90°F → result = "REJECT" due to overheating

---

### 🧰 What Students Build:

* Integrate sensors (e.g., temp, light, deck state)
* Implement rules that govern safe/unsafe actions
* Add **conditional logic branches** in FSM
* Make agent behavior **situational**, not rigid

---

### 🧠 Learning Goals of Lab 4:

* Use multiple data sources for decision-making
* Build more realistic, safety-aware agents
* Reinforce FSM branching and control structure
* Introduce the concept of **operating rules or policies**

---

### ✅ Script Name:

```plaintext
lab4_contextual_decision_agent.ino
```
![image](https://github.com/user-attachments/assets/1f4e2225-619c-4531-b5b8-a0a7780f690a)





