---
title: "ShapeCollection.AddShapeInChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge una forma al grafico. Tutte le unità sono 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addshapeinchart/
---
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int, byte[]) {#addshapeinchart_1}

Aggiungi una forma al grafico. Tutta l'unità è 1/4000 dell'area del grafico.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom, byte[] imageData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | MsoDrawingType | Il tipo di disegno. |
| posizionamento | PlacementType | il tipo di posizionamento. |
| sinistra | Int32 | In unità di larghezza dell'area del grafico pari a 1/4000. |
| alto | Int32 | In unità di altezza dell'area del grafico pari a 1/4000. |
| destra | Int32 | In unità di larghezza dell'area del grafico pari a 1/4000. |
| basso | Int32 | In unità di altezza dell'area del grafico pari a 1/4000. |
| imageData | Byte[] | Se la forma non è un'immagine o un oggetto OLE, imageData dovrebbe essere null. |

### Vedi anche

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int) {#addshapeinchart}

Aggiungi una forma al grafico. Tutta l'unità è 1/4000 dell'area del grafico.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | MsoDrawingType | Il tipo di disegno. |
| posizionamento | PlacementType | il tipo di posizionamento. |
| sinistra | Int32 | In unità di larghezza dell'area del grafico pari a 1/4000. |
| alto | Int32 | In unità di altezza dell'area del grafico pari a 1/4000. |
| destra | Int32 | In unità di larghezza dell'area del grafico pari a 1/4000. |
| basso | Int32 | In unità di altezza dell'area del grafico pari a 1/4000. |

### Esempi

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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Aggiungi forma al grafico
            chart.Shapes.AddShapeInChart(MsoDrawingType.CheckBox, PlacementType.Move, 100, 100, 1000, 1000);
            
            // Imposta il testo della forma
            chart.Shapes[0].Text = "Sample CheckBox";
            
            // Salva cartella di lavoro
            workbook.Save("AddShapeInChartWithMsoDrawingType.xlsx");
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


