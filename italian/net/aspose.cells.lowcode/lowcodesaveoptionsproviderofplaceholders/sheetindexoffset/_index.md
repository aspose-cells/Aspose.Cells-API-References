---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptionsProviderOfPlaceHolders. Offset dell'indice dei fogli tra quello usato nel percorso file e il suo valore reale SheetIndex"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset property

Offset dell'indice del foglio tra quello usato nel percorso del file e il suo valore reale ([`SheetIndex`](../../splitpartinfo/sheetindex/)).

```csharp
public int SheetIndexOffset { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexOffsetDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con più fogli
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Crea un'istanza di LowCodeSaveOptionsProviderOfPlaceHolders
            string pathTemplate = "output_{sheet_index}.xlsx";
            var optionsProvider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Mostra il valore corrente di SheetIndexOffset (il valore predefinito è 0)
            Console.WriteLine("Current SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);

            // Imposta SheetIndexOffset a 1 per spostare gli indici dei fogli nei nomi dei file di output
            optionsProvider.SheetIndexOffset = 1;
            Console.WriteLine("New SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);

            // Configura le opzioni di salvataggio
            optionsProvider.SaveOptionsTemplate = new LowCodeSaveOptions();
            optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;

            // Dimostra l'effetto di SheetIndexOffset sui nomi dei file di output
            // Normalmente questo verrebbe usato con GetSaveOptions() durante le operazioni di salvataggio effettive
            Console.WriteLine("With SheetIndexOffset=1, output files would be named:");
            Console.WriteLine("Sheet1 -> output_1.xlsx (original index 0 + offset 1)");
            Console.WriteLine("Sheet2 -> output_2.xlsx (original index 1 + offset 1)");
            Console.WriteLine("Sheet3 -> output_3.xlsx (original index 2 + offset 1)");

            // Ripristina al valore predefinito
            optionsProvider.SheetIndexOffset = 0;
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


