---
title: "ChartFrame.Background"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Hämtar och anger visningsläget för bakgrunden. Denna egenskap är endast giltig i Excel 2003 eller tidigare versioner."
type: docs
url: /sv/net/aspose.cells.charts/chartframe/background/
---
## ChartFrame.Background property

Hämtar och anger visningsläget för bakgrunden. Denna egenskap är endast giltig i Excel 2003 eller tidigare versioner.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.Area.FillFormat.FillType. Till exempel, om du behöver sätta BackgroundMode till Opaque, kan du använda följande kod: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Denna egenskap kommer att tas bort 12 månader senare från JANUARY 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundDemo
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

            // Konfigurera dataetiketter med bakgrundsinställningar
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Background = BackgroundMode.Transparent;

            // Spara arbetsboken
            workbook.Save("ChartBackgroundDemo.xlsx");
        }
    }
}
```

### Se även

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


