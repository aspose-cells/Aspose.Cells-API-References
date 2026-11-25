---
title: "Axis.TickLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Restituisce un oggetto TickLabels che rappresenta le etichette dei segni di graduazione per l'asse specificato"
type: docs
url: /it/net/aspose.cells.charts/axis/ticklabels/
---
## Axis.TickLabels property

Restituisce un oggetto `TickLabels` che rappresenta le etichette dei segni di graduazione per l'asse specificato.

```csharp
public TickLabels TickLabels { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accedi alle etichette di graduazione dell'asse di categoria
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            axis.TickLabels.Font.IsBold = true;
            axis.TickLabels.Font.Color = System.Drawing.Color.Red;
            axis.TickLabels.RotationAngle = 45;
            
            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyTickLabelsDemo_out.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [TickLabels](../../ticklabels/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


