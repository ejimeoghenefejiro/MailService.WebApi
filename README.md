# MailService.WebApi

A lightweight .NET Web API for sending emails using SMTP. Designed for integration into microservices or monolithic architectures needing reliable mail delivery.

## ✉️ Features

- Send e-mails using SMTP
- Configurable sender details via `appsettings.json`
- Minimal setup with RESTful endpoint

## 🔧 Technologies

- ASP.NET Core Web API
- C#
- MailKit 
- .NET 7+

## 🚀 Getting Started

1. **Clone the repo**  
   ```bash
   git clone https://github.com/ejimeoghenefejiro/MailService.WebApi.git
   ```
2. **Configure SMTP**
Update the SMTP settings in appsettings.json:
    ```bash
    "SmtpSettings": {
    "Host": "smtp.example.com",
    "Port": 587,
    "SenderName": "Your App",
    "SenderEmail": "you@example.com",
    "Username": "smtp_user",
    "Password": "smtp_password"
    
    }
   ```
3.Run the project
  ```bash
  dotnet run
  ```
4.Send a test e-mail
POST to /api/email/send with JSON body:
  ```bash
  {
  "to": "recipient@example.com",
  "subject": "Hello",
  "body": "This is a test email."
}
  ```

