# sysopctl

**sysopctl** is a command-line tool designed for system administrators to easily manage system services, monitor system performance, analyze logs, manage disk usage, and perform backups. 

## Features

- **Service Management**: Start, stop, and list services.
- **System Monitoring**: Display system load averages.
- **Disk Usage**: View disk usage statistics.
- **Process Monitoring**: Monitor running processes in real-time.
- **Log Analysis**: Analyze recent critical system logs.
- **Backup**: Easily back up directories to a specified location.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
  - [Commands](#commands)
  - [Examples](#examples)
- [License](#license)

## Installation

To install `sysopctl`, follow these steps:

1. Clone the repository or download the `sysopctl` script:
    ```bash
    git clone https://github.com/your-username/sysopctl.git
    ```

2. Make the script executable:
    ```bash
    chmod +x sysopctl
    ```

3. Move the script to a directory in your `$PATH` for global access:
    ```bash
    sudo mv sysopctl /usr/local/bin/
    ```

4. Optionally, create a manual page:
    ```bash
    sudo cp sysopctl.1 /usr/share/man/man1/
    sudo mandb
    ```

Now, you can run `sysopctl` from any terminal.

## Usage

### Commands

`sysopctl` supports the following commands:

- `--version`  
  Displays the version of the tool.
  
- `--help`  
  Displays a list of available commands and usage instructions.

- `service list`  
  Lists all currently running services.

- `service start <name>`  
  Starts a specified service.

- `service stop <name>`  
  Stops a specified service.

- `system load`  
  Displays the current system load averages.

- `disk usage`  
  Displays disk usage statistics.

- `process monitor`  
  Monitors running processes in real-time.

- `logs analyze`  
  Analyzes recent critical system logs.

- `backup <path>`  
  Creates a backup of the specified path in the user's home directory.

### Examples

1. **Display the version**:
    ```bash
    sysopctl --version
    ```

2. **List all running services**:
    ```bash
    sysopctl service list
    ```

3. **Start the `nginx` service**:
    ```bash
    sysopctl service start nginx
    ```

4. **Check system load averages**:
    ```bash
    sysopctl system load
    ```

5. **Analyze recent critical logs**:
    ```bash
    sysopctl logs analyze
    ```

6. **Backup a directory (e.g., Desktop)**:
    ```bash
    sysopctl backup ~/Desktop
    ```

## Error Handling

The tool includes robust error handling to notify users when they provide incorrect arguments or encounter issues with service management. Common errors will display clear instructions on how to fix them.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
