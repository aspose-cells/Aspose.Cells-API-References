---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetPrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfAssembling egenskap. Prefix för indexet av kalkylbladet"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetPrefix property

Prefix för indexet för kalkylbladet.

```csharp
public string SheetPrefix { get; set; }
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

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetPrefixDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
            provider.PathHeader = "output/";
            provider.PathTail = ".xlsx";
            provider.UseSheetName = false;

            Console.WriteLine("Current SheetPrefix: " + provider.SheetPrefix);
            
            provider.SheetPrefix = "Report_";
            Console.WriteLine("New SheetPrefix: " + provider.SheetPrefix);

            for (int sheetIndex = 0; sheetIndex < workbook.Worksheets.Count; sheetIndex++)
            {
                string fileName = $"{provider.PathHeader}{provider.SheetPrefix}{sheetIndex}{provider.PathTail}";
                Console.WriteLine($"Generated file path: {fileName}");
            }

            provider.SheetPrefix = "Data_";
            Console.WriteLine("Updated SheetPrefix: " + provider.SheetPrefix);

            for (int sheetIndex = 0; sheetIndex < workbook.Worksheets.Count; sheetIndex++)
            {
                string fileName = $"{provider.PathHeader}{provider.SheetPrefix}{sheetIndex}{provider.PathTail}";
                Console.WriteLine($"Generated file path: {fileName}");
            }
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


