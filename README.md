# Periodic Process Logger with Auto-Scheduled Log Report Facility

This Python script periodically logs information about all running processes on the system and sends the log file through email. The script uses `psutil` for process information, `schedule` for scheduling tasks, and `smtplib` for sending emails.

## Features

- **Periodic Logging**: Logs running processes at user-defined intervals.
- **Log File Creation**: Creates a log file in the `Marvellous` directory.
- **Email Notification**: Sends the log file via email.
- **Internet Connectivity Check**: Checks for internet connectivity before sending the email.

## Technologies Used

- Python
- `psutil` for process information
- `schedule` for task scheduling
- `smtplib` for email functionality

## Prerequisites

- Python 3.x
- Required Python packages:
  - `psutil`
  - `schedule`

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/your-repository.git
    cd your-repository
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. Install the required dependencies:
    ```bash
    pip install psutil schedule
    ```

## Usage

To run the script, provide the time interval in minutes as a command-line argument:

```bash
python your_script.py <interval>
