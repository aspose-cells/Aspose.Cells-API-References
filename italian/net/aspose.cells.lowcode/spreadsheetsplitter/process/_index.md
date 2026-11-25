---
title: "SpreadsheetSplitter.Process"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SpreadsheetSplitter. Divide il file modello fornito in più parti"
type: docs
url: /it/net/aspose.cells.lowcode/spreadsheetsplitter/process/
---
## Process(string, string) {#process_1}

Divide il file modello fornito in più parti.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| templateFile | String | Il file modello da dividere |
| resultFile | String | Il file risultante (modello di nome) |

### Osservazioni

I file di output saranno costruiti dal file risultante specificato aggiungendo il numero di sequenza del foglio e della parte divisa. Ad esempio, se il file di output specificato è Split.xlsx, i file generati saranno Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetSplitterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con più fogli di lavoro
            Workbook templateWorkbook = new Workbook();
            Worksheet sheet1 = templateWorkbook.Worksheets.Add("SalesData");
            sheet1.Cells["A1"].PutValue("Product");
            Worksheet sheet2 = templateWorkbook.Worksheets.Add("Inventory");
            sheet2.Cells["A1"].PutValue("test data");

            // Salva come file modello
            string templatePath = "SplitterTemplate.xlsx";
            templateWorkbook.Save(templatePath, SaveFormat.Xlsx);

            // Definisci il modello di output del risultato
            string resultPattern = "SplitResult_";
            
            try
            {
                // Elabora il modello direttamente usando il metodo statico
                SpreadsheetSplitter.Process(templatePath, resultPattern);
                
                Console.WriteLine($"Spreadsheet split successfully using pattern: {resultPattern}");
                Console.WriteLine("Check output directory for split files");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during spreadsheet splitting: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeSplitOptions) {#process}

Divide il file di foglio di calcolo in più parti.

```csharp
public static void Process(LowCodeSplitOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | LowCodeSplitOptions | Opzioni per la divisione del foglio di calcolo |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetSplitterMethodProcessWithLowCodeSplitOptionsDemo
    {
        public static void Run()
        {

            // Inizializza le opzioni di divisione
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions
            {
                LoadOptions = new LowCodeLoadOptions { InputFile = "split.xlsx" },
                SaveOptionsProvider = new CustomLowCodeSaveOptionsProvider()
            };

            try
            {
                // Esegui la divisione del foglio di calcolo usando il metodo statico
                SpreadsheetSplitter.Process(splitOptions);
                
                Console.WriteLine($"Spreadsheet split successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Split operation failed: {ex.Message}");
            }
        }
    }

    // Implementazione concreta di AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        {
            base.Finish(part);
        }
        // Implementa il metodo astratto richiesto
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Vedi anche

* class [LowCodeSplitOptions](../../lowcodesplitoptions/)
* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


