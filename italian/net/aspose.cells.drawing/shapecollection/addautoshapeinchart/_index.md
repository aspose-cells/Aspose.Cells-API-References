---
title: "ShapeCollection.AddAutoShapeInChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un' AutoShape al grafico"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addautoshapeinchart/
---
## ShapeCollection.AddAutoShapeInChart method

Aggiunge un AutoShape al grafico.

```csharp
public Shape AddAutoShapeInChart(AutoShapeType type, int top, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | AutoShapeType | Tipo di forma automatica. |
| alto | Int32 | Rappresenta lo spostamento verticale della textbox dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| sinistra | Int32 | Rappresenta lo spostamento verticale della textbox dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| altezza | Int32 | Rappresenta l'altezza della textbox, in unità di 1/4000 dell'area del grafico. |
| larghezza | Int32 | Rappresenta la larghezza della textbox, in unità di 1/4000 dell'area del grafico. |

### Valore di ritorno

Restituisce un oggetto shape.

### Osservazioni

Il tipo non può essere Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddAutoShapeInChartWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Chiama il metodo AddAutoShapeInChart per aggiungere una forma a stella al grafico
                Shape shape = chart.Shapes.AddAutoShapeInChart(
                    AutoShapeType.Star16,  // AutoShapeType
                    100,                  // Top position (in pixels)
                    100,                  // Left position (in pixels)
                    200,                  // Height (in pixels)
                    200);                 // Width (in pixels)

                // Imposta le proprietà della forma
                shape.Name = "SampleStar";
                shape.Fill.SolidFill.Color = System.Drawing.Color.Yellow;
                shape.Line.SolidFill.Color = System.Drawing.Color.Red;

                Console.WriteLine("Star shape added successfully to the chart.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAutoShapeInChart method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("ShapeCollectionMethodAddAutoShapeInChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


