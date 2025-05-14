---
title: WorkbookSettings.WarningCallback
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets warning callback
type: docs
url: /net/aspose.cells/workbooksettings/warningcallback/
---
## WorkbookSettings.WarningCallback property

Gets or sets warning callback.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.WarningCallback = new IWarningCallbackDemo();
public static void WorkbookSettings_Property_WarningCallback()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Set the warning callback
            workbook.Settings.WarningCallback = new IWarningCallbackDemo();

            // Load a workbook with potential warnings
            try
            {
                workbook = new Workbook("example.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }

            // Save the workbook
            workbook.Save("IWarningCallbackExample.xlsx");
        }
```

### See Also

* interface [IWarningCallback](../../iwarningcallback/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


