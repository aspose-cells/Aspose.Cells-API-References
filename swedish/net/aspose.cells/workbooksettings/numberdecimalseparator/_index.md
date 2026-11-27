---
title: "WorkbookSettings.NumberDecimalSeparator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Hämtar eller anger decimalavgränsaren för formatering/parsning av numeriska värden. Standard är decimalavgränsaren för aktuell region"
type: docs
url: /sv/net/aspose.cells/workbooksettings/numberdecimalseparator/
---
## WorkbookSettings.NumberDecimalSeparator property

Hämtar eller anger decimalavgränsaren för formatering/parsning av numeriska värden. Standard är decimalavgränsaren för aktuell region.

```csharp
public char NumberDecimalSeparator { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyNumberDecimalSeparatorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
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


