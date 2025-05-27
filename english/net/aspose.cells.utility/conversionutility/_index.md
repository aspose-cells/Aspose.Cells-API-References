---
title: Class ConversionUtility
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Utility.ConversionUtility class. Represents utility to convert files to other formats
type: docs
url: /net/aspose.cells.utility/conversionutility/
---
## ConversionUtility class

Represents utility to convert files to other formats.

```csharp
public class ConversionUtility
```

## Methods

| Name | Description |
| --- | --- |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert_1)(string, string) | Converts Excel files to other formats. |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert)(string, LoadOptions, string, SaveOptions) | Converts Excel files to other formats. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConversionUtility
    {
        public static void Convert(string sourcePath, string destPath)
        {
            Workbook workbook = new Workbook(sourcePath);
            workbook.Save(destPath, SaveFormat.Pdf);
        }
    }

    public class UtilityClassConversionUtilityDemo
    {
        public static void Run()
        {
            string sourcePath = "example.xlsx";
            string destPath = "example.pdf";
            
            ConversionUtility.Convert(sourcePath, destPath);
            Console.WriteLine("File converted successfully.");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


