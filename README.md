Javascript

The code starts by defining four variables using document.querySelector() to select DOM elements by their class name. These elements are the input field for adding new to-do items, the button for adding new to-do items, the list of existing to-do items, and a select element for filtering the to-do list by status.

Next, the code adds event listeners to the todoButton, todoList, and filterOption elements, which call corresponding functions to handle the events.

The addTodo() function is called when the todoButton is clicked, and it creates a new to-do item by creating new DOM elements for a div, li, and two button elements. It then adds these elements to the todoList, and saves the new to-do item to local storage using the saveLocalTodos() function.

The deleteCheck() function is called when a click event occurs within the todoList, and it handles deleting or completing a to-do item depending on which button was clicked. If the "trash" button is clicked, the corresponding to-do item is removed from the DOM and local storage using the removeLocalTodos() function. If the "complete" button is clicked, the corresponding to-do item is toggled between a "completed" and "incomplete" status by adding or removing a "completed" class from its parent div element.

The filterTodo() function is called when the value of the filterOption select element is changed, and it filters the displayed to-do items according to the selected status ("all", "completed", or "incomplete").

The saveLocalTodos(), getLocalTodos(), and removeLocalTodos() functions are used to manage the storage of to-do items in the browser's local storage. saveLocalTodos() saves a new to-do item to local storage, getLocalTodos() retrieves all stored to-do items from local storage and displays them in the todoList, and removeLocalTodos() removes a to-do item from local storage.

Overall, this code demonstrates the use of event listeners, DOM manipulation, and local storage in building a simple to-do list application.

HTML