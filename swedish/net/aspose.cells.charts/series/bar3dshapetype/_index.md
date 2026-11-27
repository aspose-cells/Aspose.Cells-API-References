---
title: "Series.Bar3DShapeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Hämtar eller anger 3D-formtypen som används med 3D-stapeldiagram eller kolumndiagram"
type: docs
url: /sv/net/aspose.cells.charts/series/bar3dshapetype/
---
## Series.Bar3DShapeType property

Hämtar eller anger 3D-formtypen som används med 3‑D stapel- eller kolumndiagram.

```csharp
public Bar3DShapeType Bar3DShapeType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBar3DShapeTypeDemo
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

            // Lägg till ett 3D-stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in stapelformtypen till Cylinder
            chart.NSeries[0].Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Spara arbetsboken
            workbook.Save("Bar3DShapeTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [Bar3DShapeType](../../bar3dshapetype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


