---
title: "AbstractLowCodeProtectionProvider.GetWorksheetPassword"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractLowCodeProtectionProvider-Methode. Gibt das Passwort zurück, um das angegebene Arbeitsblatt zu schützen"
type: docs
url: /de/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/
---
## AbstractLowCodeProtectionProvider.GetWorksheetPassword method

Liefert das Passwort zum Schützen des angegebenen Arbeitsblatts.

```csharp
public virtual string GetWorksheetPassword(string sheetName)
```

### Rückgabewert

Passwort zum Schutz des angegebenen Arbeitsblatts.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetPasswordWithStringDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            string sheetName = worksheet.Name;

            // Erstelle eine benutzerdefinierte Instanz des Schutz-Providers
            var provider = new CustomProtectionProvider();

            try
            {
                // Rufe GetWorksheetPassword mit dem Arbeitsblattnamen auf
                string password = provider.GetWorksheetPassword(sheetName);

                // Schütze das Arbeitsblatt mit dem abgerufenen Passwort
                worksheet.Protect(ProtectionType.All, password, null);

                Console.WriteLine($"Protected worksheet '{sheetName}' with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorksheetPassword: {ex.Message}");
            }

            // Speichern Sie die geschützte Arbeitsmappe
            workbook.Save("WorksheetPasswordDemo.xlsx");

        }
    }

    // Benutzerdefinierte Implementierung, die das Passwort basierend auf dem Blattnamen zurückgibt
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public new string GetWorksheetPassword(string sheetName)
        {
            // Einfache Passwortgenerierungslogik zur Demonstration
            return $"pw_{sheetName}";
        }
    }
}
```

### Siehe auch

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


