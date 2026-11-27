---
title: "ChartTextFrame.IsDeleted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartTextFrame-egenskap. Anger om denna datamärkning är raderad"
type: docs
url: /sv/net/aspose.cells.charts/charttextframe/isdeleted/
---
## ChartTextFrame.IsDeleted property

Anger om denna datamärkning har raderats.

```csharp
public bool IsDeleted { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till datamärkningar och demonstrera IsDeleted-egenskapen
            chart.NSeries[0].DataLabels.ShowValue = true;
            bool isDeletedBefore = chart.NSeries[0].DataLabels.IsDeleted;
            
            // Ta bort datamärkningar genom att sätta ShowValue till falskt
            chart.NSeries[0].DataLabels.ShowValue = false;
            bool isDeletedAfter = chart.NSeries[0].DataLabels.IsDeleted;

            Console.WriteLine($"DataLabels IsDeleted before removal: {isDeletedBefore}");
            Console.WriteLine($"DataLabels IsDeleted after removal: {isDeletedAfter}");
        }
    }
}
```

### Se även

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


