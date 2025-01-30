# Automated Gmail sender


## Setup instructions

To use this script, you'll need to follow these steps:

1. First, set up Google App Password:
- Go to your Google Account settings
- Navigate to Security > 2-Step Verification
- At the bottom, click on "App passwords"
- Generate a new app password for your Python script
- Save this password safely (you'll only see it once)


Use the script
```
# Create the sender object
sender = GmailSender("your.email@gmail.com", "your-app-password")

sender.send_email(
    to_email="recipient@example.com",
    subject="Hello!",
    body="This is an automated email."
)

# Use the below script to send the email via attachments
sender.send_email(
    to_email="recipient@example.com",
    subject="Report",
    body="Please find the attached report.",
    attachments=["report.pdf", "data.xlsx"]
)
```

