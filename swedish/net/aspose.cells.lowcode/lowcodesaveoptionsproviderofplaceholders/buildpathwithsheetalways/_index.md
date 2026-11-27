---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfPlaceHolders egenskap. Anger om bladindex eller namn alltid ska läggas till i filsökvägen. Standardvärdet är falskt, vilket innebär att när det bara finns ett blad så kommer bladindex, namn och motsvarande prefixSheetNamePrefix inte att läggas till i filsökvägen."
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways property

Anger om bladindex eller namn alltid ska läggas till i filsökvägen. Standardvärdet är falskt, vilket innebär att när det bara finns ett blad så kommer bladindex, namn och motsvarande prefix([`SheetNamePrefix`](../sheetnameprefix/)) inte att läggas till i filsökvägen.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok med två blad för att demonstrera sökvägsskillnader
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Konfigurera leverantör med platshållare för bladindex
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_{sheet_index}.xlsx")
            {
                // Demonstrera bladindexoffset (valfritt)
                SheetIndexOffset = 1
            };

            Console.WriteLine($"Initial BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");

            // Spara med bladindex endast när flera blad finns (standardbeteende)
            provider.BuildPathWithSheetAlways = false;
            SaveWithProvider(workbook, provider, "DefaultBehavior");

            // Tvinga bladindex i filnamn även för enskilda blad
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine($"Modified BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");
            SaveWithProvider(workbook, provider, "ForcedSheetIndex");
        }

        private static void SaveWithProvider(Workbook workbook, LowCodeSaveOptionsProviderOfPlaceHolders provider, string saveDescription)
        {
            // Konfigurera sparalternativ med JSON-format för att möjliggöra delning
            var saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Json
            };

            // Konfigurera leverantören med sparalternativen
            provider.SaveOptionsTemplate = saveOptions;

            // Spara med leverantörsbestämda sökvägar
            Console.WriteLine($"Saving with {saveDescription} - check output files");
            workbook.Save($"dummy_{saveDescription}.json", saveOptions.SaveFormat);
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


