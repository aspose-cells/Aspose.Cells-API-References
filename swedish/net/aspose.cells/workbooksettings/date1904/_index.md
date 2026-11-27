---
title: "WorkbookSettings.Date1904"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Hämtar eller anger ett värde som representerar om arbetsboken använder 1904-datumsystemet"
type: docs
url: /sv/net/aspose.cells/workbooksettings/date1904/
---
## WorkbookSettings.Date1904 property

Hämtar eller anger ett värde som visar om arbetsboken använder 1904-datersystemet.

```csharp
public bool Date1904 { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDate1904Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Date1904 = true;

            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells[0, 0];
            
            // Demonstrera negativ tid med Date1904
            Style style = cell.GetStyle();
            style.Custom = "h:mm";
            cell.SetStyle(style);
            cell.PutValue(-0.0736111111111112);
            Console.WriteLine("Negative time value: " + cell.DisplayStringValue);

            // Demonstrera negativt datum med Date1904
            style = cell.GetStyle();
            style.Custom = "mm/dd/yyyy h:mm:ss";
            cell.SetStyle(style);
            cell.PutValue(-42389.47075706);
            Console.WriteLine("Negative date value: " + cell.DisplayStringValue);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


