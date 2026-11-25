---
title: "Protection.GetPasswordHash"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Protection. Ottiene l'hash della password corrente"
type: docs
url: /it/net/aspose.cells/protection/getpasswordhash/
---
## Protection.GetPasswordHash method

Ottiene l'hash della password corrente.

```csharp
public int GetPasswordHash()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodGetPasswordHashDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta le impostazioni di protezione con password
            Protection protection = worksheet.Protection;
            protection.Password = "password123";
            protection.AllowDeletingColumn = true;
            protection.AllowFormattingCell = true;
            
            // Proteggi il foglio di lavoro
            worksheet.Protect(ProtectionType.All);

            try
            {
                // Ottieni l'hash della password
                int passwordHash = protection.GetPasswordHash();
                
                // Visualizza il risultato
                Console.WriteLine($"Password hash: {passwordHash}");
                Console.WriteLine($"Is protected with password: {protection.IsProtectedWithPassword}");

                // Verifica la password (dimostrando la funzionalità correlata)
                bool isVerified = protection.VerifyPassword("password123");
                Console.WriteLine($"Password verification result: {isVerified}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPasswordHash method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ProtectionMethodGetPasswordHashDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


