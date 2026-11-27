---
title: "ShapeCollection.AddShapeInChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addshapeinchart/
---
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int, byte[]) {#addshapeinchart_1}

Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagramområdet.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom, byte[] imageData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | MsoDrawingType | Ritningstypen. |
| placering | PlacementType | placerings typen. |
| vänster | Int32 | I enhet av 1/4000 av diagramområdets bredd. |
| top | Int32 | I enhet av 1/4000 av diagramområdets höjd. |
| höger | Int32 | I enhet av 1/4000 av diagramområdets bredd. |
| bottom | Int32 | I enhet av 1/4000 av diagramområdets höjd. |
| imageData | Byte[] | Om formen inte är en bild eller ole-objekt, ska imageData vara null. |

### Se även

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int) {#addshapeinchart}

Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagramområdet.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | MsoDrawingType | Ritningstypen. |
| placering | PlacementType | placerings typen. |
| vänster | Int32 | I enhet av 1/4000 av diagramområdets bredd. |
| top | Int32 | I enhet av 1/4000 av diagramområdets höjd. |
| höger | Int32 | I enhet av 1/4000 av diagramområdets bredd. |
| bottom | Int32 | I enhet av 1/4000 av diagramområdets höjd. |

### Exempel

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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Lägg till form i diagrammet
            chart.Shapes.AddShapeInChart(MsoDrawingType.CheckBox, PlacementType.Move, 100, 100, 1000, 1000);
            
            // Ange formtext
            chart.Shapes[0].Text = "Sample CheckBox";
            
            // Spara arbetsbok
            workbook.Save("AddShapeInChartWithMsoDrawingType.xlsx");
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


