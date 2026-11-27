---
title: "Series.ShapeProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Hämtar ShapePropertyCollection-objektet som innehåller de visuella formegenskaperna för serien"
type: docs
url: /sv/net/aspose.cells.charts/series/shapeproperties/
---
## Series.ShapeProperties property

Hämtar [`ShapePropertyCollection`](../../../aspose.cells.drawing/shapepropertycollection/) objektet som innehåller de visuella formegenskaperna för serien.

```csharp
public ShapePropertyCollection ShapeProperties { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShapePropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagramdata
            chart.NSeries.Add("Sheet1!B2:B4", true);
            chart.NSeries.CategoryData = "Sheet1!A2:A4";

            // Hämta den första serien och dess formegenskaper
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Konfigurera 3D-format och fasning
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;

            // Konfigurera material och belysning
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            // Ange seriefärger
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Spara arbetsboken
            workbook.Save("SeriesShapePropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [ShapePropertyCollection](../../../aspose.cells.drawing/shapepropertycollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


