**MailService.WebApi**
A lightweight .NET Web API for sending emails via SMTP. Ideal for microservices or monolithic applications requiring reliable email delivery.

✉️ **Features**
- Send e-mails using SMTP
- Configurable sender details via `appsettings.json`
- Minimal setup with RESTful endpoint

🔧 **Technologies**
- ASP.NET Core Web API – For building robust and scalable RESTful services
- C# – Strongly-typed, object-oriented language for maintainable backend logic
- MailKit - High-performance .NET email library used for handling SMTP communication
- .NET 7+ – Modern, cross-platform runtime powering the application’s performance and security

🚀 **Getting Started**
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
3. **Run the project**
  ```bash
  dotnet run
  ```
4. **Send a test e-mail**
Make a POST request to /api/email/send with the following JSON body:
  ```bash
  {
  "to": "recipient@example.com",
  "subject": "Hello",
  "body": "This is a test email."
}
  ```

