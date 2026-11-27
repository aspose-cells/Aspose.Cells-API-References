---
title: "ChartTextFrame.TextDirection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartTextFrame-egenskap. Representerar textens läsriktning"
type: docs
url: /sv/net/aspose.cells.charts/charttextframe/textdirection/
---
## ChartTextFrame.TextDirection property

Representerar textens läsriktning.

```csharp
[Obsolete("Use ChartTextFrame.ReadingOrder property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextDirectionType TextDirection { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartTextFrame.ReadingOrder. Denna egenskap kommer att tas bort 12 månader senare sedan mars 2020. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Konfigurera diagramdata
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Konfigurera datamärkningar
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            
            // Demonstrera egenskapen TextDirection
            dataLabels.TextDirection = TextDirectionType.LeftToRight;

            // Spara arbetsboken
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


