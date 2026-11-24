---
title: "Chart.PageSetup"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Stellt die Seiten-Setup-Beschreibung in diesem Diagramm dar"
type: docs
url: /de/net/aspose.cells.charts/chart/pagesetup/
---
## Chart.PageSetup property

Stellt die Seitenlayoutbeschreibung in diesem Diagramm dar.

```csharp
public PageSetup PageSetup { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie ein Arbeitsblatt hinzu und fügen Sie einige Daten für das Diagramm ein
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

            // Fügen Sie ein Diagrammblatt hinzu
            int chartSheetIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartSheetIndex];
            chartSheet.Name = "ChartSheet";

            // Fügen Sie ein Diagramm zum Diagrammblatt hinzu
            int chartIndex = chartSheet.Charts.Add(ChartType.Column, 0, 0, 800, 600);
            Chart chart = chartSheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Greifen Sie auf das PageSetup des Diagramms zu
            PageSetup pageSetup = chart.PageSetup;

            // Seitenlayout-Eigenschaften festlegen
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Zoom = 90;
            pageSetup.LeftMargin = 2.0;
            pageSetup.RightMargin = 2.0;
            pageSetup.TopMargin = 2.0;
            pageSetup.BottomMargin = 2.0;

            // Setzen Sie die Kopfzeile mit Text und Bild
            byte[] imageData = File.ReadAllBytes("logo.png");
            pageSetup.SetHeaderPicture(0, imageData);
            pageSetup.SetHeader(0, "&G");
            pageSetup.SetHeader(1, "Sales Report");
            pageSetup.SetHeader(2, "&D");

            // Setzen Sie die Fußzeile
            pageSetup.SetFooter(0, "Page &P of &N");

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPageSetupDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../../../aspose.cells/pagesetup/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


