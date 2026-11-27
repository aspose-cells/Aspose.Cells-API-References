---
title: "ConversionUtility.Convert"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConversionUtility-metod. Konverterar Excel-filer till andra format"
type: docs
url: /sv/net/aspose.cells.utility/conversionutility/convert/
---
## Convert(string, string) {#convert_1}

Konverterar Excel-filer till andra format.

```csharp
public static void Convert(string source, string saveAs)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | String | Källfilens namn. |
| saveAs | String | Filnamnet på den förväntade filen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ConversionUtilityMethodConvertWithStringStringDemo
    {
        public static void Run()
        {
            // Initiera filvägar för källa och mål
            string sourcePath = "source.xlsx";
            string destPath = "output.pdf";
            // Konvertera Excel-fil till PDF
            ConversionUtility.Convert(sourcePath, destPath);

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### Se även

* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## Convert(string, LoadOptions, string, SaveOptions) {#convert}

Konverterar Excel-filer till andra format.

```csharp
public static void Convert(string source, LoadOptions loadOptions, string saveAs, 
    SaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | String | Källfilens namn. |
| loadOptions | LoadOptions | Alternativen för att läsa in källfilen. |
| saveAs | String | Filnamnet på den förväntade filen. |
| saveOptions | SaveOptions | Alternativen för att spara filen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ConversionUtilityMethodConvertWithStringLoadOptionsStringSaveOptDemo
    {
        public static void Run()
        {
            // Käll- och destinationsfilvägar
            string sourceFile = "input.csv";
            string outputFile = "output.xlsx";

            // Skapa en exempel-CSV-fil för demonstration
            System.IO.File.WriteAllText(sourceFile, "Name,Age\nJohn,30\nAlice,25");

            try
            {
                // Skapa läsalternativ för CSV-fil
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                
                // Skapa sparaalternativ för XLSX-fil
                SaveOptions saveOptions = new OoxmlSaveOptions();

                // Konvertera CSV till XLSX med angivna alternativ
                ConversionUtility.Convert(sourceFile, loadOptions, outputFile, saveOptions);

                Console.WriteLine($"File converted successfully from {sourceFile} to {outputFile}");
                
                // Verifiera konverteringen genom att läsa in utdatafilen
                Workbook workbook = new Workbook(outputFile);
                Console.WriteLine($"Output file contains {workbook.Worksheets.Count} worksheet(s)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Rensa temporära filer
                if (System.IO.File.Exists(sourceFile))
                {
                    System.IO.File.Delete(sourceFile);
                }
            }
        }
    }
}
```

### Se även

* class [LoadOptions](../../../aspose.cells/loadoptions/)
* class [SaveOptions](../../../aspose.cells/saveoptions/)
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


