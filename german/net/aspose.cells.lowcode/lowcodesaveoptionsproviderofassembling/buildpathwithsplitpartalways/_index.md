---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfAssembling Eigenschaft. Ob der Index des geteilten Teils immer zum Dateipfad hinzugefügt wird. Standardwert ist false, das heißt, wenn nur ein geteiltes Teil vorhanden ist, wird der Index des geteilten Teils und das entsprechende Präfix nicht zum Dateipfad hinzugefügt."
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways property

Ob der Index des geteilten Teils immer zum Dateipfad hinzugefügt wird. Standardwert ist false, d.h., wenn nur ein geteiltes Teil vorhanden ist, werden der Teil‑Index und das entsprechende Präfix nicht zum Dateipfad hinzugefügt.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### Beispiele

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

### Siehe auch

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


