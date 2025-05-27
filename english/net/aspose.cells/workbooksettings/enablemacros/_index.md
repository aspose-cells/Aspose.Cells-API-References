---
title: WorkbookSettings.EnableMacros
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Enable macros
type: docs
url: /net/aspose.cells/workbooksettings/enablemacros/
---
## WorkbookSettings.EnableMacros property

Enable macros;

```csharp
public bool EnableMacros { get; set; }
```

### Remarks

Now it only works when copying a worksheet to other worksheet in a workbook.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyEnableMacrosDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook wb = new Workbook();
            
            // Access first worksheet
            Worksheet sheet = wb.Worksheets[0];
            
            // Add sample data
            sheet.Cells["A1"].PutValue("Macro Test");
            
            // Demonstrate EnableMacros property
            Console.WriteLine("Initial EnableMacros value: " + wb.Settings.EnableMacros);
            
            // Disable macros
            wb.Settings.EnableMacros = false;
            Console.WriteLine("After disabling macros: " + wb.Settings.EnableMacros);
            
            // Enable macros
            wb.Settings.EnableMacros = true;
            Console.WriteLine("After enabling macros: " + wb.Settings.EnableMacros);
            
            // Save the workbook
            wb.Save("EnableMacrosDemo.xlsx");
        }
    }
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


