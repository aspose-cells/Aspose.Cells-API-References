---
title: Enum MemorySetting
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.MemorySetting enum. Memory usage options
type: docs
url: /net/aspose.cells/memorysetting/
---
## MemorySetting enumeration

Memory usage options.

```csharp
public enum MemorySetting
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Normal | `0` | Default option for cells model. |
| MemoryPreference | `1` | Memory performance preferrable. With this option the data will be held in compact format so for common scenarios it may give lower memory cost. However, this option also may degrade R/W performance a bit in some special cases. |

### Examples

```csharp
[C#]

namespace Demos
{
    using Aspose.Cells;
    using System;

    public class MemorySettingDemo
    {
        public static void MemorySettingExample()
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
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


