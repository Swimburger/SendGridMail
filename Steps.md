Create new folder
```bash
mkdir SendGridMail
```

Move into to the new folder
```bash
cd SendGridMail
```

Create new .NET console application using .NET CLI
```bash
dotnet new console
```

Add SendGrid NuGet package
```bash
dotnet add package SendGrid
```

Set environment variable to store SendGrid API KEY:
```bash
export SENDGRID_API_KEY=[REPLACE WITH YOUR API KEY]
```

Update code.

Run project
```bash
dotnet run
```

If email not received, check https://app.sendgrid.com/email_activity for details.

Add the following packages:
```bash
dotnet add package Microsoft.Extensions.Hosting
dotnet add package Microsoft.Extensions.Configuration.UserSecret
```

Update code

Create appsettings.json.

Initialize user-secrets for your project:
```bash
dotnet user-secrets init
```

Set the SendGrid API Key in the User Secrets store:
```bash
dotnet user-secrets set SendGridApiKey [PASTE IN YOUR SENDGRID API KEY]
```

dotnet run --environment Development


dotnet add package SendGrid.Extensions.DependencyInjection