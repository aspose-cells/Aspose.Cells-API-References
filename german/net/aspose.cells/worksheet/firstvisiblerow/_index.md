---
title: "Worksheet.FirstVisibleRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt den Index der ersten sichtbaren Zeile an"
type: docs
url: /de/net/aspose.cells/worksheet/firstvisiblerow/
---
## Worksheet.FirstVisibleRow property

Stellt den Index der ersten sichtbaren Zeile dar.

```csharp
public int FirstVisibleRow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten festlegen
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Setzen Sie die erste sichtbare Zeile auf Zeile 20
            worksheet.FirstVisibleRow = 20;
            
            // Zeigen Sie die erste sichtbare Zeile an
            Console.WriteLine("First visible row: " + worksheet.FirstVisibleRow);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FirstVisibleRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


