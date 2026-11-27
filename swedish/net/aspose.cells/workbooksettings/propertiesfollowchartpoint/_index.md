---
title: "WorkbookSettings.PropertiesFollowChartPoint"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings‑egenskap. Anger om datapunktsegenskaper och datalabels i alla diagram i denna arbetsbok följer deras referens"
type: docs
url: /sv/net/aspose.cells/workbooksettings/propertiesfollowchartpoint/
---
## WorkbookSettings.PropertiesFollowChartPoint property

Indikerar om datapunkts egenskaper och datamärkningar i alla diagram i denna arbetsbok följer deras referens.

```csharp
public bool PropertiesFollowChartPoint { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPropertiesFollowChartPointDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ställ in PropertiesFollowChartPoint till true
            workbook.Settings.PropertiesFollowChartPoint = true;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Verifiera att inställningen sparades
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("PropertiesFollowChartPoint: " + loadedWorkbook.Settings.PropertiesFollowChartPoint);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


