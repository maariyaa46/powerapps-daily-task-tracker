# ✅ Power Apps – Daily Task Tracker (Canvas App)

This repository contains a Microsoft Power Apps **Canvas App** for managing daily tasks. It enables users to **create**, **view**, **edit**, and **delete** tasks through a clean and responsive interface, with all data securely stored in **Microsoft Dataverse**.

---

## 🚀 Overview

The **Daily Task Tracker App** is a simple and efficient productivity tool that helps users:

- Add new tasks via a form
- Track progress with status and priority fields
- Organize tasks by category
- Update or delete tasks as needed

Built with **Canvas App UI** and **Dataverse** as the data backend, this app demonstrates the power of low-code development for daily use cases.

---

## 🔗 Data Source

The app is connected to a single Dataverse table named: **`Tasks`**

### 📄 Dataverse Table: `Tasks`

| Column Name  | Data Type | Description |
|--------------|-----------|-------------|
| `Task Name`  | Text      | Name or title of the task |
| `Due Date`   | Date/Time | Deadline or target completion date |
| `Category`   | Choice    | Task category (e.g., Work, Personal, Urgent) |
| `Status`     | Choice    | Current progress status (e.g., To Do, In Progress, Done) |
| `Priority`   | Choice    | Task importance (e.g., Low, Medium, High) |

---

## 🧭 How the App Works

### 🖥️ UI Layout
- **Top/Side Form**: For entering new task data or editing selected tasks
- **Gallery**: Displays all existing tasks in a scrollable list
- Each gallery item shows key info and buttons for:
  - **Edit**: Load data into the form for update
  - **Delete**: Remove the task from Dataverse

---

## 🔧 Functionality

### ✅ Add Task
- User fills out `Task Name`, `Due Date`, selects `Category`, `Status`, and `Priority`
- Form submits data to Dataverse's `Tasks` table

### ✏️ Edit Task
- Tapping an item loads it into the form
- After editing, user saves changes back to Dataverse

### ❌ Delete Task
- Pressing the delete icon on a gallery item removes it from the table

---

### 2. Recreate the Dataverse Table
Manually create a table called **`Tasks`** with the following columns:

- `Task Name`: Text
- `Due Date`: Date/Time
- `Category`: Choice (create a new global or local choice set like: Work, Personal, Urgent, Other)
- `Status`: Choice (e.g., To Do, In Progress, Done)
- `Priority`: Choice (e.g., Low, Medium, High)



