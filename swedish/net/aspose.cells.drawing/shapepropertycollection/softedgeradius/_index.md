---
title: "ShapePropertyCollection.SoftEdgeRadius"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePropertyCollection egenskap. Hämtar och anger suddradien för kanterna i enheter av punkter"
type: docs
url: /sv/net/aspose.cells.drawing/shapepropertycollection/softedgeradius/
---
## ShapePropertyCollection.SoftEdgeRadius property

Hämtar och anger radien för oskärpa som ska tillämpas på kanterna, i enheten punkter.

```csharp
public double SoftEdgeRadius { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShapePropertyCollectionPropertySoftEdgeRadiusDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett exempeldiagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);

            chart.NSeries.Add("B1:B2", true);
            chart.NSeries.CategoryData = "A1:A2";

            // Åtkomst till formegenskaper för den första serien
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Konfigurera 3D-format och fasning
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;

            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;

            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            shapeProperties.SoftEdgeRadius = 20;

            // Ange seriefärger
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Spara arbetsboken för att se effekterna
            workbook.Save("SoftEdgeRadiusDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


