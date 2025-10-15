# ✅ To-Do List Web App

A simple and efficient **To-Do List** application built using **HTML**, **CSS**, and **JavaScript**.
This app allows users to **sign up, log in, add, edit, delete, and manage daily tasks** — all within the browser.

---

## 🚀 Features

🧍 **User Authentication** — Sign up and log in to manage your own personal to-do list.
📝 **Add Tasks** — Create tasks with titles and optional descriptions.
✏️ **Edit Tasks** — Update tasks anytime with one click.
✅ **Mark as Complete** — Check off tasks as you finish them.
🗑️ **Delete Tasks** — Remove unwanted or completed tasks easily.
💾 **Persistent Data** — Tasks and user info are stored locally using LocalStorage.
🎨 **Responsive Design** — Clean and user-friendly interface that adapts to all screen sizes.

---

## ⚙️ Project Logic

This To-Do List app is fully client-side and stores all information using **browser LocalStorage** — no backend needed.
Below is the working logic of the app:

### 🔐 1. Authentication (Signup & Login)

* **Signup:**

  * User enters a username, email, and password.
  * Checks whether the email already exists in LocalStorage.
  * If new, saves user info as:

    ```js
    { id, username, email, password }
    ```
  * Redirects to login after successful signup.
* **Login:**

  * Validates entered credentials with stored user data.
  * If valid, saves the session as `currentUser` in LocalStorage.
  * Redirects the user to the To-Do Dashboard.

---

### 🧾 2. Add Task

* User inputs a task title and optional description.
* Each task is saved as:

  ```js
  {
    id: 1,
    userId: currentUser.id,
    title: "Finish homework",
    description: "Complete before 6 PM",
    completed: false,
    createdAt: "2025-10-15T10:00:00Z"
  }
  ```
* The task is stored in LocalStorage under the key `"tasks"`.
* Tasks are instantly displayed on the dashboard.

---

### ✏️ 3. Edit Task

* The app allows editing existing tasks by updating their title or description.
* Updated details are saved back to LocalStorage.

---

### ✅ 4. Mark Task as Complete

* Clicking the checkbox toggles the `completed` property.
* The task UI changes visually (e.g., line-through text or faded color).

---

### 🗑️ 5. Delete Task

* Removes a selected task after user confirmation.
* Updates LocalStorage and re-renders the task list.

---

### 🚪 6. Logout

* Clears the `currentUser` session from LocalStorage.
* Redirects the user back to the login page.

---

## 🛠️ Tech Stack

| Layer        | Technology             |
| ------------ | ---------------------- |
| **Frontend** | HTML, CSS, JavaScript  |
| **Storage**  | Browser LocalStorage   |
| **Design**   | Responsive, minimal UI |

---

## 📸 Screenshots

<img width="1894" height="883" alt="image" src="https://github.com/user-attachments/assets/a10f17ab-f1c7-4f3b-ae11-13cf0c368860" />
<img width="1880" height="882" alt="image" src="https://github.com/user-attachments/assets/1d42aa3d-9b57-4296-92a8-ff660a7a5a3e" />



---

## ⚙️ How to Use

1️⃣ **Clone the repository**

```bash
git clone https://github.com/yourusername/todo-list-app.git
```

2️⃣ **Open the project folder**

```bash
cd todo-list-app
```

3️⃣ **Run the app**
Simply open `index.html` in your browser.

4️⃣ **Start managing your tasks!**
Sign up or log in to create, update, and track your to-do items.

---

## 🌐 Live Demo
🔗 (https://to-dolst.netlify.app/)

---

## 🌟 Future Enhancements

* 📅 Add due dates and reminders for each task
* 🏷️ Introduce task categories (Work, Study, Personal, etc.)
* 📊 Add progress analytics and completion charts
* 🔐 Integrate backend authentication (Node.js or Firebase)
* 🌙 Add dark/light mode toggle

---

## 🧑‍💻 Author

**Ayusmita Bardoloi**
🌐 [github](https://github.com/ayusmitabardoloi)

---


