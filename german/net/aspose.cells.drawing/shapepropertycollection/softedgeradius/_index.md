---
title: "ShapePropertyCollection.SoftEdgeRadius"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePropertyCollection-Eigenschaft. Gibt den Radius der Unschärfe, der auf die Kanten in Punkten angewendet wird, zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/shapepropertycollection/softedgeradius/
---
## ShapePropertyCollection.SoftEdgeRadius property

Liest und setzt den Radius der Unschärfe, die auf die Kanten angewendet wird, in Punkt-Einheiten.

```csharp
public double SoftEdgeRadius { get; set; }
```

### Beispiele

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

            // Erstelle ein Beispiel-Diagramm
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);

            chart.NSeries.Add("B1:B2", true);
            chart.NSeries.CategoryData = "A1:A2";

            // Greife auf Formeigenschaften der ersten Serie zu
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Konfiguriere 3D-Format und Abschrägung
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;

            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;

            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            shapeProperties.SoftEdgeRadius = 20;

            // Setze Serienfarben
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Speichere die Arbeitsmappe, um die Auswirkungen zu sehen
            workbook.Save("SoftEdgeRadiusDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


