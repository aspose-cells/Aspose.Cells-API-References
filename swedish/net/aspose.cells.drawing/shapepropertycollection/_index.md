---
title: "Klassen ShapePropertyCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShapePropertyCollection klass. Denna klass specificerar de visuella formegenskaperna för ett diagramelement eller en form"
type: docs
url: /sv/net/aspose.cells.drawing/shapepropertycollection/
---
## ShapePropertyCollection class

Denna klass specificerar de visuella formegenskaperna för ett diagram‑element eller en form.

```csharp
public class ShapePropertyCollection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Format3D](../../aspose.cells.drawing/shapepropertycollection/format3d/) { get; } | Representerar ett [`Format3D`](./format3d/) objekt som specificerar 3D-formegenskaper för diagramelementet eller formen. |
| [GlowEffect](../../aspose.cells.drawing/shapepropertycollection/gloweffect/) { get; } | Representerar ett [`GlowEffect`](./gloweffect/) objekt som specificerar glödeffekt för diagramelementet eller formen. |
| [ShadowEffect](../../aspose.cells.drawing/shapepropertycollection/shadoweffect/) { get; } | Representerar ett [`ShadowEffect`](./shadoweffect/) objekt som specificerar skuggeffekt för diagramelementet eller formen. |
| [SoftEdgeRadius](../../aspose.cells.drawing/shapepropertycollection/softedgeradius/) { get; set; } | Hämtar och anger radien för oskärpa som ska tillämpas på kanterna, i enheten punkter. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ClearFormat3D](../../aspose.cells.drawing/shapepropertycollection/clearformat3d/)() | Rensar 3D-formegenskaperna för formen. |
| [ClearGlowEffect](../../aspose.cells.drawing/shapepropertycollection/cleargloweffect/)() | Rensar glödeffekten för formen. |
| [ClearShadowEffect](../../aspose.cells.drawing/shapepropertycollection/clearshadoweffect/)() | Rensar skuggeffekten för diagrammet eller formen. |
| [HasFormat3D](../../aspose.cells.drawing/shapepropertycollection/hasformat3d/)() | Anger om formen har 3D-formatdata. |
| [HasGlowEffect](../../aspose.cells.drawing/shapepropertycollection/hasgloweffect/)() | Anger om formen har glödeffektdata. |
| [HasShadowEffect](../../aspose.cells.drawing/shapepropertycollection/hasshadoweffect/)() | Anger om formen har skuggeffektdata. |

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePropertyCollectionDemo
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

            // Ange seriefärger
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Spara arbetsboken
            workbook.Save("ShapePropertyCollectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


