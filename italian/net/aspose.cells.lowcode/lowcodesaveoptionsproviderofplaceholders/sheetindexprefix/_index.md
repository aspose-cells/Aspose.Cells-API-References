---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptionsProviderOfPlaceHolders. Prefisso per l'indice del foglio di lavoro"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix property

Prefisso per l'indice del foglio di lavoro.

```csharp
public string SheetIndexPrefix { get; set; }
```

### Osservazioni

Se c'è solo un foglio di lavoro e [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) è false, allora questo prefisso e l'indice del foglio (o nome) non verranno aggiunti al percorso del file risultante.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexPrefixDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con più fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Crea un'istanza di LowCodeSaveOptionsProviderOfPlaceHolders
            string pathTemplate = "output_{sheetindex}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Visualizza e modifica SheetIndexPrefix
            Console.WriteLine("Original SheetIndexPrefix: " + provider.SheetIndexPrefix);
            provider.SheetIndexPrefix = "sheet_";
            Console.WriteLine("Modified SheetIndexPrefix: " + provider.SheetIndexPrefix);

            // Imposta le altre proprietà richieste
            provider.BuildPathWithSheetAlways = true;
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();

            // Dimostra l'effetto di SheetIndexPrefix sui percorsi dei file
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                // Poiché non possiamo creare e popolare SplitPartInfo direttamente,
                // mostreremo semplicemente il modello di denominazione senza di esso
                Console.WriteLine($"Sheet {sheet.Name} would save to: output_{provider.SheetIndexPrefix}{sheet.Index}.xlsx");
            }

            // Salva la cartella di lavoro per dimostrare il modello di denominazione
            workbook.Save("output_sheet_0.xlsx");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


