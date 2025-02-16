# Linux Process Management

## Viewing Running Processes

### `ps`
- **Description**: Displays currently running processes.
- **ps aux**: Shows all running processes with detailed information.
- **ps -ef**: Shows all processes in a different format.

### `top`
- **Description**: Displays real-time information about system resource usage and running processes.
- **q**: Quit `top`.
- **k**: Kill a process by entering its PID.

### `htop`
- **Description**: An interactive, user-friendly version of `top` (requires installation).
- **Arrow Keys**: Navigate between processes.
- **F9**: Kill a process.

## Managing Processes

### `kill`
- **Description**: Terminates a process using its PID.
- **kill PID**: Sends the default signal (TERM) to terminate a process.
- **kill -9 PID**: Forcefully kills a process.

### `pkill`
- **Description**: Terminates a process by name.
- **pkill process_name**: Kills a process by its name.

### `nice`
- **Description**: Starts a process with a specific priority.
- **nice -n 10 command**: Starts a process with lower priority.

### `renice`
- **Description**: Changes the priority of a running process.
- **renice -n 5 -p PID**: Changes the priority of a process.
