---
title: "Format3D.LightingAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Format3D. Получает и задает угол освещения. Диапазон от 0 до 359,9 градусов"
type: docs
url: /ru/net/aspose.cells.drawing/format3d/lightingangle/
---
## Format3D.LightingAngle property

Получает и задает угол освещения. Диапазон от 0 до 359,9 градусов.

```csharp
public double LightingAngle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class Format3DPropertyLightingAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            Series series = chart.NSeries[0];
            Format3D format3D = series.ShapeProperties.Format3D;

            format3D.SurfaceMaterialType = PresetMaterialType.Metal;
            format3D.LightingAngle = 45;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;

            workbook.Save("Format3DLightingAngleDemo.xlsx");
            Console.WriteLine("Workbook saved with 3D lighting angle set to 45 degrees.");
        }
    }
}
```

### См. также

* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


