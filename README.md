# MailPlosive

MailPlosive is an email bombing tool designed for penetration testing purposes. This tool allows you to send a large number of emails to a target address using Gmail, Yahoo, or Outlook as SMTP servers.

**DISCLAIMER: This tool is intended for legal penetration testing and educational purposes only. Do not use it for illegal activities.**

## Features

- Supports multiple modes for sending varying numbers of emails (customizable).
- Easy configuration of SMTP settings.
- Compatible with major email services like Gmail, Yahoo, and Outlook.
- Automatic rate-limiting to avoid sending too many emails too fast.

## Requirements

- Python 3.x
- smtplib (Python built-in library)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/xenigmus/mailplosive.git
    ```

2. Navigate to the project directory:

    ```bash
    cd mailplosive
    ```

3. Install necessary dependencies (if any). The `smtplib` library is built into Python, so no additional installations should be necessary for this tool.

## Usage

1. Run the tool:

    ```bash
    python mailplosive.py
    ```

2. Enter the required information (target email, SMTP server, number of emails, etc.) as prompted.

## Supported SMTP Services

- **Gmail**: `smtp.gmail.com`
- **Yahoo**: `smtp.mail.yahoo.com`
- **Outlook**: `smtp-mail.outlook.com`

### Example

```bash
python mailplosive.py
# Output:
Initializing program
Enter the target mail: target@example.com
Enter Bomb Mode (1,2,3,4) || 1:(1000) || 2:(500) || 3:(250) || 4:(Custom): 1
Setting up Bomber...
You have chosen Mode: 1 (1000)
Enter from Address: example@gmail.com
Enter from Password: yourapppassword
Enter the Subject: Test Bomb
Enter the message: This is a test.
