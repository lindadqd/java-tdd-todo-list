

# User stories

As a user I want to be able to:
- add tasks to my todo list.
- see all the tasks in my todo list.
- change the status of a task between incomplete and complete.
- to get only the complete tasks.
- to get only the incomplete tasks.
- search for a task and receive a message that says it wasn't found if it doesn't exist.
- remove tasks from my list.
- see all the tasks in my list ordered alphabetically in ascending order.
- see all the tasks in my list ordered alphabetically in descending order.


| Classes  | Methods                                                                        | Scenario                                      | Output                                     |
|----------|--------------------------------------------------------------------------------|-----------------------------------------------|--------------------------------------------|
| ToDoList | void addTask (Map<'String,String> toDoList, String task)                       | if task not in list                           | add task to toDoList                       |
|          |                                                                                | if task already in list                       | return false                               |
|          | void printTask(Map<'String,String> toDoList)                                   | if toDolist is empty                          | return false                               |
|          |                                                                                | if toDoList contains atleast one task         | print task(s) in list                      |
|          | void changeStatus(Map<'String,String> toDoList, String task)                   | if task in toDoList                           | change status                              |
|          |                                                                                | if task not in toDoList                       | return false                               |
|          | List<String'> completeTasks(Map<'String,String> toDoList)                      | if toDoList contains completed tasks          | return completed tasks                     |
|          |                                                                                | if toDoList does not contain completed tasks  | return empty list                          |
|          | List <String'> incompleteTasks(Map<'String,String> toDoList)                   | if toDoList contains incomplete tasks         | return uncompleted tasks                   |
|          |                                                                                | if toDoList does not contain incomplete tasks | return empty list                          |
|          | String searchTask(Map<'String,String> toDoList, String task)                   | if task does not exist                        | "The task was not found"                   |
|          |                                                                                | if task exist                                 | return false                               |
|          | void removeTask(Map<'String,String> toDoList, String task)                     | if task is in toDoList                        | remove task from toDoList                  |
|          |                                                                                | if task not in toDoList                       | return false                               |
|          | Map<String,String> ascendingList sortAscending(Map<'String,String> toDoList)   | if toDoList not empty                         | return sorted toDoList in ascending order  |
|          |                                                                                | if toDoList is empty                          | return empty list                          |
|          | Map<String,String> descendingList sortDescending(Map<'String,String> toDoList) | if toDoList not empty                         | return sorted toDoList in descending order |
|          |                                                                                | if toDoList empty                             | return empty list                          |