---
title: "Worksheet.UniqueId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die eindeutige ID zurück und setzt sie; sie ist dieselbe wie 15DB5C3CA5A148AF8F253D86AC232D4F."
type: docs
url: /de/net/aspose.cells/worksheet/uniqueid/
---
## Worksheet.UniqueId property

Ruft die eindeutige ID ab und setzt sie; sie ist identisch mit {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

```csharp
public string UniqueId { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyUniqueIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle eine eindeutige ID für das Arbeitsblatt.
            string uniqueId = "{" + Guid.NewGuid().ToString() + "}";
            
            // Setze die UniqueId‑Eigenschaft des ersten Arbeitsblatts.
            workbook.Worksheets[0].UniqueId = uniqueId;
            
            // Speichere die Arbeitsmappe
            string outputPath = "SheetUniqueIdDemo.xlsx";
            workbook.Save(outputPath);
            
            // Lade die Arbeitsmappe neu, um zu überprüfen, dass die UniqueId erhalten bleibt.
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Gib die UniqueId aus, um die Funktionalität zu demonstrieren.
            Console.WriteLine("Worksheet UniqueId: " + loadedWorkbook.Worksheets[0].UniqueId);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


