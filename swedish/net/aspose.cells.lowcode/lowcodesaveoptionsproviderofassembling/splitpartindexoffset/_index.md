---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfAssembling egenskap. Offset för delade del-index mellan vad som används i filsökvägen och dess faktiska värde PartIndex"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset property

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

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartIndexOffsetDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i kalkylbladet för att skapa flera delade delar
            for(int i = 0; i < 150; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Item {i+1}";
            }

            // Konfigurera sidbrytningar för att dela upp i 3 delar
            worksheet.HorizontalPageBreaks.Add(0, 50);
            worksheet.HorizontalPageBreaks.Add(0, 100);

            // Skapa leverantör och konfigurera sparalternativ
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Part_",
                SplitPartPrefix = "-",
                PathTail = ".xlsx",
                SplitPartIndexOffset = 10
            };

            // Visa den initiala konfigurationen
            Console.WriteLine($"Initial SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
            Console.WriteLine("First save operation (offset 10):");
            Console.WriteLine($"Expected filenames: output/Part_-10.xlsx, output/Part_-11.xlsx, output/Part_-12.xlsx");

            // Ändra förskjutning och visa ny konfiguration
            provider.SplitPartIndexOffset = 0;
            Console.WriteLine($"\nModified SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
            Console.WriteLine("Second save operation (offset 0):");
            Console.WriteLine($"Expected filenames: output/Part_-0.xlsx, output/Part_-1.xlsx, output/Part_-2.xlsx");

            // Den faktiska sparåtgärden skulle vanligtvis vara:
            // workbook.Save("output/main.xlsx", new OoxmlSaveOptions { SaveProvider = provider });
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


