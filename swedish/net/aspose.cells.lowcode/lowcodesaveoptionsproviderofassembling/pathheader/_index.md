---
title: "LowCodeSaveOptionsProviderOfAssembling.PathHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfAssembling egenskap. Header-del som läggs till innan bladets innehåll och den delade delen av filsökvägen"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/
---
## LowCodeSaveOptionsProviderOfAssembling.PathHeader property

Headerdel (innan tillagt innehåll från blad och delningsdel) av filsökvägen.

```csharp
public string PathHeader { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathHeaderDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med data som kommer att delas upp i flera delar
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 150; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Initiera sparalternativleverantör med standardvärden
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/QuarterlyReport_",
                PathTail = ".html",
                UseSheetName = true,
                SaveOptionsTemplate = new LowCodeSaveOptions() // Changed from HtmlSaveOptions to LowCodeSaveOptions
            };

            Console.WriteLine($"Initial PathHeader: {provider.PathHeader}");

            // Ändra sökvägskonfiguration
            provider.PathHeader = "output/ModifiedReport_";
            provider.SheetPrefix = "Sheet_";
            provider.SplitPartPrefix = "Part_";

            // Visa effekten genom att spara med den aktuella leverantörskonfigurationen
            workbook.Save("result.html", SaveFormat.Html); // Changed second parameter to SaveFormat.Html

            Console.WriteLine("Check 'output' directory for split files named like 'ModifiedReport_Sheet_0_Part_0.html'");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


