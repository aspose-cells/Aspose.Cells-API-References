---
title: "WriteProtection.Password"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WriteProtection-Eigenschaft. Legt das geschützte Passwort zum Ändern der Datei fest"
type: docs
url: /de/net/aspose.cells/writeprotection/password/
---
## WriteProtection.Password property

Setzt das geschützte Passwort, um die Datei zu ändern.

```csharp
public string Password { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Schreibschutz-Passwort festlegen
            workbook.Settings.WriteProtection.Password = "owner";
            
            // Speichere die Arbeitsmappe
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            Console.WriteLine("Workbook write-protected with password successfully.");
        }
    }
}
```

### Siehe auch

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


