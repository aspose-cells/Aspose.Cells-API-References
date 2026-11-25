---
title: "Series.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene o imposta il nome della serie di dati"
type: docs
url: /it/net/aspose.cells.charts/series/name/
---
## Series.Name property

Ottiene o imposta il nome della serie di dati.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Series Name");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie al grafico
            chart.NSeries.Add("A2:C2", true);
            
            // Dimostra l'uso della proprietà Name
            // 1. Nome di riferimento a una cella
            chart.NSeries[0].Name = "=A1";
            
            // 2. Imposta una stringa come nome
            chart.NSeries[0].Name = "First Series";
            
            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyNameDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


