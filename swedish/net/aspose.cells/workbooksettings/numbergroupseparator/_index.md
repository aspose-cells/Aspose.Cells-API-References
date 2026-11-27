---
title: "WorkbookSettings.NumberGroupSeparator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Hämtar eller anger tecknet som separerar grupper av siffror till vänster om decimalen i numeriska värden. Standard är gruppseparatorn för aktuell region"
type: docs
url: /sv/net/aspose.cells/workbooksettings/numbergroupseparator/
---
## WorkbookSettings.NumberGroupSeparator property

Hämtar eller anger tecknet som separerar grupper av siffror till vänster om decimalen i numeriska värden. Standard är gruppavgränsaren för aktuell region.

```csharp
public char NumberGroupSeparator { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyNumberGroupSeparatorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            wb.Settings.NumberDecimalSeparator = ',';
            wb.Settings.NumberGroupSeparator = '.';
            
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00";
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(12345.6798);
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


