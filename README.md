<a id="readme-top"></a>

# TO-DO CLI 📝

This is a simple Command Line Interface (CLI) application for managing to-do lists. 
<br/>
It allows users to create, view, update, and delete tasks directly from their terminal. All tasks are stored in a local JSON file for easy access.

## Prerequisites 📌

- Go (v1.18 or later)
- Git
- VS Code (or any other text editor)

## Installation 🔧

1. Clone the repository:
    ```console
    git clone https://github.com/rahulxyzten/todo-cli.git
    ```

2. Navigate to the project directory:
    ```console
    cd todo-cli
    ```

3. Install dependencies:
    ```console
    go mod tidy
    ```

4. Build the application:
    ```console
    go build -o todo.exe
    ```
    
## Usage 📅

Once you've built the application, you can start using it!

**Add a New Task**
<br/>
To add a task, use the `-add` flag followed by the task description:
  ```console
  ./todo -add <text message>
  ```

**List All Tasks**
<br/>
To display all the tasks, use the `-list` flag:
  ```console
  ./todo -list
  ```

**Toggle a Task**
<br/>
To toggle a task as done or undone, use the `-toggle` flag followed by the task index (start from 0):
  ```console
  ./todo -toggle <index>
  ```

**Edit a Task**
<br/>
To edit a specific task, use the `-edit` flag followed by the task index and new task description:
  ```console
  ./todo -edit <index>:<text message>
  ```

**Delete a Task**
<br/>
To delete a task, use the `-del` flag followed by the task index:
  ```console
  ./todo -del <index>
  ```

**See all commands**
<br/>
To get a list of all available commands, use the `--help` flag:
  ```console
  ./todo --help
  ```

## Example Workflow 💡

1. Add tasks:
    ```console
    ./todo -add "Eat"
    ./todo -add "Code"
    ./todo -add "Sleep"
    ./todo -add "Repeat"
    ```

2. Mark tasks 1 & 2 as done:
    ```console
    ./todo -toggle 0
    ./todo -toggle 1
    ```
    
3. Edit task 2:
    ```console
    ./todo -edit 1:"Make Project"
    ```

4. Delete task 4:
    ```console
    ./todo -del 3
    ```

5. List tasks:
    ```console
    ./todo -list
    ```

1. Output:
<img src="https://github.com/user-attachments/assets/99554338-1526-4361-aa70-5573f0d77a43" alt="output" />
   
## Task Storage 🗂️

All tasks are stored in a `.todos.json` file in the root directory of the project. You can manually edit this file if needed.

<br/>
<br/>
<p align="center">Stay Organized, Stay Productive! ⏰🔥</p>
<p align="center">
  <a href="#">
    <img src="https://forthebadge.com/images/badges/built-with-love.svg" alt="Built with Love">
  </a>
</p>

<p align="right">(<a href="#readme-top">back to top</a>)</p>
