---
title: "DataLabels.NumberFormatLinked"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. True se il formato numerico è collegato alle celle in modo che il formato numerico cambi nelle etichette quando cambia nelle celle"
type: docs
url: /it/net/aspose.cells.charts/datalabels/numberformatlinked/
---
## DataLabels.NumberFormatLinked property

True se il formato numerico è collegato alle celle (in modo che il formato numerico cambi nelle etichette quando cambia nelle celle).

```csharp
public bool NumberFormatLinked { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberFormatLinkedDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Formatted Value");
            worksheet.Cells["C2"].PutValue("100 units");
            worksheet.Cells["C3"].PutValue("200 units");

            // Crea un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Configura le etichette dei dati
            var series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.LinkedSource = "C2:C3";
            series.DataLabels.NumberFormatLinked = true; // Link number format from source cells
            
            // Salva la cartella di lavoro
            workbook.Save("DataLabelsNumberFormatLinkedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


