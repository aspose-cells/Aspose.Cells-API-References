---
title: "Protection.VerifyPassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Protection. Verifica la password"
type: docs
url: /it/net/aspose.cells/protection/verifypassword/
---
## Protection.VerifyPassword method

Verifica la password.

```csharp
public bool VerifyPassword(string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | La password. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodVerifyPasswordWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Proteggi il foglio di lavoro con una password
            worksheet.Protection.AllowDeletingColumn = false;
            worksheet.Protection.AllowDeletingRow = false;
            worksheet.Protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            try
            {
                // Verifica la password
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
            
            // Salva la cartella di lavoro
            workbook.Save("ProtectionMethodVerifyPasswordWithStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


