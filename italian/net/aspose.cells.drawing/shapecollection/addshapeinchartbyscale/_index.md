---
title: "ShapeCollection.AddShapeInChartByScale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge una forma al grafico. Tutte le unità sono in scala percentuale dell'area del grafico"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addshapeinchartbyscale/
---
## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double) {#addshapeinchartbyscale}

Aggiungi una forma al grafico. Tutta l'unità è in scala percentuale dell'area del grafico.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | MsoDrawingType | Il tipo di disegno. |
| posizionamento | PlacementType | il tipo di posizionamento. |
| sinistra | Double | L'unità è la scala percentuale della larghezza dell'area del grafico. |
| alto | Double | L'unità è la scala percentuale dell'altezza dell'area del grafico. |
| destra | Double | L'unità è la scala percentuale della larghezza dell'area del grafico. |
| basso | Double | L'unità è la scala percentuale dell'altezza dell'area del grafico. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Calcola il grafico
            chart.Calculate();

            // Aggiungi una forma rettangolare al grafico usando coordinate in scala
            Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle, 
                PlacementType.Move,
                0.2,  // x1 (20% from left)
                0.2,  // y1 (20% from top)
                0.4,  // x2 (40% from left)
                0.4); // y2 (40% from top)
            rectangle.Fill.SolidFill.Color = Color.Blue;
            rectangle.Line.SolidFill.Color = Color.Black;

            // Aggiungi una forma ovale al grafico usando coordinate in scala
            Shape oval = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Oval,
                PlacementType.Move,
                0.6,  // x1 (60% from left)
                0.6,  // y1 (60% from top)
                0.8,  // x2 (80% from left)
                0.8); // y2 (80% from top)
            oval.Fill.SolidFill.Color = Color.Red;
            oval.Line.SolidFill.Color = Color.Black;

            // Salva la cartella di lavoro
            workbook.Save("AddShapeInChartByScaleWithMsoDrawingType.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double, byte[]) {#addshapeinchartbyscale_1}

Aggiungi una forma al grafico. Tutta l'unità è 1/4000 dell'area del grafico.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom, byte[] imageData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | MsoDrawingType | Il tipo di disegno. |
| posizionamento | PlacementType | il tipo di posizionamento. |
| sinistra | Double | L'unità è la scala percentuale della larghezza dell'area del grafico. |
| alto | Double | L'unità è la scala percentuale dell'altezza dell'area del grafico. |
| destra | Double | L'unità è la scala percentuale della larghezza dell'area del grafico. |
| basso | Double | L'unità è la scala percentuale dell'altezza dell'area del grafico. |
| imageData | Byte[] | Se la forma non è un'immagine o un oggetto OLE, imageData dovrebbe essere null. |

### Vedi anche

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


