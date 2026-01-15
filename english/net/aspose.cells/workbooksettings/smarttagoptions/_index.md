---
title: WorkbookSettings.SmartTagOptions
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets the options of the smart tag
type: docs
url: /net/aspose.cells/workbooksettings/smarttagoptions/
---
## WorkbookSettings.SmartTagOptions property

Gets the options of the smart tag.

```csharp
public SmartTagOptions SmartTagOptions { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySmartTagOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();

                // Access the workbook settings
                WorkbookSettings settings = workbook.Settings;

                // Read the SmartTagOptions property
                var smartTagOptions = settings.SmartTagOptions;

                // Display information about the SmartTagOptions instance
                Console.WriteLine("SmartTagOptions instance type: " + smartTagOptions.GetType().FullName);

                // Optionally, you can inspect the default state via ToString()
                Console.WriteLine("SmartTagOptions details: " + smartTagOptions.ToString());

                // Save the workbook (the file will contain default settings)
                workbook.Save("SmartTagOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SmartTagOptions](../../../aspose.cells.markup/smarttagoptions/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


