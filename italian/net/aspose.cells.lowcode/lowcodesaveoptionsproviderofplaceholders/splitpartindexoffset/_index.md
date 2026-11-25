---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptionsProviderOfPlaceHolders. Scostamento dell'indice delle parti divise tra quello usato nel percorso del file e il suo valore reale valuePartIndex"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset property

Offset dell'indice della parte divisa tra quello usato nel percorso del file e il suo valore reale ([`PartIndex`](../../splitpartinfo/partindex/)).

```csharp
public int SplitPartIndexOffset { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartIndexOffsetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // Crea un modello di opzioni di salvataggio low code
            LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();
            saveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;

            // Inizializza il provider con il modello di percorso
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/SplitPart_{0}.xlsx");
            provider.SaveOptionsTemplate = saveOptionsTemplate;

            // Visualizza e modifica SplitPartIndexOffset
            Console.WriteLine("Initial SplitPartIndexOffset: " + provider.SplitPartIndexOffset);
            provider.SplitPartIndexOffset = 1;

            // Salva la cartella di lavoro per generare parti divise con indice regolato
            workbook.Save("SplitPartIndexOffsetDemo", saveOptionsTemplate.SaveFormat);

            Console.WriteLine("Generated split parts with offset applied.");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


