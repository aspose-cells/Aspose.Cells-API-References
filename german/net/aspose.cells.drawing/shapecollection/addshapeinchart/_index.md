---
title: "ShapeCollection.AddShapeInChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Fügt eine Form zum Diagramm hinzu. Alle Einheiten sind 1/4000 der Diagrammfläche"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addshapeinchart/
---
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int, byte[]) {#addshapeinchart_1}

Füge ein Shape zum Diagramm hinzu. Alle Einheiten sind 1/4000 der Diagrammfläche.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom, byte[] imageData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | MsoDrawingType | Der Zeichnungstyp. |
| Platzierung | PlacementType | Der Platzierungstyp. |
| links | Int32 | In Einheiten von 1/4000 der Diagrammbreite. |
| oben | Int32 | In Einheiten von 1/4000 der Diagrammhöhe. |
| rechts | Int32 | In Einheiten von 1/4000 der Diagrammbreite. |
| unten | Int32 | In Einheiten von 1/4000 der Diagrammhöhe. |
| imageData | Byte[] | Wenn die Form kein Bild oder OLE-Objekt ist, sollte imageData null sein. |

### Siehe auch

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int) {#addshapeinchart}

Füge ein Shape zum Diagramm hinzu. Alle Einheiten sind 1/4000 der Diagrammfläche.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | MsoDrawingType | Der Zeichnungstyp. |
| Platzierung | PlacementType | Der Platzierungstyp. |
| links | Int32 | In Einheiten von 1/4000 der Diagrammbreite. |
| oben | Int32 | In Einheiten von 1/4000 der Diagrammhöhe. |
| rechts | Int32 | In Einheiten von 1/4000 der Diagrammbreite. |
| unten | Int32 | In Einheiten von 1/4000 der Diagrammhöhe. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeInChartWithMsoDrawingTypePlacementTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Form zum Diagramm hinzufügen
            chart.Shapes.AddShapeInChart(MsoDrawingType.CheckBox, PlacementType.Move, 100, 100, 1000, 1000);
            
            // Formtext festlegen
            chart.Shapes[0].Text = "Sample CheckBox";
            
            // Arbeitsmappe speichern.
            workbook.Save("AddShapeInChartWithMsoDrawingType.xlsx");
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


