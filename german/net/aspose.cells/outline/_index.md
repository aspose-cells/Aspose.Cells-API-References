---
title: "Klasse Outline"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Outline‑Klasse. Stellt eine Gliederung in einem Arbeitsblatt dar"
type: docs
url: /de/net/aspose.cells/outline/
---
## Outline class

Stellt eine Gliederung in einem Arbeitsblatt dar.

```csharp
public class Outline
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [SummaryColumnRight](../../aspose.cells/outline/summarycolumnright/) { get; set; } | Gibt an, ob die Zusammenfassungsspalte rechts von den Detailspalten in der Gliederung positioniert wird. |
| [SummaryRowBelow](../../aspose.cells/outline/summaryrowbelow/) { get; set; } | Gibt an, ob die Zusammenfassungszeile unter den Detailzeilen in der Gliederung positioniert wird. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OutlineDemo
    {
        public static void OutlineExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt in der Arbeitsmappe zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greife auf die Gliederung des Arbeitsblatts zu
            Outline outline = worksheet.Outline;
            
            // Setze die Eigenschaften der Gliederung
            outline.SummaryRowBelow = true; // Indicates if the summary row will be positioned below the detail rows
            outline.SummaryColumnRight = true; // Indicates if the summary column will be positioned to the right of the detail columns
            
            // Speichere die Arbeitsmappe
            workbook.Save("OutlineExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


