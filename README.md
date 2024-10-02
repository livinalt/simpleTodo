# SimpleTodo Smart Contract

## Description
The `SimpleTodo` contract is a basic to-do list manager built on Solidity. It allows users to create, update, delete, and retrieve tasks. Each task is stored in a struct containing the following fields:
- `Id`: The task's unique identifier.
- `title`: The task's title.
- `description`: A brief description of the task.
- `status`: The current status of the task.

The contract also includes functionality for updating the task status and retrieving all tasks.

## Contract Features
- **Create a Todo**: Add a new to-do item to the list.
- **Update a Todo**: Modify the title, description, or status of an existing to-do.
- **Update Status**: Change the status of an existing to-do.
- **Delete a Todo**: Remove a to-do item from the list.
- **Retrieve a Todo**: Fetch a specific to-do item by its `Id`.
- **Get All Todos**: Retrieve the complete list of todos.
- **Get Todo Status**: Fetch the status of a specific todo.

## Functions
1. `createTodo(string memory _title, string memory _desc, string memory _status)`
   - Adds a new todo with the specified title, description, and status.
   
2. `updateTodoList(uint256 _id, string memory _title, string memory _desc, string memory _status) returns (Todo memory)`
   - Updates the specified todo's title, description, and status.
   
3. `updateStatus(uint256 _id, string memory _status) returns (Todo memory)`
   - Updates the status of a todo by its `Id`.
   
4. `deleteTodoList(uint256 _id)`
   - Removes a todo from the list.
   
5. `retrieveTodo(uint256 _id) view returns (Todo memory)`
   - Retrieves a todo by its `Id`.
   
6. `getAllList() view returns (Todo[] memory)`
   - Returns the entire list of todos.
   
7. `getStatus(uint256 _id) view returns (string memory)`
   - Returns the status of a specific todo by its `Id`.

## Deployment Details
- **Contract Address**: [0x85A6673ba9BD53B8d78C37A062D598B4E52959ef](https://sepolia-blockscout.lisk.com/address/0x85A6673ba9BD53B8d78C37A062D598B4E52959ef#code)
  
- **Blockchain Explorer**: Successfully verified on the Sepolia Blockscout explorer.

