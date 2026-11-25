---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptionsProviderOfAssembling. Offset dell'indice dei fogli tra quello usato nel percorso del file e il suo valore reale SheetIndex"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset property

Offset dell'indice del foglio tra quello usato nel percorso del file e il suo valore reale ([`SheetIndex`](../../splitpartinfo/sheetindex/)).

```csharp
public int SheetIndexOffset { get; set; }
```

### Osservazioni

Ha effetto solo quando [`UseSheetName`](../usesheetname/) è false.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetIndexOffsetDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con più fogli
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("Inventory");

            // Inizializza il provider delle opzioni di salvataggio
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Quarter_",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet",
                SheetIndexOffset = 10,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Mostra l'offset originale
            Console.WriteLine($"Original SheetIndexOffset: {provider.SheetIndexOffset}");

            // Salva con l'offset iniziale (i fogli saranno numerati 10 e 11)
            workbook.Save("output/with_offset", provider.SaveOptionsTemplate.SaveFormat);

            // Modifica l'offset e salva di nuovo
            provider.SheetIndexOffset = 100;
            Console.WriteLine($"Modified SheetIndexOffset: {provider.SheetIndexOffset}");
            
            // Salva con il nuovo offset (i fogli saranno numerati 100 e 101)
            workbook.Save("output/with_modified_offset", provider.SaveOptionsTemplate.SaveFormat);
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


