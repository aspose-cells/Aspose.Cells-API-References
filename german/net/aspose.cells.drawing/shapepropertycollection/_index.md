---
title: "Klasse ShapePropertyCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapePropertyCollection Klasse. Diese Klasse gibt die visuellen Formeigenschaften für ein Diagrammelement oder eine Form an."
type: docs
url: /de/net/aspose.cells.drawing/shapepropertycollection/
---
## ShapePropertyCollection class

Diese Klasse gibt die visuellen Formeigenschaften für ein Diagrammelement oder eine Form an.

```csharp
public class ShapePropertyCollection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Format3D](../../aspose.cells.drawing/shapepropertycollection/format3d/) { get; } | Stellt ein [`Format3D`](./format3d/) Objekt dar, das 3D-Formeigenschaften für das Diagrammelement oder die Form festlegt. |
| [GlowEffect](../../aspose.cells.drawing/shapepropertycollection/gloweffect/) { get; } | Stellt ein [`GlowEffect`](./gloweffect/) Objekt dar, das den Leuchteffekt für das Diagrammelement oder die Form festlegt. |
| [ShadowEffect](../../aspose.cells.drawing/shapepropertycollection/shadoweffect/) { get; } | Stellt ein [`ShadowEffect`](./shadoweffect/) Objekt dar, das den Schatteneffekt für das Diagrammelement oder die Form festlegt. |
| [SoftEdgeRadius](../../aspose.cells.drawing/shapepropertycollection/softedgeradius/) { get; set; } | Liest und setzt den Radius der Unschärfe, die auf die Kanten angewendet wird, in Punkt-Einheiten. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ClearFormat3D](../../aspose.cells.drawing/shapepropertycollection/clearformat3d/)() | Löscht die 3D-Formeigenschaften der Form. |
| [ClearGlowEffect](../../aspose.cells.drawing/shapepropertycollection/cleargloweffect/)() | Löscht den Leuchteffekt der Form. |
| [ClearShadowEffect](../../aspose.cells.drawing/shapepropertycollection/clearshadoweffect/)() | Entfernt den Schatteneffekt des Diagrammelements oder der Form. |
| [HasFormat3D](../../aspose.cells.drawing/shapepropertycollection/hasformat3d/)() | Gibt an, ob die Form 3D-Formatdaten enthält. |
| [HasGlowEffect](../../aspose.cells.drawing/shapepropertycollection/hasgloweffect/)() | Gibt an, ob die Form Leuchteffekt-Daten enthält. |
| [HasShadowEffect](../../aspose.cells.drawing/shapepropertycollection/hasshadoweffect/)() | Gibt an, ob die Form Schatteneffekt-Daten enthält. |

### Beispiele

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

            // Setze Serienfarben
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapePropertyCollectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


