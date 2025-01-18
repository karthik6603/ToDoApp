# Todo App

## Overview
A modern and interactive Todo application to help users manage their tasks effectively. The app provides features to add, mark, and delete tasks while maintaining a visually appealing and user-friendly interface.

---

## Features
- **Add Tasks:** Add new tasks with ease using the input field.
- **Mark Tasks as Complete:** Use checkboxes to mark tasks as done.
- **Delete Tasks:** Remove unwanted tasks with a simple delete button.
- **Data Persistence:** Tasks are stored locally using the browser's Local Storage.
- **Responsive Design:** Fully optimized for both desktop and mobile devices.

---

## Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Local Storage:** For task persistence

---

## Folder Structure
```
project-folder
├── index.html     # Main HTML file
├── style.css      # Styling for the application
├── script.js      # JavaScript logic for functionality
├── icons          # Icons used in this project
└── README.md      # Project documentation
```

---

## How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd project-folder
   ```
3. Open the `index.html` file in any modern browser.

---

## Code Snippets
### Task Addition
```javascript
function addTodo() {
    const todotext = todoInput.value.trim();
    if (todotext.length > 0) {
        const todoObject = {
            text: todotext,
            conpleted: false,
        };
        allTodos.push(todoObject);
        createTodoItem(todoObject, allTodos.length - 1);
        updateTodoList();
        saveTodos();
        todoInput.value = "";
    }
}
```
### Responsive Styling
```css
@media (max-width: 640px) {
    body {
        padding: 1rem;
    }

    h1 {
        font-size: 2.5rem;
        margin-bottom: 1.5rem;
    }

    form {
        flex-direction: column;
    }

    #add-button {
        width: 100%;
    }

    .todo {
        padding: 1rem;
    }
}
```

---

## Design Highlights
- **Thematic Colors:** Uses CSS variables for a consistent theme.
- **Hover Effects:** Interactive hover effects on buttons and tasks.
- **Responsive Layout:** Fluid layout adapts seamlessly to smaller screens.

---

## Screenshots
1. **Desktop View:**
   ![Desktop View](screenshot-desktop.png)
2. **Mobile View:**
   ![Mobile View](screenshot-mobile.png)

---

## Future Enhancements
- Add a due date feature for tasks.
- Include a priority system for tasks.
- Option to categorize tasks into groups.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.
