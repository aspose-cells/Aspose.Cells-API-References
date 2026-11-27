---
title: "ShapeCollection.AddShapeInChartByScale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägg till en shape i diagrammet. Alla enheter är procentuell skala av diagramområdet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addshapeinchartbyscale/
---
## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double) {#addshapeinchartbyscale}

Lägg till en form i diagrammet. Alla enheter är i procent av diagramområdet.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | MsoDrawingType | Ritningstypen. |
| placering | PlacementType | placerings typen. |
| vänster | Double | Enheten är procentuell skala av diagramområdets bredd. |
| top | Double | Enheten är procentuell skala av diagramområdets höjd. |
| höger | Double | Enheten är procentuell skala av diagramområdets bredd. |
| bottom | Double | Enheten är procentuell skala av diagramområdets höjd. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Beräkna diagrammet
            chart.Calculate();

            // Lägg till en rektangelshape i diagrammet med skalkoordinater
            Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle, 
                PlacementType.Move,
                0.2,  // x1 (20% from left)
                0.2,  // y1 (20% from top)
                0.4,  // x2 (40% from left)
                0.4); // y2 (40% from top)
            rectangle.Fill.SolidFill.Color = Color.Blue;
            rectangle.Line.SolidFill.Color = Color.Black;

            // Lägg till en oval shape i diagrammet med skalkoordinater
            Shape oval = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Oval,
                PlacementType.Move,
                0.6,  // x1 (60% from left)
                0.6,  // y1 (60% from top)
                0.8,  // x2 (80% from left)
                0.8); // y2 (80% from top)
            oval.Fill.SolidFill.Color = Color.Red;
            oval.Line.SolidFill.Color = Color.Black;

            // Spara arbetsboken
            workbook.Save("AddShapeInChartByScaleWithMsoDrawingType.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double, byte[]) {#addshapeinchartbyscale_1}

Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagramområdet.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom, byte[] imageData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | MsoDrawingType | Ritningstypen. |
| placering | PlacementType | placerings typen. |
| vänster | Double | Enheten är procentuell skala av diagramområdets bredd. |
| top | Double | Enheten är procentuell skala av diagramområdets höjd. |
| höger | Double | Enheten är procentuell skala av diagramområdets bredd. |
| bottom | Double | Enheten är procentuell skala av diagramområdets höjd. |
| imageData | Byte[] | Om formen inte är en bild eller ole-objekt, ska imageData vara null. |

### Se även

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


