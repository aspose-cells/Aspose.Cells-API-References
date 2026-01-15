---
title: Class FontFileDataInfo
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FontFileDataInfo class. Represents data information of font file data
type: docs
url: /net/aspose.cells/fontfiledatainfo/
---
## FontFileDataInfo class

Represents data information of font file data.

```csharp
public class FontFileDataInfo
```

## Properties

| Name | Description |
| --- | --- |
| [Data](../../aspose.cells/fontfiledatainfo/data/) { get; } | Gets binary data of font file. |
| [FormatType](../../aspose.cells/fontfiledatainfo/formattype/) { get; } | Gets font format type of font file. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassFontFileDataInfoDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Example: Loading font file data
            string fontFilePath = "arial.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Note: FontFileDataInfo cannot be directly instantiated as it has no public constructor
            // and its properties are read-only. In a real scenario, you would get an instance
            // from another API method (like FontConfigs.GetFontFileDataInfo())
            FontFileDataInfo fontInfo = null; // Would be populated by API call in real scenario

            // Demonstrate how properties would be used if we had an instance
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
                Console.WriteLine("Font data length: " + (fontInfo.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            }

            // Demonstrate integration with Workbook
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Save the workbook
            workbook.Save("FontFileDataInfoDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


