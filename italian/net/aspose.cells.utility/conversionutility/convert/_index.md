---
title: "ConversionUtility.Convert"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ConversionUtility. Converte i file Excel in altri formati"
type: docs
url: /it/net/aspose.cells.utility/conversionutility/convert/
---
## Convert(string, string) {#convert_1}

Converte file Excel in altri formati.

```csharp
public static void Convert(string source, string saveAs)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | String | Il nome del file di origine. |
| saveAs | String | Il nome del file previsto. |

### Esempi

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
            // Inizializza i percorsi dei file di origine e destinazione
            string sourcePath = "source.xlsx";
            string destPath = "output.pdf";
            // Converti il file Excel in PDF
            ConversionUtility.Convert(sourcePath, destPath);

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### Vedi anche

* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## Convert(string, LoadOptions, string, SaveOptions) {#convert}

Converte file Excel in altri formati.

```csharp
public static void Convert(string source, LoadOptions loadOptions, string saveAs, 
    SaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | String | Il nome del file di origine. |
| loadOptions | LoadOptions | Le opzioni di caricamento del file di origine. |
| saveAs | String | Il nome del file previsto. |
| saveOptions | SaveOptions | Le opzioni di salvataggio del file. |

### Esempi

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
            // Percorsi dei file di origine e destinazione
            string sourceFile = "input.csv";
            string outputFile = "output.xlsx";

            // Crea un file CSV di esempio per la dimostrazione
            System.IO.File.WriteAllText(sourceFile, "Name,Age\nJohn,30\nAlice,25");

            try
            {
                // Crea opzioni di caricamento per il file CSV
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                
                // Crea opzioni di salvataggio per il file XLSX
                SaveOptions saveOptions = new OoxmlSaveOptions();

                // Converti CSV in XLSX con le opzioni specificate
                ConversionUtility.Convert(sourceFile, loadOptions, outputFile, saveOptions);

                Console.WriteLine($"File converted successfully from {sourceFile} to {outputFile}");
                
                // Verifica la conversione caricando il file di output
                Workbook workbook = new Workbook(outputFile);
                Console.WriteLine($"Output file contains {workbook.Worksheets.Count} worksheet(s)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Pulisci i file temporanei
                if (System.IO.File.Exists(sourceFile))
                {
                    System.IO.File.Delete(sourceFile);
                }
            }
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../../../aspose.cells/loadoptions/)
* class [SaveOptions](../../../aspose.cells/saveoptions/)
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


