Create new folder
```bash
mkdir SendGridMail
```

Move into to the new folder
```bash
cd SendGridMail
```

Create new .NET console application using .NET CLI
```
dotnet new console
```

Add SendGrid NuGet package
```
dotnet add package SendGrid
```

Set environment variable to store SendGrid API KEY:
```
export SENDGRID_API_KEY=[REPLACE WITH YOUR API KEY]
```

Update code.

Run project
```
dotnet run
```

If email not received, check https://app.sendgrid.com/email_activity for details.