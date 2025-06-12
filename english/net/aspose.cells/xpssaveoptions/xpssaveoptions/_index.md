---
title: XpsSaveOptions.XpsSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: XpsSaveOptions constructor. Creates options for saving xps file
type: docs
url: /net/aspose.cells/xpssaveoptions/xpssaveoptions/
---
## XpsSaveOptions() {#constructor}

Creates options for saving xps file.

```csharp
public XpsSaveOptions()
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XpsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add sample data
            sheet.Cells["A1"].PutValue("XPS Save Options Demo");

            // Initialize XpsSaveOptions using constructor
            XpsSaveOptions saveOptions = new XpsSaveOptions();

            // Configure save options
            saveOptions.OnePagePerSheet = true;
            saveOptions.DefaultFont = "Arial";
            saveOptions.PageIndex = 0;
            saveOptions.PageCount = 1;

            // Save workbook with options
            workbook.Save("XpsSaveOptionsDemo.xps", saveOptions);
        }
    }
}
```

### See Also

* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XpsSaveOptions(SaveFormat) {#constructor_1}

Creates options for saving xps file.

```csharp
[Obsolete("Use XpsSaveOptions() constructor instead.")]
public XpsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The save format, it must be xps format. |

### Remarks

NOTE: This constructor is now obsolete. Instead, please use XpsSaveOptions() constructor. This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XpsSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("XPS SaveOptions Constructor Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates XpsSaveOptions(SaveFormat) constructor");
            
            try
            {
                // Call the constructor with SaveFormat parameter
                XpsSaveOptions options = new XpsSaveOptions(SaveFormat.Xps);
                
                Console.WriteLine("XpsSaveOptions constructor executed successfully with SaveFormat.Xps parameter");
                
                // Save the workbook with XPS options
                workbook.Save("XpsSaveOptionsCtorDemo.xps", options);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XpsSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


