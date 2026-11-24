---
title: "Klasse ConversionUtility"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Utility.ConversionUtility Klasse. Stellt ein Dienstprogramm zum Konvertieren von Dateien in andere Formate dar"
type: docs
url: /de/net/aspose.cells.utility/conversionutility/
---
## ConversionUtility class

Stellt ein Hilfswerkzeug zum Konvertieren von Dateien in andere Formate dar.

```csharp
public class ConversionUtility
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert_1)(string, string) | Konvertiert Excel-Dateien in andere Formate. |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert)(string, LoadOptions, string, SaveOptions) | Konvertiert Excel-Dateien in andere Formate. |

### Beispiele

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
            // Erstelle eine Beispiel‑CSV‑Datei für die Konvertierung
            string sourceFile = "sample.csv";
            string outputFile = "converted.xlsx";

            try
            {
                // Erstelle Beispiel‑CSV‑Inhalt
                File.WriteAllText(sourceFile, "Product,Price,Quantity\nApple,1.50,100\nBanana,0.75,150\nOrange,1.25,120");

                // Konvertiere CSV nach XLSX mit der statischen Konvertierungsmethode
                ConversionUtility.Convert(sourceFile, outputFile);

                Console.WriteLine($"Successfully converted {sourceFile} to {outputFile}");

                // Überprüfe die Konvertierung, indem du prüfst, ob die Ausgabedatei existiert
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
                // Bereinige temporäre Dateien
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

### Siehe auch

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


