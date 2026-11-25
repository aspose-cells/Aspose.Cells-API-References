---
title: "SplitPartInfo.PartIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SplitPartInfo. Indice della parte corrente basato su indice zero. 1 significa che non ci sono più parti, quindi il risultato è singolo"
type: docs
url: /it/net/aspose.cells.lowcode/splitpartinfo/partindex/
---
## SplitPartInfo.PartIndex property

Indice della parte corrente nella sequenza (basata su 0). -1 indica che non ci sono più parti, quindi il risultato è singolo.

```csharp
public int PartIndex { get; }
```

### Osservazioni

Se è necessario elaborare più fogli e ogni foglio viene elaborato (diviso) separatamente, l'indice della parte inizia sempre da 0 per ogni foglio. Ad esempio, durante la conversione della cartella di lavoro in immagini, rappresenta l'indice della pagina di output del foglio attualmente elaborato. E -1 indica che c'è una sola pagina per il foglio corrente.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertyPartIndexDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una cartella di lavoro con più fogli
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Salva la cartella di lavoro per usarla con l'operazione di divisione
                workbook.Save("sample.xlsx");

                // Crea opzioni di caricamento
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                // Crea opzioni di divisione con provider personalizzato
                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;
                splitOptions.SaveOptionsProvider = new CustomPartIndexProvider();

                // Elabora l'operazione di divisione
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomPartIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Dimostra la lettura della proprietà PartIndex
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Vedi anche

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


