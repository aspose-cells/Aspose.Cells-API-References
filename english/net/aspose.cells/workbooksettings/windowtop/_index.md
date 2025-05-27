---
title: WorkbookSettings.WindowTop
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. The distance from the top edge of the client area to the top edge of the window in unit of point
type: docs
url: /net/aspose.cells/workbooksettings/windowtop/
---
## WorkbookSettings.WindowTop property

The distance from the top edge of the client area to the top edge of the window, in unit of point.

```csharp
public double WindowTop { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Set WindowTop property to position the window 100 pixels from top
            settings.WindowTop = 100;
            
            // Verify the WindowTop value
            Console.WriteLine("Window top position set to: " + settings.WindowTop);

            // Save the workbook
            workbook.Save("WindowTopDemo.xlsx");
        }
    }
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


