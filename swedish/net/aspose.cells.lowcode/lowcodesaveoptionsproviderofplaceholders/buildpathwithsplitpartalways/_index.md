---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfPlaceHolders egenskap. Anger om split‑delens index alltid ska läggas till i filsökvägen. Standardvärdet är falskt, vilket innebär att när det bara finns en split‑del så kommer split‑delens index och motsvarande prefixSplitPartPrefix inte att läggas till i filsökvägen."
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways property

Anger om split‑delens index alltid ska läggas till i filsökvägen. Standardvärdet är falskt, vilket innebär att när det bara finns en split‑del så kommer split‑delens index och motsvarande prefix([`SplitPartPrefix`](../splitpartprefix/)) inte att läggas till i filsökvägen.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSplitPartAlwaysDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok med data som inte kommer att delas upp i flera delar
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Single Part Demonstration";

            // Skapa leverantör med sökvägsmall och delningsvillkor som resulterar i en del
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Result_{split}.xlsx")
            {
                SaveOptionsTemplate = new LowCodeSaveOptions()
            };

            // Demonstrera egenskapens falska tillstånd (standard)
            Console.WriteLine($"Initial BuildPathWithSplitPartAlways: {provider.BuildPathWithSplitPartAlways}");
            provider.BuildPathWithSplitPartAlways = false;
            
            // Detta skulle generera Result.xlsx när endast en del finns
            Console.WriteLine("Saving with BuildPathWithSplitPartAlways=false");
            ExecuteDummySave(workbook, "Result.xlsx");

            // Växla egenskapen och demonstrera sant tillstånd
            provider.BuildPathWithSplitPartAlways = true;
            Console.WriteLine("\nSaving with BuildPathWithSplitPartAlways=true");
            
            // Detta skulle generera Result_0.xlsx även med en enda del
            ExecuteDummySave(workbook, "Result_0.xlsx");
        }

        private static void ExecuteDummySave(Workbook workbook, string filename)
        {
            // I verklig användning, ersätt med en leverantörsbaserad sparoperation
            Console.WriteLine($"Simulated save operation -> Filename: {filename}");
            workbook.Save(filename, SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


