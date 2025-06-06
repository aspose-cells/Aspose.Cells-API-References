---
title: WorkbookSettings.Date1904
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets a value which represents if the workbook uses the 1904 date system
type: docs
url: /net/aspose.cells/workbooksettings/date1904/
---
## WorkbookSettings.Date1904 property

Gets or sets a value which represents if the workbook uses the 1904 date system.

```csharp
public bool Date1904 { get; set; }
```

### Examples

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
            
            // Demonstrate negative time with Date1904
            Style style = cell.GetStyle();
            style.Custom = "h:mm";
            cell.SetStyle(style);
            cell.PutValue(-0.0736111111111112);
            Console.WriteLine("Negative time value: " + cell.DisplayStringValue);

            // Demonstrate negative date with Date1904
            style = cell.GetStyle();
            style.Custom = "mm/dd/yyyy h:mm:ss";
            cell.SetStyle(style);
            cell.PutValue(-42389.47075706);
            Console.WriteLine("Negative date value: " + cell.DisplayStringValue);
        }
    }
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


