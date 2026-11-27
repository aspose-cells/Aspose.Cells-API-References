---
title: "Klass ConversionUtility"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Utility.ConversionUtility-klass. Representerar ett verktyg för att konvertera filer till andra format."
type: docs
url: /sv/net/aspose.cells.utility/conversionutility/
---
## ConversionUtility class

Representerar verktyg för att konvertera filer till andra format.

```csharp
public class ConversionUtility
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert_1)(string, string) | Konverterar Excel-filer till andra format. |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert)(string, LoadOptions, string, SaveOptions) | Konverterar Excel-filer till andra format. |

### Exempel

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
            // Skapa en exempel-CSV-fil för konvertering
            string sourceFile = "sample.csv";
            string outputFile = "converted.xlsx";

            try
            {
                // Skapa exempel-CSV-innehåll
                File.WriteAllText(sourceFile, "Product,Price,Quantity\nApple,1.50,100\nBanana,0.75,150\nOrange,1.25,120");

                // Konvertera CSV till XLSX med statisk konverteringsmetod
                ConversionUtility.Convert(sourceFile, outputFile);

                Console.WriteLine($"Successfully converted {sourceFile} to {outputFile}");

                // Verifiera konverteringen genom att kontrollera om utdatafilen finns
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
                // Rensa temporära filer
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

### Se även

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


