---
title: DocxSaveOptions.AsNormalView
second_title: Aspose.Cells for .NET API Reference
description: DocxSaveOptions property. Exporting Excel file to docx fiel as normal view. If this property is true  one Area will be output and no scale will take effect. The default value is false
type: docs
url: /net/aspose.cells/docxsaveoptions/asnormalview/
---
## DocxSaveOptions.AsNormalView property

Exporting Excel file to docx fiel as normal view. If this property is true , one Area will be output, and no scale will take effect. The default value is false.

```csharp
public bool AsNormalView { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsNormalViewDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet and add sample data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Normal View Demo";

            try
            {
                // Initialize DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Display the default value of AsNormalView property
                Console.WriteLine("Default AsNormalView value: " + saveOptions.AsNormalView);

                // Set AsNormalView to true to demonstrate its usage
                saveOptions.AsNormalView = true;
                Console.WriteLine("AsNormalView set to: " + saveOptions.AsNormalView);

                // Save the workbook as DOCX with the configured options
                workbook.Save("AsNormalViewDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsNormalView option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


