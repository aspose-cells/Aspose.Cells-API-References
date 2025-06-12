---
title: Class SpreadsheetConverter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.SpreadsheetConverter class. Converter for conversion between different spreadsheet file formats such as xls xlsx xlsb spreadsheet ml
type: docs
url: /net/aspose.cells.lowcode/spreadsheetconverter/
---
## SpreadsheetConverter class

Converter for conversion between different spreadsheet file formats, such as xls, xlsx, xlsb, spreadsheet ml...

```csharp
public class SpreadsheetConverter
```

## Methods

| Name | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Converts between different spreadsheet file formats. |
| static [Process](../../aspose.cells.lowcode/spreadsheetconverter/process/#process_1)(string, string) | Converts given template file between spreadsheet file formats. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LowCodeClassSpreadsheetConverterDemo
    {
        public static void Run()
        {
            try
            {
                // Initialize workbook with template file
                Workbook workbook = new Workbook("template.xlsx");
                
                // Save in XLSB format
                workbook.Save("template.xlsb", SaveFormat.Xlsb);
                
                Console.WriteLine("Conversion completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error during conversion: " + ex.Message);
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


