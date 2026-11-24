---
title: "Protection.GetPasswordHash"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection method. Gibt den Hash des aktuellen Passworts zurück"
type: docs
url: /de/net/aspose.cells/protection/getpasswordhash/
---
## Protection.GetPasswordHash method

Ermittelt den Hash des aktuellen Passworts.

```csharp
public int GetPasswordHash()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodGetPasswordHashDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Schutzeinstellungen mit Passwort festlegen
            Protection protection = worksheet.Protection;
            protection.Password = "password123";
            protection.AllowDeletingColumn = true;
            protection.AllowFormattingCell = true;
            
            // Schützen Sie das Arbeitsblatt
            worksheet.Protect(ProtectionType.All);

            try
            {
                // Hash des Passworts abrufen
                int passwordHash = protection.GetPasswordHash();
                
                // Ergebnis anzeigen
                Console.WriteLine($"Password hash: {passwordHash}");
                Console.WriteLine($"Is protected with password: {protection.IsProtectedWithPassword}");

                // Passwort überprüfen (demonstriert verwandte Funktionalität)
                bool isVerified = protection.VerifyPassword("password123");
                Console.WriteLine($"Password verification result: {isVerified}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPasswordHash method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ProtectionMethodGetPasswordHashDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


