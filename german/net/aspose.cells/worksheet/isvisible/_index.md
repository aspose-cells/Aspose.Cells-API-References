---
title: "Worksheet.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt an, ob das Arbeitsblatt sichtbar ist"
type: docs
url: /de/net/aspose.cells/worksheet/isvisible/
---
## Worksheet.IsVisible property

Stellt dar, ob das Arbeitsblatt sichtbar ist.

```csharp
public bool IsVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie 3 Arbeitsblätter hinzu
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Setzen Sie das zweite Arbeitsblatt auf verborgen
            workbook.Worksheets[1].IsVisible = false;
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetVisibilityDemo.xlsx");
            
            // Zeigen Sie den Sichtbarkeitsstatus an
            Console.WriteLine("Worksheet Visibility Status:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Console.WriteLine($"{workbook.Worksheets[i].Name}: {(workbook.Worksheets[i].IsVisible ? "Visible" : "Hidden")}");
            }
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


