# User Management

### `useradd`
- **Description**: Creates a new user.
- **useradd username**: Creates a user with the specified username.
- **useradd -m username**: Creates a user and their home directory.
- **useradd -G groupname username**: Creates a user and adds them to a group.

### `usermod`
- **Description**: Modifies an existing user account.
- **usermod -l newname oldname**: Renames a user.
- **usermod -aG groupname username**: Adds a user to a group.
- **usermod -d /new/home username**: Changes a user's home directory.

### `passwd`
- **Description**: Sets or changes a user's password.
- **passwd username**: Changes the password for the specified user.
- **passwd -l username**: Locks a user's account.
- **passwd -u username**: Unlocks a locked user account.

### `deluser`
- **Description**: Deletes a user account.
- **deluser username**: Removes a user but keeps their home directory.
- **deluser --remove-home username**: Removes a user and deletes their home directory.

## Group Management

### `groupadd`
- **Description**: Creates a new group.
- **groupadd groupname**: Creates a group with the specified name.

### `groupdel`
- **Description**: Deletes a group.
- **groupdel groupname**: Removes a group from the system.

### `gpasswd`
- **Description**: Manages group administrators and passwords.
- **gpasswd -a username groupname**: Adds a user to a group.
- **gpasswd -d username groupname**: Removes a user from a group.

## Switching Users & Permissions

### `su`
- **Description**: Switches to another user account.
- **su username**: Switches to the specified user.
- **su - username**: Switches to the specified user with their environment.

### `sudo`
- **Description**: Executes a command as another user (usually root).
- **sudo command**: Runs a command with superuser privileges.
- **sudo -u username command**: Runs a command as a specific user.

### `/etc/sudoers`
- **Description**: Configures user privileges for `sudo`.
- **visudo**: Safely edits the `/etc/sudoers` file.
- Example entry: `username ALL=(ALL) ALL` (Grants full sudo access to a user).
