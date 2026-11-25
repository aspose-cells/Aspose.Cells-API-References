---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "LowCodeSaveOptionsProviderOfAssembling property. Indica se aggiungere sempre l'indice della parte divisa al percorso del file. Il valore predefinito è false, cioè quando c'è una sola parte divisa l'indice della parte divisa e il prefisso corrispondente non verranno aggiunti al percorso del file"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways property

Indica se aggiungere sempre l'indice della parte divisa al percorso del file. Il valore predefinito è false, cioè, quando c'è una sola parte divisa, l'indice della parte divisa e il prefisso corrispondente non verranno aggiunti al percorso del file.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### Esempi

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

### Vedi anche

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


