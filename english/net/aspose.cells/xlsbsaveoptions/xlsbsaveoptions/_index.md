---
title: XlsbSaveOptions.XlsbSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: XlsbSaveOptions constructor. Creates xlsb file save options
type: docs
url: /net/aspose.cells/xlsbsaveoptions/xlsbsaveoptions/
---
## XlsbSaveOptions() {#constructor}

Creates xlsb file save options.

```csharp
public XlsbSaveOptions()
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Test Value");

            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.ExportAllColumnIndexes = true;

            workbook.Save("output.xlsb", saveOptions);
        }
    }
}
```

### See Also

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsbSaveOptions(SaveFormat) {#constructor_1}

Creates xlsb file save options.

```csharp
[Obsolete("Use XlsbSaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public XlsbSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The save format . It must be xlsb. |

### Remarks

NOTE: This constructor is now obsolete. Instead, please use XlsbSaveOptions() constructor. This property will be removed 12 months later since January 2021. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsbSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Using XlsbSaveOptions";

            try
            {
                // Create XlsbSaveOptions using the constructor with SaveFormat parameter
                XlsbSaveOptions saveOptions = new XlsbSaveOptions(SaveFormat.Xlsb);

                // Set additional properties if needed
                saveOptions.ExportAllColumnIndexes = true;

                // Save the workbook with the specified save options
                workbook.Save("XlsbSaveOptionsDemo.xlsb", saveOptions);

                Console.WriteLine("Workbook saved successfully with XlsbSaveOptions");
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

* enum [SaveFormat](../../saveformat/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


