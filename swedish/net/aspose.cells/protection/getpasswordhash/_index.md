---
title: "Protection.GetPasswordHash"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Skyddmetod. Hämtar hashvärdet för aktuellt lösenord"
type: docs
url: /sv/net/aspose.cells/protection/getpasswordhash/
---
## Protection.GetPasswordHash method

Hämtar hashvärdet för det aktuella lösenordet.

```csharp
public int GetPasswordHash()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodGetPasswordHashDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in skyddsinställningar med lösenord
            Protection protection = worksheet.Protection;
            protection.Password = "password123";
            protection.AllowDeletingColumn = true;
            protection.AllowFormattingCell = true;
            
            // Skydda kalkylbladet
            worksheet.Protect(ProtectionType.All);

            try
            {
                // Hämta lösenordshash
                int passwordHash = protection.GetPasswordHash();
                
                // Visa resultatet
                Console.WriteLine($"Password hash: {passwordHash}");
                Console.WriteLine($"Is protected with password: {protection.IsProtectedWithPassword}");

                // Verifiera lösenordet (demonstrerar relaterad funktionalitet)
                bool isVerified = protection.VerifyPassword("password123");
                Console.WriteLine($"Password verification result: {isVerified}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPasswordHash method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("ProtectionMethodGetPasswordHashDemo.xlsx");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


