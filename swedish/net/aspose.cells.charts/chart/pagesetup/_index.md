---
title: "Chart.PageSetup"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-egenskap. Representerar sidinställningsbeskrivningen i detta diagram"
type: docs
url: /sv/net/aspose.cells.charts/chart/pagesetup/
---
## Chart.PageSetup property

Representerar sidinställningsbeskrivningen i detta diagram.

```csharp
public PageSetup PageSetup { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett arbetsblad och infoga lite data för diagrammet
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

            // Lägg till ett diagramblad
            int chartSheetIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartSheetIndex];
            chartSheet.Name = "ChartSheet";

            // Lägg till ett diagram i diagrambladet
            int chartIndex = chartSheet.Charts.Add(ChartType.Column, 0, 0, 800, 600);
            Chart chart = chartSheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Kom åt PageSetup för diagrammet
            PageSetup pageSetup = chart.PageSetup;

            // Ställ in sidinställningsegenskaper
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Zoom = 90;
            pageSetup.LeftMargin = 2.0;
            pageSetup.RightMargin = 2.0;
            pageSetup.TopMargin = 2.0;
            pageSetup.BottomMargin = 2.0;

            // Ange sidhuvud med text och bild
            byte[] imageData = File.ReadAllBytes("logo.png");
            pageSetup.SetHeaderPicture(0, imageData);
            pageSetup.SetHeader(0, "&G");
            pageSetup.SetHeader(1, "Sales Report");
            pageSetup.SetHeader(2, "&D");

            // Ange sidfot
            pageSetup.SetFooter(0, "Page &P of &N");

            // Spara arbetsboken
            workbook.Save("ChartPageSetupDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../../../aspose.cells/pagesetup/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


