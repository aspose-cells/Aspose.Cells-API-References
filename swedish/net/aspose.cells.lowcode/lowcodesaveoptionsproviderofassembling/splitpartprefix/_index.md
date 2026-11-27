---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfAssembling-egenskap. Prefix för indexet för split part."
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix property

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
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok med data som sträcker sig över flera sidor
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
                worksheet.Cells[$"A{i + 1}"].Value = $"Data Row {i + 1}";

            // Konfigurera sidinställningar för att skapa flera sidor
            worksheet.PageSetup.PrintArea = "A1:A30";
            worksheet.PageSetup.FitToPagesTall = 1;

            // Initiera sparaalternativleverantör med split-konfiguration
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitResults/",
                SplitPartPrefix = "OriginalPart_",
                PathTail = ".pdf",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Pdf }
            };

            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");

            // Spara med initialt prefix (kommer att generera SplitResults/OriginalPart_0.pdf osv.)
            workbook.Save("InitialSplit.pdf", new PdfSaveOptions());

            // Ändra split-prefix
            provider.SplitPartPrefix = "ModifiedPart_";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // Spara med modifierat prefix (kommer att generera SplitResults/ModifiedPart_0.pdf osv.)
            workbook.Save("ModifiedSplit.pdf", new PdfSaveOptions());
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


