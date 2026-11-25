---
title: "ChartFrame.HeightPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene o imposta l'altezza del frame in unità di pixel"
type: docs
url: /it/net/aspose.cells.charts/chartframe/heightpixel/
---
## ChartFrame.HeightPixel property

Ottiene o imposta l'altezza del frame in unità di pixel.

```csharp
public virtual int HeightPixel { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightPixelDemo
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
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accedi al titolo del grafico (che è un ChartFrame)
            ChartFrame chartTitle = chart.Title;
            
            // Visualizza l'altezza corrente in pixel
            Console.WriteLine("Current title height: " + chartTitle.HeightPixel + " pixels");
            
            // Imposta una nuova altezza per il titolo
            chartTitle.HeightPixel = 40;
            Console.WriteLine("New title height: " + chartTitle.HeightPixel + " pixels");
            
            // Accedi alla legenda (un altro ChartFrame)
            ChartFrame legend = chart.Legend;
            
            // Visualizza e modifica l'altezza della legenda
            Console.WriteLine("Current legend height: " + legend.HeightPixel + " pixels");
            legend.HeightPixel = 60;
            Console.WriteLine("New legend height: " + legend.HeightPixel + " pixels");
            
            // Salva la cartella di lavoro
            workbook.Save("ChartFrameHeightPixelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


