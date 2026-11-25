---
title: "Classe JsonConverter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.JsonConverter. Convertitore per la conversione tra la struttura dati json e altri formati di foglio di calcolo"
type: docs
url: /it/net/aspose.cells.lowcode/jsonconverter/
---
## JsonConverter class

Convertitore per la conversione tra la struttura dati JSON e altri formati di file di foglio di calcolo.

```csharp
public class JsonConverter
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Converte tra dati json e altri formati di foglio di calcolo. |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process_1)(string, string) | Converte il file modello fornito tra json e altri formati. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassJsonConverterDemo
    {
        public static void Run()
        {
            string jsonFilePath = "data.json";
            string excelFilePath = "res.xlsx";

            try
            {
                // Converti JSON in Excel usando Aspose.Cells.LowCode.JsonConverter
                JsonConverter.Process(jsonFilePath, excelFilePath);

                Console.WriteLine("Conversion completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


