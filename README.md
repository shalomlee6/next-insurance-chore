# Your broken Tasks Widget
Complete as many tasks as can before deadline.
The order is up to you :)
Feel free to remove code and implement your own version, or change it anyway you like.
You can use any resource you like, and ask us questions during the session. 

## Tasks:
1.  Tasks should persist after closing the browser. ( 5pt )
# Question 1 => use local storage NOT as const in store.js => // const localStorage = window.sessionStorage;
# data in localStorage doesn't expire, data in sessionStorage is cleared when the page session ends.
2.  Prevent duplication in tasks. ( 10pt )
#   in store.js insert methode => i check for duplicates in todos
#   using => todos.find( (todoItem) =>  todoItem.title==item.title ? todoItem : null) 
#   NOT WORKING...
3.  Fix the `clear completed` action in the footer ( 15pt )

4.  After doubleClick on an item, clicking enter should exit "edit" (10pt)
# In bindEditItemCancel set keyupevent for exsit to enter

5.  Fix Style issue when inserts a lot of items - add short description for how you approach it (5pt)
# Question five => using overflow-y: 'scrol' so that the task items will stay in the ul with scrolling && remove max-height: 300px.

6.  When launching the app for the first time, the `addItem` input should be in focus (5pt)
#   add focus => bindAddItem in view.js to this.$newTodo.focus();

7.  Fix the counter on the footer (5pt)
#  in controller class in _filter methode set from 0 to active items

8.  Add a code comment explaining what `delegateEvent` function does (10pt)
# delegateEvent map an event such as double click to the specific function to envoke that event.
# example:
#     delegateEvent(event-src/target, UI Element selector, event-type, callback function to trigger   )       
#     delegateEvent(this.$todoList, 'li label', 'dblclick', ({ target }) => {
#      this.editItem(target);
#    });
#
9.  Load and display tasks from https://jsonplaceholder.typicode.com/todos when application loads (20pt)

10. Prevent adding task that contain `< >` in the title. (replace with blank), For example: 'Learn < JS >' should become 'Learn JS' (10pt) 
11. Handle the error in the console (15pt)

Good luck! 
