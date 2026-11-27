---
title: "Protection.VerifyPassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection-metod. Verifierar lösenordet"
type: docs
url: /sv/net/aspose.cells/protection/verifypassword/
---
## Protection.VerifyPassword method

Verifierar lösenord.

```csharp
public bool VerifyPassword(string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | String | Lösenordet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodVerifyPasswordWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skydda arbetsbladet med ett lösenord
            worksheet.Protection.AllowDeletingColumn = false;
            worksheet.Protection.AllowDeletingRow = false;
            worksheet.Protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            try
            {
                // Verifiera lösenordet
                bool isPasswordCorrect = worksheet.Protection.VerifyPassword("password123");
                
                Console.WriteLine($"Password verification result: {isPasswordCorrect}");
                
                if (isPasswordCorrect)
                {
                    Console.WriteLine("The provided password matches the worksheet protection password.");
                }
                else
                {
                    Console.WriteLine("The provided password does not match the worksheet protection password.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing VerifyPassword method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("ProtectionMethodVerifyPasswordWithStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


