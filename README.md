Certainly! Below is a readme file with explanations for the provided Bash script:

```markdown
# internsctl Bash Script Readme

## Overview
`internsctl` is a Bash script designed to provide system-related information and perform basic system operations. It supports commands related to CPU, memory, user management, and file information.

## Usage
```bash
./internsctl <command> [options] [arguments]
```

### Commands:
- **cpu getinfo**: Display CPU information.
- **memory getinfo**: Display Memory information.
- **user create \<username\>**: Create a new user.
- **user list**: List all regular users.
- **user list --sudo-only**: List users with sudo permissions.
- **file getinfo \<file-name\> [options]**: Display information about a file.

### Options for File Command:
- **--size, -s**: Print file size.
- **--permissions, -p**: Print file permissions.
- **--owner, -o**: Print file owner.
- **--last-modified, -m**: Print last modified time.

## Functions
### 1. `display_help`
Displays the script usage information.

### 2. `display_version`
Displays the script version.

### 3. `get_cpu_info`
Displays CPU information using the `lscpu` command.

### 4. `get_memory_info`
Displays memory information using the `free -m` command.

### 5. `create_user`
Creates a new user. Requires a username as an argument.

### 6. `list_users`
Lists all regular users or users with sudo permissions based on the presence of the `--sudo-only` option.

### 7. `get_file_info`
Displays basic information about a file, such as permissions, size, owner, and last modified time.

### 8. `get_file_info_with_options`
Displays specific information about a file based on the provided option.

## How to Run
1. Make the script executable:
   ```bash
   chmod +x internsctl
   ```
2. Run the script:
   ```bash
   ./internsctl <command> [options] [arguments]
   ```

## Examples
```bash
./internsctl cpu getinfo
./internsctl memory getinfo
./internsctl user create john_doe
./internsctl user list --sudo-only
./internsctl file getinfo sample.txt
./internsctl file getinfo sample.txt --size
```


## Version History
- Version: 0.1.0
