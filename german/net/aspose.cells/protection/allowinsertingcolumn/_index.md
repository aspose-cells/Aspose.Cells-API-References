---
title: "Protection.AllowInsertingColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection-Eigenschaft. Gibt an, ob das Einfügen von Spalten in einem geschützten Arbeitsblatt erlaubt ist."
type: docs
url: /de/net/aspose.cells/protection/allowinsertingcolumn/
---
## Protection.AllowInsertingColumn property

Stellt dar, ob das Einfügen von Spalten in einem geschützten Arbeitsblatt erlaubt ist

```csharp
public bool AllowInsertingColumn { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Abrufen der Schutz-Einstellungen
            Protection protection = worksheet.Protection;

            // Setzen Sie AllowInsertingColumn auf true
            protection.AllowInsertingColumn = true;

            // Überprüfen Sie die Einstellung
            Console.WriteLine("AllowInsertingColumn is set to: " + protection.AllowInsertingColumn);

            // Schützen Sie das Arbeitsblatt mit einem Passwort (unter Verwendung der Methode Workbook.Protect)
            workbook.Protect(ProtectionType.All, "password123");
            protection.AllowInsertingColumn = true; // Explicitly set again to demonstrate

            // Speichere die Arbeitsmappe
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


