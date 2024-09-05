
### GitHub Stats Inflator

This project is an automated script that creates and configures a cron job to run a GitHub stats inflator script daily at 7:00 AM. The inflator script performs automatic commits to a text file, simulating coding activity.

### Project Structure

```
inflator/
    banner
    cron-creator
    inflate
    setup
README.md
work/
    working_hard.txt
```

- **[`inflator/setup`](./inflator/setup)**: Configuration script that guides the user through the setup process.
- **[`inflator/cron-creator`](./inflator/cron-creator)**: Script that creates a cron job to execute the inflator script.
- **[`inflator/inflate`](./inflator/inflate)**: Main script that performs automatic commits.
- **[`work/working_hard.txt`](./work/working_hard.txt)**: Text file where automatic commits are logged.

## Installation

1. Clone this repo and change directory to the root of this project.

2. Change permissions for setup, inflate and cron-creator scripts.
   ```sh
   chmod +x setup inflate cron-creator
   ```
2. Execute setup script.
   ```sh
   ./setup
   ```

## Usage

The setup script will do the following:
1. Display a welcome banner.
2. Test an execution of the inflate script.
3. Create a cron job that will run the inflate script daily at 7:00 AM.

### Manual inflate execution

If you want to manually execute the inflation script, you can do it with the following command:
```sh
./inflate <number_of_commits>
```

## Requisites

- Git installed and configured on the system.
- Superuser permissions to create cron jobs.

## Contributions

Contributions are welcome. Please open an issue or a pull request on GitHub.

## License

This project is licensed under the [MIT License](./LICENCE).
