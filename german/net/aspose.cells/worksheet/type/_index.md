---
title: "Worksheet.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Stellt den Arbeitsblatttyp dar"
type: docs
url: /de/net/aspose.cells/worksheet/type/
---
## Worksheet.Type property

Stellt den Arbeitsblatttyp dar.

```csharp
public SheetType Type { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige grundlegende Eigenschaften festlegen
            worksheet.Name = "DemoSheet";
            worksheet.IsVisible = true;
            
            // Demonstriere die Verwendung der Type‑Eigenschaft
            Console.WriteLine("Worksheet Type: " + worksheet.Type);
            
            // Ein Diagrammblatt hinzufügen, um verschiedene Arbeitsblatttypen zu demonstrieren
            workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[1];
            
            // Arbeitsblatttypen vergleichen
            Console.WriteLine("Regular Sheet Type: " + worksheet.Type);
            Console.WriteLine("Chart Sheet Type: " + chartSheet.Type);
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SheetType](../../sheettype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


