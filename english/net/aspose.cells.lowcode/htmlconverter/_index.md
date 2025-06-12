---
title: Class HtmlConverter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.HtmlConverter class. Converter for conversion between html fileshtml or mht and other spreadsheet file formats
type: docs
url: /net/aspose.cells.lowcode/htmlconverter/
---
## HtmlConverter class

Converter for conversion between html files(html or mht) and other spreadsheet file formats.

```csharp
public class HtmlConverter
```

## Methods

| Name | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/htmlconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Converts file between html and other spreadsheet file formats. |
| static [Process](../../aspose.cells.lowcode/htmlconverter/process/#process_1)(string, string) | Converts given template file between html and other formats. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LowCodeClassHtmlConverterDemo
    {
        public static void Run()
        {
            // Initialize workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(699.99);

            // Save as HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            workbook.Save("res.html", options);
            
            Console.WriteLine("HTML conversion completed successfully.");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


