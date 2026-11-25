---
title: "Classe ConversionUtility"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Utility.ConversionUtility. Rappresenta un'utilità per convertire file in altri formati"
type: docs
url: /it/net/aspose.cells.utility/conversionutility/
---
## ConversionUtility class

Rappresenta l'utilità per convertire i file in altri formati.

```csharp
public class ConversionUtility
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert_1)(string, string) | Converte file Excel in altri formati. |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert)(string, LoadOptions, string, SaveOptions) | Converte file Excel in altri formati. |

### Esempi

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
            // Crea un file CSV di esempio per la conversione
            string sourceFile = "sample.csv";
            string outputFile = "converted.xlsx";

            try
            {
                // Crea contenuto CSV di esempio
                File.WriteAllText(sourceFile, "Product,Price,Quantity\nApple,1.50,100\nBanana,0.75,150\nOrange,1.25,120");

                // Converti CSV in XLSX usando il metodo di conversione statico
                ConversionUtility.Convert(sourceFile, outputFile);

                Console.WriteLine($"Successfully converted {sourceFile} to {outputFile}");

                // Verifica la conversione controllando se il file di output esiste
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
                // Pulisci i file temporanei
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

### Vedi anche

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


