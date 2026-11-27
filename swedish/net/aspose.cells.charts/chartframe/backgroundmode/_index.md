---
title: "ChartFrame.BackgroundMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Hämtar och anger visningsläget för bakgrunden. Denna egenskap är endast giltig i Excel 2003 eller tidigare versioner."
type: docs
url: /sv/net/aspose.cells.charts/chartframe/backgroundmode/
---
## ChartFrame.BackgroundMode property

Hämtar och anger visningsläget för bakgrunden. Denna egenskap är endast giltig i Excel 2003 eller tidigare versioner.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode BackgroundMode { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ChartFrame.Area.FillFormat.FillType. Till exempel, om du behöver sätta BackgroundMode till Opaque, kan du använda följande kod: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundModeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["B4"].PutValue(20);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagramdata
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstrera egenskapen BackgroundMode
            chart.ChartArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Transparent;
            chart.PlotArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Automatic;

            // Spara arbetsboken
            workbook.Save("ChartBackgroundModeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


