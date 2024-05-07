# To-Do-App-FastAPI


### Micky Malvino Kusandiwinata
### 2602174522
### Class L4CC

---------

| Endpoint          | Method | Description                                     | Body Request                                        | Body Response                                      | Error Response                                     |
|-------------------|--------|-------------------------------------------------|-----------------------------------------------------|----------------------------------------------------|----------------------------------------------------|
| /createTask       | POST   | Create a Task with provided ID and Title        | `{ "id": {id}, "title": "{title}", "completed": false }` | `{ "id": {id}, "title": "{title}", "completed": false }` | `{"error": "Task not found"}`                     |
| /getTaskByID/{task_id} | GET    | Get a task by its ID                            | -                                                   | `{ "id": {id}, "title": "{title}", "completed": {completed} }` | `{"error": "Task not found"}`                     |
| /getTaskByTitle/{title} | GET    | Get task by its title                       | -                                                   | `[{ "id": {id}, "title": "{title}", "completed": {completed} }]` | `{"error": "No tasks found with title '{title}'"}` |
| /deleteByID/{task_id}   | DELETE | Delete a task by its ID                         | `{ "id": {id}, "title": "{title}", "completed": false }` | `{"message": "Task deleted successfully"}`        | `{"error": "Task not found"}`                     |
| /deleteByTitle/{title}  | DELETE | Delete task by its title                     | `{ "id": {id}, "title": "{title}", "completed": false }` | `{"message": "All tasks with title '{title}' deleted successfully"}` | `{"error": "No tasks found with title '{title}'"}` |
| /deleteAll       | DELETE | Delete all tasks                                | `{ "id": {id}, "title": "{title}", "completed": false }` | `{"message": "All tasks deleted successfully"}`   | -                                                  |
| /getAllTasks     | GET    | Get all tasks                                   | `{ "id": {id}, "title": "{title}", "completed": false }` | `[{ "id": {id}, "title": "{title}", "completed": false }]` | -                                                  |
| /updateTask/{task_id}   | PUT    | Update a task by providing a new data          | `{ "id": {id}, "title": "{title}", "completed": {completed} }` | `{"message": "Task updated successfully"}`        | `{"error": "Task not found"}`                     |

-------


<img width="1728" alt="Screenshot 2024-05-07 at 22 19 12" src="https://github.com/mmalvino/To-Do-App-FastAPI/assets/114371813/1a1f2433-7396-43ee-9fcc-ba9e1ca8fdae">
