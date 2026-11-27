---
title: "Area.Formatting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Area-egenskap. Representerar formateringen av området"
type: docs
url: /sv/net/aspose.cells.drawing/area/formatting/
---
## Area.Formatting property

Representerar formateringen av området.

```csharp
public FormattingType Formatting { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyFormattingDemo
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
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till diagramområde och ställ in formatering
            ChartArea chartArea = chart.ChartArea;
            chartArea.Area.Formatting = FormattingType.None;

            // Spara arbetsboken
            workbook.Save("AreaPropertyFormattingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [FormattingType](../../../aspose.cells.charts/formattingtype/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


