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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;
    using System.IO;

    public class UtilityClassConversionUtilityDemo
    {
        public static void Run()
        {
            // Create a sample CSV file for conversion
            string sourceFile = "sample.csv";
            string outputFile = "converted.xlsx";

            try
            {
                // Create sample CSV content
                File.WriteAllText(sourceFile, "Product,Price,Quantity\nApple,1.50,100\nBanana,0.75,150\nOrange,1.25,120");

                // Convert CSV to XLSX using static conversion method
                ConversionUtility.Convert(sourceFile, outputFile);

                Console.WriteLine($"Successfully converted {sourceFile} to {outputFile}");

                // Verify the conversion by checking if output file exists
                if (File.Exists(outputFile))
                {
                    Console.WriteLine("Output file created successfully");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Clean up temporary files
                if (File.Exists(sourceFile))
                {
                    File.Delete(sourceFile);
                }
                if (File.Exists(outputFile))
                {
                    File.Delete(outputFile);
                }
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


