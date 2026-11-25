---
title: "Classe SplitPartInfo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.LowCode.SplitPartInfo. Rappresenta le informazioni di un input/output per più input/output, come la pagina corrente da renderizzare durante la conversione del foglio di calcolo in immagine"
type: docs
url: /it/net/aspose.cells.lowcode/splitpartinfo/
---
## SplitPartInfo class

Rappresenta le informazioni di un singolo input/output per più input/output, ad esempio la pagina corrente da renderizzare durante la conversione di un foglio di calcolo in immagine.

```csharp
public class SplitPartInfo
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [PartIndex](../../aspose.cells.lowcode/splitpartinfo/partindex/) { get; } | Indice della parte corrente nella sequenza (basata su 0). -1 indica che non ci sono più parti, quindi il risultato è singolo. |
| [SheetIndex](../../aspose.cells.lowcode/splitpartinfo/sheetindex/) { get; } | Indice del foglio in cui si trova la parte corrente. -1 indica che c'è un solo foglio. |
| [SheetName](../../aspose.cells.lowcode/splitpartinfo/sheetname/) { get; } | Nome del foglio in cui si trova la parte corrente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassSplitPartInfoDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una cartella di lavoro con più fogli per la dimostrazione
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Crea LowCodeLoadOptions e LowCodeSplitOptions
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;

                // Crea un provider personalizzato per dimostrare l'uso di SplitPartInfo
                splitOptions.SaveOptionsProvider = new CustomSplitOptionsProvider();

                // Elabora l'operazione di divisione
                SpreadsheetSplitter.Process(splitOptions);

                Console.WriteLine("Split operation completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSplitOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Dimostra l'accesso alle proprietà di SplitPartInfo
            Console.WriteLine($"Processing part: Index={partInfo.PartIndex}, SheetIndex={partInfo.SheetIndex}, SheetName={partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


