# Task-Commander

Task-Commander is a comprehensive tool for managing and running scripts in a containerized environment. It allows you to upload, delete, list, and update scripts, with each script running in its own isolated Docker container. This ensures consistency and isolation, making it ideal for software developers and computer science students.

## Features

- **Upload Scripts**: Upload your scripts to the containerized environment.
- **Delete Scripts**: Remove scripts from the environment.
- **List Scripts**: List all uploaded scripts with metadata.
- **Update Scripts**: Update existing scripts without the need for deletion and re-upload.
- **Isolated Execution**: Each script runs in its own Docker container, ensuring isolation and consistency.

## Installation

### Using Docker

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/yourusername/task-commander.git
    cd task-commander
    ```

2. **Build the Docker Image**:
    ```sh
    docker build -t task_commander .
    ```

## Usage

### Uploading a Script

Upload a script to the containerized environment:
```sh
docker run --rm -v ~/Documents/new-personal-projects/project:/app task_commander add /app/scripts/example_script.py
