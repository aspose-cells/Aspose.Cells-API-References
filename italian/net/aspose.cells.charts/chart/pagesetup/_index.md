---
title: "Chart.PageSetup"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Rappresenta la descrizione della configurazione della pagina in questo grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/pagesetup/
---
## Chart.PageSetup property

Rappresenta la descrizione dell'impostazione pagina in questo grafico.

```csharp
public PageSetup PageSetup { get; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPageSetupDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e inserisci alcuni dati per il grafico
            Worksheet dataSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            dataSheet.Name = "DataSheet";
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["B4"].PutValue(30);

            // Aggiungi un foglio di grafico
            int chartSheetIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartSheetIndex];
            chartSheet.Name = "ChartSheet";

            // Aggiungi un grafico al foglio di grafico
            int chartIndex = chartSheet.Charts.Add(ChartType.Column, 0, 0, 800, 600);
            Chart chart = chartSheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Accedi al PageSetup del grafico
            PageSetup pageSetup = chart.PageSetup;

            // Imposta le proprietà di configurazione della pagina
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Zoom = 90;
            pageSetup.LeftMargin = 2.0;
            pageSetup.RightMargin = 2.0;
            pageSetup.TopMargin = 2.0;
            pageSetup.BottomMargin = 2.0;

            // Imposta l'intestazione con testo e immagine
            byte[] imageData = File.ReadAllBytes("logo.png");
            pageSetup.SetHeaderPicture(0, imageData);
            pageSetup.SetHeader(0, "&G");
            pageSetup.SetHeader(1, "Sales Report");
            pageSetup.SetHeader(2, "&D");

            // Imposta il piè di pagina
            pageSetup.SetFooter(0, "Page &P of &N");

            // Salva la cartella di lavoro
            workbook.Save("ChartPageSetupDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../../../aspose.cells/pagesetup/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


