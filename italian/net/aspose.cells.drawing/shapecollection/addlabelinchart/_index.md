---
title: "ShapeCollection.AddLabelInChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un'etichetta al grafico"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addlabelinchart/
---
## ShapeCollection.AddLabelInChart method

Aggiunge un'etichetta al grafico.

```csharp
public Label AddLabelInChart(int top, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| alto | Int32 | Rappresenta lo spostamento verticale dell'etichetta dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| sinistra | Int32 | Rappresenta lo spostamento verticale dell'etichetta dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| altezza | Int32 | Rappresenta l'altezza dell'etichetta, in unità di 1/4000 dell'area del grafico. |
| larghezza | Int32 | Rappresenta la larghezza dell'etichetta, in unità di 1/4000 dell'area del grafico. |

### Valore di ritorno

Un nuovo oggetto Label.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per creare un grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];            
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Chiama il metodo AddLabelInChart con i parametri (top, left, height, width)
                Label label = chart.Shapes.AddLabelInChart(100, 100, 200, 200);
                
                // Imposta le proprietà dell'etichetta
                label.Text = "Sample Chart Label";
                label.Font.Color = System.Drawing.Color.Red;
                label.Font.Size = 12;

                Console.WriteLine("Label added successfully to chart with parameters (100, 100, 200, 50)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddLabelInChart method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


