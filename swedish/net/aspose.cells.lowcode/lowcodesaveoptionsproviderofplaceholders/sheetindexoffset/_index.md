---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfPlaceHolders-egenskap. Offset för kalkylbladsindex mellan vad som används i filsökvägen och dess faktiska valueSheetIndex"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset property

Förskjutning av bladets index mellan vad som används i filsökvägen och dess faktiska värde ([`SheetIndex`](../../splitpartinfo/sheetindex/)).

```csharp
public int SheetIndexOffset { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok med flera blad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Skapa en instans av LowCodeSaveOptionsProviderOfPlaceHolders
            string pathTemplate = "output_{sheet_index}.xlsx";
            var optionsProvider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Visa aktuellt SheetIndexOffset-värde (standard är 0)
            Console.WriteLine("Current SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);

            // Ställ in SheetIndexOffset till 1 för att förskjuta kalkylbladsindex i utdatafilnamn
            optionsProvider.SheetIndexOffset = 1;
            Console.WriteLine("New SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);

            // Konfigurera sparalternativ
            optionsProvider.SaveOptionsTemplate = new LowCodeSaveOptions();
            optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;

            // Demonstrera effekten av SheetIndexOffset på utdatafilnamn
            // Normalt skulle detta användas med GetSaveOptions() under faktiska sparoperationer
            Console.WriteLine("With SheetIndexOffset=1, output files would be named:");
            Console.WriteLine("Sheet1 -> output_1.xlsx (original index 0 + offset 1)");
            Console.WriteLine("Sheet2 -> output_2.xlsx (original index 1 + offset 1)");
            Console.WriteLine("Sheet3 -> output_3.xlsx (original index 2 + offset 1)");

            // Återställ till standardvärde
            optionsProvider.SheetIndexOffset = 0;
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


