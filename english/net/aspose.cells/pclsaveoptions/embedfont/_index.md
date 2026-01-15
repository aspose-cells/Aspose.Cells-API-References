---
title: PclSaveOptions.EmbedFont
second_title: Aspose.Cells for .NET API Reference
description: PclSaveOptions property. Indicates whether to embed font into the output Pcl file
type: docs
url: /net/aspose.cells/pclsaveoptions/embedfont/
---
## PclSaveOptions.EmbedFont property

Indicates whether to embed font into the output Pcl file.

```csharp
public bool EmbedFont { get; set; }
```

### Remarks

The default value is true.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsPropertyEmbedFontDemo
    {
        public static void Run()
        {
            // Create a new workbook and add some sample data
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demonstrating EmbedFont property");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            try
            {
                // Create PCL save options
                PclSaveOptions pclOptions = new PclSaveOptions();

                // Read and display the current value of the EmbedFont property
                Console.WriteLine("Current EmbedFont value: " + pclOptions.EmbedFont);

                // (Optional) If the property is writable you could set it, but we only read it here
                // pclOptions.EmbedFont = true;

                // Save the workbook as a PCL file using the options
                workbook.Save("EmbedFontDemo.pcl", pclOptions);

                Console.WriteLine("Workbook saved successfully with EmbedFont demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### See Also

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


