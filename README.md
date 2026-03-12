# TaskGenerator

Automates commit workflows and updates task status in ClickUp using TASK ID.

## Requirements

- Python 3.10+
- See requirements.txt

## Setup

1. Create and activate a virtual environment.
2. Install dependencies:

   pip install -r requirements.txt

## Usage

- Create a .env file with the required variables.
- Run the script from the project root.

### Script parameters

The script accepts the following parameters (short and long forms are equivalent):

- `-t` / `--task-id`: ClickUp task ID (example: `-t abc123`).
- `-s` / `--status`: New ClickUp status to set (example: `-s "in review"`).
- `-m` / `--message`: Git commit message (example: `-m "feat: add login page"`).
- `-b` / `--branch`: Remote branch to push to. Optional; defaults to the current Git branch (example: `-b main`).

Example:

   python src/clickup_commit_script.py -t abc123 -s "in review" -m "feat: add login page" -b main

