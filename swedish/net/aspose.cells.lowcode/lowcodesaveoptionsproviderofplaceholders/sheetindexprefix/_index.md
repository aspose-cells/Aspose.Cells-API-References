---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfPlaceHolders-egenskap. Prefix för indexet på kalkylbladet"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix property

Prefix för indexet för kalkylbladet.

```csharp
public string SheetIndexPrefix { get; set; }
```

### Anmärkningar

Om det bara finns ett kalkylblad och [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) är falskt, kommer detta prefix och kalkylbladsindexet (eller namnet) inte att läggas till i den resulterande filsökvägen.

### Exempel

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
            // Skapa en ny arbetsbok med flera kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Skapa en instans av LowCodeSaveOptionsProviderOfPlaceHolders
            string pathTemplate = "output_{sheetindex}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Visa och ändra SheetIndexPrefix
            Console.WriteLine("Original SheetIndexPrefix: " + provider.SheetIndexPrefix);
            provider.SheetIndexPrefix = "sheet_";
            Console.WriteLine("Modified SheetIndexPrefix: " + provider.SheetIndexPrefix);

            // Ställ in andra nödvändiga egenskaper
            provider.BuildPathWithSheetAlways = true;
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();

            // Demonstrera effekten av SheetIndexPrefix på filsökvägar
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                // Eftersom vi inte kan skapa och fylla i SplitPartInfo direkt,
                // vi kommer bara att demonstrera namnmönstret utan det
                Console.WriteLine($"Sheet {sheet.Name} would save to: output_{provider.SheetIndexPrefix}{sheet.Index}.xlsx");
            }

            // Spara arbetsboken för att demonstrera namnmönstret
            workbook.Save("output_sheet_0.xlsx");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


