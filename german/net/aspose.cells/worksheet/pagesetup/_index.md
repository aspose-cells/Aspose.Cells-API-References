---
title: "Worksheet.PageSetup"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Stellt die Seitenlayoutbeschreibung in diesem Blatt dar"
type: docs
url: /de/net/aspose.cells/worksheet/pagesetup/
---
## Worksheet.PageSetup property

Stellt die Seitenlayoutbeschreibung in diesem Blatt dar.

```csharp
public PageSetup PageSetup { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPageSetupDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Seitenlayout-Eigenschaften festlegen
            worksheet.PageSetup.PrintArea = "A1:L50";
            worksheet.PageSetup.PrintTitleRows = "1:2";
            worksheet.PageSetup.PrintTitleColumns = "A:B";
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperA4;
            
            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PageSetupDemo.xlsx");
            
            Console.WriteLine("Worksheet page setup demo completed successfully.");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../../pagesetup/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


