---
title: "ShapeCollection.AddShapeInChartByScale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt dem Diagramm eine Form hinzu. Alle Einheiten sind prozentuale Skalierung des Diagrammbereichs"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addshapeinchartbyscale/
---
## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double) {#addshapeinchartbyscale}

Füge ein Shape zum Diagramm hinzu. Alle Einheiten sind prozentualer Maßstab der Diagrammfläche.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | MsoDrawingType | Der Zeichnungstyp. |
| Platzierung | PlacementType | Der Platzierungstyp. |
| links | Double | Einheit ist prozentuale Skalierung der Diagrammbereichsbreite. |
| oben | Double | Einheit ist prozentuale Skalierung der Diagrammbereichshöhe. |
| rechts | Double | Einheit ist prozentuale Skalierung der Diagrammbereichsbreite. |
| unten | Double | Einheit ist prozentuale Skalierung der Diagrammbereichshöhe. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeInChartByScaleWithMsoDrawingTypePlacementTypeDouDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Diagramm berechnen
            chart.Calculate();

            // Füge dem Diagramm eine Rechteckform mit skalaren Koordinaten hinzu
            Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle, 
                PlacementType.Move,
                0.2,  // x1 (20% from left)
                0.2,  // y1 (20% from top)
                0.4,  // x2 (40% from left)
                0.4); // y2 (40% from top)
            rectangle.Fill.SolidFill.Color = Color.Blue;
            rectangle.Line.SolidFill.Color = Color.Black;

            // Füge dem Diagramm eine Ovalform mit skalaren Koordinaten hinzu
            Shape oval = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Oval,
                PlacementType.Move,
                0.6,  // x1 (60% from left)
                0.6,  // y1 (60% from top)
                0.8,  // x2 (80% from left)
                0.8); // y2 (80% from top)
            oval.Fill.SolidFill.Color = Color.Red;
            oval.Line.SolidFill.Color = Color.Black;

            // Speichere die Arbeitsmappe
            workbook.Save("AddShapeInChartByScaleWithMsoDrawingType.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double, byte[]) {#addshapeinchartbyscale_1}

Füge ein Shape zum Diagramm hinzu. Alle Einheiten sind 1/4000 der Diagrammfläche.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom, byte[] imageData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | MsoDrawingType | Der Zeichnungstyp. |
| Platzierung | PlacementType | Der Platzierungstyp. |
| links | Double | Einheit ist prozentuale Skalierung der Diagrammbereichsbreite. |
| oben | Double | Einheit ist prozentuale Skalierung der Diagrammbereichshöhe. |
| rechts | Double | Einheit ist prozentuale Skalierung der Diagrammbereichsbreite. |
| unten | Double | Einheit ist prozentuale Skalierung der Diagrammbereichshöhe. |
| imageData | Byte[] | Wenn die Form kein Bild oder OLE-Objekt ist, sollte imageData null sein. |

### Siehe auch

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


