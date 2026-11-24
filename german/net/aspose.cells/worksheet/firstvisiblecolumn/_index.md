---
title: "Worksheet.FirstVisibleColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Stellt den Index der ersten sichtbaren Spalte dar"
type: docs
url: /de/net/aspose.cells/worksheet/firstvisiblecolumn/
---
## Worksheet.FirstVisibleColumn property

Stellt den Index der ersten sichtbaren Spalte dar.

```csharp
public int FirstVisibleColumn { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erste Spalte ausblenden (Index 0)
            worksheet.Cells.HideColumn(0);
            
            // Den Index der ersten sichtbaren Spalte abrufen und anzeigen
            Console.WriteLine("First visible column index: " + worksheet.FirstVisibleColumn);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FirstVisibleColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


