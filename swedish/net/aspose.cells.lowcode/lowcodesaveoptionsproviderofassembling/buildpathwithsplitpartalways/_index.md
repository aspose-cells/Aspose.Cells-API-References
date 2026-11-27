---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfAssembling egenskap. Anger om delad del-index alltid ska läggas till i filsökvägen. Standardvärdet är falskt, vilket innebär att när det bara finns en delad del så läggs inte del-indexet och motsvarande prefix till i filsökvägen."
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways property

Om delningsdelens index alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns en delningsdel, kommer delningsdelens index och motsvarande prefix inte att läggas till i filsökvägen.

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

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyBuildPathWithSplitPartAlwaysDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
            }

            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitData/",
                PathTail = ".xlsx",
                SplitPartPrefix = "Part_",
                SaveOptionsTemplate = new LowCodeSaveOptions()
            };

            Console.WriteLine("Initial BuildPathWithSplitPartAlways: " + provider.BuildPathWithSplitPartAlways);
            workbook.Save("Output1", provider.SaveOptionsTemplate.SaveFormat);

            provider.BuildPathWithSplitPartAlways = true;
            Console.WriteLine("Updated BuildPathWithSplitPartAlways: " + provider.BuildPathWithSplitPartAlways);
            workbook.Save("Output2", provider.SaveOptionsTemplate.SaveFormat);
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


