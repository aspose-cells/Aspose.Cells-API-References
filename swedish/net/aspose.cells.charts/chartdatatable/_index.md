---
title: "Klass ChartDataTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ChartDataTable-klass. Representerar en diagramdatatabell"
type: docs
url: /sv/net/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class

Representerar en diagramdatatabell.

```csharp
public class ChartDataTable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont/) { get; set; } | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant. |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode/) { get; set; } | Hämtar och anger visningsläget för bakgrunden |
| [Border](../../aspose.cells.charts/chartdatatable/border/) { get; } | Returnerar ett Border-objekt som representerar objektets ram |
| [Font](../../aspose.cells.charts/chartdatatable/font/) { get; } | Hämtar ett [`Font`](./font/)-objekt som representerar teckensnittsinställningen för den angivna diagramdatatabellen. |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal/) { get; set; } | (**Obsolete.**) Sant om diagramdatatabellen har horisontella cellramar |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline/) { get; set; } | (**Obsolete.**) Sant om diagramdatatabellen har konturramar |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical/) { get; set; } | (**Obsolete.**) Sant om diagramdatatabellen har vertikala cellramar |
| [HasHorizontalBorder](../../aspose.cells.charts/chartdatatable/hashorizontalborder/) { get; set; } | Sant om diagramdatatabellen har horisontella cellramar |
| [HasOutlineBorder](../../aspose.cells.charts/chartdatatable/hasoutlineborder/) { get; set; } | Sant om diagramdatatabellen har konturramar |
| [HasVerticalBorder](../../aspose.cells.charts/chartdatatable/hasverticalborder/) { get; set; } | Sant om diagramdatatabellen har vertikala cellramar |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey/) { get; set; } | Sant om nyckeln för datalabellegenden är synlig. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDataTableDemo
    {
        public static void ChartDataTableExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Hämtning av referensen till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till exempelvärden i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Lägger till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

            // Åtkomst till instansen av det nyligen tillagda diagrammet
            Chart chart = worksheet.Charts[chartIndex];

            // Lägger till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cellen "A1" till "B3"
            chart.NSeries.Add("A1:B3", true);

            // Visar datatabellen
            chart.ShowDataTable = true;

            // Hämtar diagramdatatabell
            ChartDataTable chartTable = chart.ChartDataTable;

            // Ställer in egenskaper för diagramdatatabell
            chartTable.Font.Color = Color.Red;
            chartTable.AutoScaleFont = true;
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderOutline = true;
            chartTable.ShowLegendKey = false;

            // Sparar Excel-filen
            workbook.Save("ChartDataTableExample.xlsx");
            workbook.Save("ChartDataTableExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


