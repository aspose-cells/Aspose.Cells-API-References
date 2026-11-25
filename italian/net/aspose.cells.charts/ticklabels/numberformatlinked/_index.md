---
title: "TickLabels.NumberFormatLinked"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabels. Vero se il formato numerico è collegato alle celle in modo che il formato numerico cambi nelle etichette quando cambia nelle celle"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/numberformatlinked/
---
## TickLabels.NumberFormatLinked property

True se il formato numerico è collegato alle celle (in modo che il formato numerico cambi nelle etichette quando cambia nelle celle).

```csharp
public bool NumberFormatLinked { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatLinkedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["A4"].PutValue(400);
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("A1:A4", true);
            
            // Accedi alle etichette di tick dell'asse dei valori
            Aspose.Cells.Charts.TickLabels tickLabels = chart.ValueAxis.TickLabels;
            
            // Dimostra la proprietà NumberFormatLinked
            Console.WriteLine("NumberFormatLinked (default): " + tickLabels.NumberFormatLinked);
            
            // Modifica la proprietà
            tickLabels.NumberFormatLinked = false;
            Console.WriteLine("NumberFormatLinked after change: " + tickLabels.NumberFormatLinked);
            
            // Salva la cartella di lavoro
            workbook.Save("TickLabelsNumberFormatLinkedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


