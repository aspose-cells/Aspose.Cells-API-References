---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfPlaceHolders egenskap. Offset för split‑delarnas index mellan vad som används i filsökvägen och dess faktiska valuePartIndex"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset property

Offset för delad del-index mellan vad som används i filsökvägen och dess faktiska värde ([`PartIndex`](../../splitpartinfo/partindex/)).

```csharp
public int SplitPartIndexOffset { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // Skapa mall för lågkods sparalternativ
            LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();
            saveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;

            // Initiera leverantör med sökvägsmall
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/SplitPart_{0}.xlsx");
            provider.SaveOptionsTemplate = saveOptionsTemplate;

            // Visa och ändra SplitPartIndexOffset
            Console.WriteLine("Initial SplitPartIndexOffset: " + provider.SplitPartIndexOffset);
            provider.SplitPartIndexOffset = 1;

            // Spara arbetsbok för att generera split‑delar med justerat index
            workbook.Save("SplitPartIndexOffsetDemo", saveOptionsTemplate.SaveFormat);

            Console.WriteLine("Generated split parts with offset applied.");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


