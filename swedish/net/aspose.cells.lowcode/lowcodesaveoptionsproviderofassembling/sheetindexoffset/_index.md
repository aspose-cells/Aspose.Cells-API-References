---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfAssembling-egenskap. Förskjutning av bladindex mellan vad som används i filsökvägen och dess faktiska värde SheetIndex."
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset property

Förskjutning av bladets index mellan vad som används i filsökvägen och dess faktiska värde ([`SheetIndex`](../../splitpartinfo/sheetindex/)).

```csharp
public int SheetIndexOffset { get; set; }
```

### Anmärkningar

Gäller endast när [`UseSheetName`](../usesheetname/) är false.

### Exempel

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
            // Skapa en ny arbetsbok med flera blad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("Inventory");

            // Initiera sparalternativsleverantör
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Quarter_",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet",
                SheetIndexOffset = 10,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Visa ursprunglig förskjutning
            Console.WriteLine($"Original SheetIndexOffset: {provider.SheetIndexOffset}");

            // Spara med initial förskjutning (blad kommer att numreras 10 och 11)
            workbook.Save("output/with_offset", provider.SaveOptionsTemplate.SaveFormat);

            // Ändra förskjutning och spara igen
            provider.SheetIndexOffset = 100;
            Console.WriteLine($"Modified SheetIndexOffset: {provider.SheetIndexOffset}");
            
            // Spara med ny förskjutning (blad kommer att numreras 100 och 101)
            workbook.Save("output/with_modified_offset", provider.SaveOptionsTemplate.SaveFormat);
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


