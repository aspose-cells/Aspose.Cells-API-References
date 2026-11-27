---
title: "ShapePropertyCollection.ClearShadowEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePropertyCollection metod. Rensar skuggeffekten på diagrammet eller formen"
type: docs
url: /sv/net/aspose.cells.drawing/shapepropertycollection/clearshadoweffect/
---
## ShapePropertyCollection.ClearShadowEffect method

Rensar skuggeffekten för diagrammet eller formen.

```csharp
public void ClearShadowEffect()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShapePropertyCollectionMethodClearShadowEffectDemo
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

            ShadowEffect shadowEffect = shapeProperties.ShadowEffect;
            shadowEffect.Size = 1.5;
            shadowEffect.Color.Color = Color.Red;
            shadowEffect.Angle = 180;

            // Ange seriefärger
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            workbook.Save("ShapePropertyCollectionMethodClearShadowEffectDemo.xlsx");

            shapeProperties.ClearShadowEffect();

            // Spara resultatet
            workbook.Save("ShapePropertyCollectionMethodClearShadowEffectDemo2.xlsx");
        }
    }
}
```

### Se även

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


