---
title: LoadOptions.MemorySetting
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets or sets the memory usage options
type: docs
url: /net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

Gets or sets the memory usage options.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Examples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Create load options with memory preference setting
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;

            // Load workbook with memory optimized settings
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Access worksheet and add some sample data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Memory Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Save the workbook
            workbook.Save("MemorySettingDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with MemoryPreference setting.");
        }
    }
}
```

### See Also

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


