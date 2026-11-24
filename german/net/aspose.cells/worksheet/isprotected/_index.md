---
title: "Worksheet.IsProtected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt an, ob das Arbeitsblatt geschützt ist"
type: docs
url: /de/net/aspose.cells/worksheet/isprotected/
---
## Worksheet.IsProtected property

Gibt an, ob das Arbeitsblatt geschützt ist.

```csharp
public bool IsProtected { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Schützen Sie die Arbeitsmappe und das erste Arbeitsblatt
            workbook.Protect(ProtectionType.All, "password");
            workbook.Worksheets[0].Protect(ProtectionType.All, "password", null);

            // Prüfen Sie, ob das Arbeitsblatt geschützt ist
            bool isProtected = workbook.Worksheets[0].IsProtected;
            Console.WriteLine($"Worksheet is protected: {isProtected}");

            // Speichere die Arbeitsmappe
            workbook.Save("protected_worksheet.xlsx");

            // Laden Sie die gespeicherte Arbeitsmappe und überprüfen Sie den Schutz
            Workbook loadedWorkbook = new Workbook("protected_worksheet.xlsx");
            Console.WriteLine($"Loaded worksheet is protected: {loadedWorkbook.Worksheets[0].IsProtected}");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


