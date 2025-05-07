---
title: LoadOptions.InterruptMonitor
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets and sets the interrupt monitor
type: docs
url: /net/aspose.cells/loadoptions/interruptmonitor/
---
## LoadOptions.InterruptMonitor property

Gets and sets the interrupt monitor.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Examples

```csharp
// Called: InterruptMonitor = monitor
public static void Property_InterruptMonitor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Create an instance of CustomInterruptMonitor
            CustomInterruptMonitor monitor = new CustomInterruptMonitor();

            // Set load options with the custom interrupt monitor
            LoadOptions loadOptions = new LoadOptions
            {
                InterruptMonitor = monitor
            };

            // Load the workbook with the specified options
            workbook = new Workbook("Sample.xlsx", loadOptions);

            // Perform calculations
            workbook.CalculateFormula();

            // Save the workbook
            workbook.Save("InterruptMonitorDemo.xlsx");
        }
```

### See Also

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


