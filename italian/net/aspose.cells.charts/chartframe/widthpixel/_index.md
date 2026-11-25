---
title: "ChartFrame.WidthPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene o imposta la larghezza del frame in unità di Pixel"
type: docs
url: /it/net/aspose.cells.charts/chartframe/widthpixel/
---
## ChartFrame.WidthPixel property

Ottiene o imposta la larghezza del frame in unità di pixel.

```csharp
public virtual int WidthPixel { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthPixelDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accedi al titolo del grafico (che eredita da ChartFrame)
            chart.Title.Text = "Sample Chart";
            
            // Visualizza il valore corrente di WidthPixel del titolo del grafico
            Console.WriteLine("Current Title WidthPixel: " + chart.Title.WidthPixel);
            
            // Imposta una nuova larghezza per il titolo del grafico in pixel
            chart.Title.WidthPixel = 300;
            
            // Visualizza il nuovo valore di WidthPixel
            Console.WriteLine("New Title WidthPixel: " + chart.Title.WidthPixel);
            
            // Salva la cartella di lavoro
            workbook.Save("ChartFrameWidthPixelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


