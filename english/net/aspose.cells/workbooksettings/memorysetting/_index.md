---
title: WorkbookSettings.MemorySetting
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets
type: docs
url: /net/aspose.cells/workbooksettings/memorysetting/
---
## WorkbookSettings.MemorySetting property

Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Examples

```csharp
// Called: settings.MemorySetting = MemorySetting.MemoryPreference;
public static void Property_MemorySetting()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the workbook settings
            WorkbookSettings settings = workbook.Settings;

            // Set the memory usage option to MemoryPreference
            settings.MemorySetting = MemorySetting.MemoryPreference;

            // Create a worksheet and add some data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);

            // Save the workbook
            workbook.Save("MemorySettingExample.xlsx");

            Console.WriteLine("Workbook saved with MemorySetting.MemoryPreference.");
        }
```

### See Also

* enum [MemorySetting](../../memorysetting/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


