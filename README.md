

```markdown
# `internsctl`

`internsctl` is a custom Linux command that provides various system information and user management functionalities.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/shivamsinghcse/LinuxInterview.git
   ```

2. Make the script executable:

   ```bash
   chmod +x internsctl
   ```

3. Run the script:

   ```bash
   ./internsctl --help
   ```

## Usage

### CPU Information

```bash
./internsctl cpu getinfo
```

Display detailed information about the CPU.

### Memory Information

```bash
./internsctl memory getinfo
```

Display information about system memory.

### User Management

#### Create User

```bash
./internsctl user create <username>
```

Create a new user with the specified username.

#### List Users

```bash
./internsctl user list [--sudo-only]
```

List all regular users or users with sudo permissions. Use the `--sudo-only` option to list users with sudo permissions.

### File Information

#### Get File Info

```bash
./internsctl file getinfo <file-name>
```

Get detailed information about a file, including size, permissions, owner, and last modification time.

#### Options for File Info

```bash
./internsctl file getinfo [options] <file-name>
```

Options:
- `--size`, `-s`: Print file size.
- `--permissions`, `-p`: Print file permissions.
- `--owner`, `-o`: Print file owner.
- `--last-modified`, `-m`: Print last modification time.

## Options

- `--version`: Display the version of the command.
- `--help`: Display usage information.

## Examples

```bash
./internsctl cpu getinfo
./internsctl memory getinfo
./internsctl user create john_doe
./internsctl user list
./internsctl user list --sudo-only
./internsctl file getinfo my_file.txt
./internsctl file getinfo --size my_file.txt
```

