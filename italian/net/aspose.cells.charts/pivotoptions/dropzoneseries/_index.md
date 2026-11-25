---
title: "PivotOptions.DropZoneSeries"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotOptions property. Specifica se un controllo per ogni campo della PivotTable sull'asse della colonna della PivotTable di origine appare sul grafico quando dropZonesVisible è impostato su true"
type: docs
url: /it/net/aspose.cells.charts/pivotoptions/dropzoneseries/
---
## PivotOptions.DropZoneSeries property

Specifica se un controllo per ogni campo della PivotTable sull'asse delle colonne della PivotTable di origine appare sul grafico quando dropZonesVisible è impostato su true.

```csharp
public bool DropZoneSeries { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneSeriesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e ottieni il primo foglio
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(7);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("A1:B4", true);
            
            // Ottieni le opzioni pivot dal grafico
            PivotOptions options = chart.PivotOptions;
            
            // Dimostra la proprietà DropZoneSeries
            Console.WriteLine("Original DropZoneSeries value: " + options.DropZoneSeries);
            options.DropZoneSeries = true;
            Console.WriteLine("Modified DropZoneSeries value: " + options.DropZoneSeries);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotOptionsPropertyDropZoneSeriesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


