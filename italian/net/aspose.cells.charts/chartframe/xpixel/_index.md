---
title: "ChartFrame.XPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di Pixel"
type: docs
url: /it/net/aspose.cells.charts/chartframe/xpixel/
---
## ChartFrame.XPixel property

Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di pixel.

```csharp
public virtual int XPixel { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXPixelDemo
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
            
            // Accedi al titolo del grafico (che eredita da ChartFrame)
            chart.Title.Text = "Sample Chart";
            
            // Visualizza la posizione corrente XPixel del titolo
            Console.WriteLine("Current Title XPixel position: " + chart.Title.XPixel);
            
            // Sposta il titolo orizzontalmente modificando XPixel
            chart.Title.XPixel = 200;
            
            // Visualizza la nuova posizione XPixel
            Console.WriteLine("New Title XPixel position: " + chart.Title.XPixel);
            
            // Salva la cartella di lavoro
            workbook.Save("ChartFrameXPixelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


