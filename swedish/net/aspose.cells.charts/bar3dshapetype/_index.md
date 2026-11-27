---
title: "Enum Bar3DShapeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.Bar3DShapeType enum. Representerar formen som används med 3D-stapeldiagrammet eller kolumndiagrammet"
type: docs
url: /sv/net/aspose.cells.charts/bar3dshapetype/
---
## Bar3DShapeType enumeration

Representerar formen som används med 3‑D‑stapeldiagrammet eller kolumndiagrammet.

```csharp
public enum Bar3DShapeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Box | `0` | Låda |
| PyramidToPoint | `1` | PyramidToPoint |
| PyramidToMax | `2` | PyramidToMax |
| Cylinder | `3` | Cylinder |
| ConeToPoint | `4` | ConeToPoint |
| ConeToMax | `5` | ConeToMax |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class Bar3DShapeTypeDemo
    {
        public static void Bar3DShapeTypeExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            // Lägger till ett nytt kalkylblad i Excel-objektet
            int sheetIndex = workbook.Worksheets.Add();
            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Lägger till exempelvärden i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Lägger till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 15, 5);
            // Åtkomst till instansen av det nyligen tillagda diagrammet
            Chart chart = worksheet.Charts[chartIndex];
            // Lägger till NSeries (diagramdatakälla) i diagrammet från cellen "A1" till "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Anger datakällan för kategoridata i NSeries
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];
            // Ställer in värdena för serien
            series.Values = "=B1:B4";

            // Ställer in 3D-formtypen för serien
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Sparar Excel-filen
            workbook.Save("Bar3DShapeTypeExample.xlsx");
            workbook.Save("Bar3DShapeTypeExample.pdf");

            // Ställer in 3D-formtypen för serien
            series.Bar3DShapeType = Bar3DShapeType.ConeToMax;

            // Sparar Excel-filen
            workbook.Save("Bar3DShapeTypeExample2.xlsx");
            workbook.Save("Bar3DShapeTypeExample2.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


