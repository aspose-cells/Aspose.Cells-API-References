---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfPlaceHolders-egenskap. Prefix för indexet på kalkylbladet"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix property

Prefix för indexet för kalkylbladet.

```csharp
public string SheetNamePrefix { get; set; }
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

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetNamePrefixDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med två kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "SalesData";
            workbook.Worksheets.Add("FinancialReport");

            // Initiera leverantören med en sökvägsmall som innehåller kalkylbladsplatshållare
            string pathTemplate = "output_{sheet}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Visa initialt SheetNamePrefix-värde (tomt som standard)
            Console.WriteLine("Initial SheetNamePrefix: " + provider.SheetNamePrefix);

            // Ställ in nytt prefix och säkerställ att sökvägsgenereringen inkluderar kalkylbladsinformation
            provider.SheetNamePrefix = "Q4_";
            provider.BuildPathWithSheetAlways = true;

            // Konfigurera sparalternativ med korrekt format
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx // Set the correct save format
            };

            // Spara arbetsbok med leverantören – genererar "output_Q4_SalesData.xlsx" och "output_Q4_FinancialReport.xlsx"
            workbook.Save("result_directory", SaveFormat.Xlsx); // Pass correct SaveFormat
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


