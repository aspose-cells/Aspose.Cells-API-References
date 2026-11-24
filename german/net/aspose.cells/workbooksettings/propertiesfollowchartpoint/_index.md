---
title: "WorkbookSettings.PropertiesFollowChartPoint"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob Datenpunkt‑Eigenschaften und Datenbeschriftungen in allen Diagrammen dieser Arbeitsmappe ihrer Referenz folgen"
type: docs
url: /de/net/aspose.cells/workbooksettings/propertiesfollowchartpoint/
---
## WorkbookSettings.PropertiesFollowChartPoint property

Gibt an, ob Datenpunkt-Eigenschaften und Datenbeschriftungen in allen Diagrammen dieser Arbeitsmappe ihrer Referenz folgen.

```csharp
public bool PropertiesFollowChartPoint { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Setzen Sie PropertiesFollowChartPoint auf true
            workbook.Settings.PropertiesFollowChartPoint = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Überprüfen Sie, ob die Einstellung gespeichert wurde
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("PropertiesFollowChartPoint: " + loadedWorkbook.Settings.PropertiesFollowChartPoint);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


