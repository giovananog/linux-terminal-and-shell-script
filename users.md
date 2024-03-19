# User Management Commands

- `adduser name` - Add a user with the name 'name'.

- `deluser name` - Remove the user 'name'.

- The `/etc/passwd` file contains information about users, such as user names, UIDs (User IDs), GIDs (Group IDs), home directories, shells, etc.

- `useradd -d /opt/dir -s /bin/bash -` - Add a user with a specified home directory (`/opt/dir`) and default shell (`/bin/bash`).

- `passwd name` - Redefine a password for the user 'name'.

- `su name` - Switch to the user 'name'.  (name have to be in the sudo group)

- `adduser name sudo` - Add the user 'name' to the sudo group, granting administrative permissions.

- `su name` - Switch to the user 'name'.

- `deluser name sudo` - Remove the user 'name' from the sudo group, revoking administrative permissions.

- `whoami` - Show the current username.

- `groups` - Display the groups to which the current user belongs.

- `id` - Display user and group information for the current user.

- `sudo command` - Execute a command with administrative privileges.