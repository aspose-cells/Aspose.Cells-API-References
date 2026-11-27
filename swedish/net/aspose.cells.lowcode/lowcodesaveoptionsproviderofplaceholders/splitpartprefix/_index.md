---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfPlaceHolders-egenskap. Prefix för indexet på uppdelad del"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix property

Prefix för indexet för delningsdelen.

```csharp
public string SplitPartPrefix { get; set; }
```

### Anmärkningar

Om det bara finns en split part och [`BuildPathWithSplitPartAlways`](../buildpathwithsplitpartalways/) är false, kommer detta prefix och split part-indexet (0) inte att läggas till i den resulterande filsökvägen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 25; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Konfigurera mall för sparalternativ
            LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();

            // Initiera leverantören med en platshållare för uppdelad del
            LowCodeSaveOptionsProviderOfPlaceHolders provider = new LowCodeSaveOptionsProviderOfPlaceHolders("SplitResult_Sheet{sheet}_Part{split}.xlsx")
            {
                SaveOptionsTemplate = saveOptionsTemplate
            };

            // Visa och ändra SplitPartPrefix
            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");
            provider.SplitPartPrefix = "Section";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // Spara arbetsbok med uppdelade delar med leverantörens sparformat
            workbook.Save("output", saveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'output' directory for split files with 'Section' prefix");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


