---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways"
second_title: "Справочник API Aspose.Cells для .NET"
description: "LowCodeSaveOptionsProviderOfAssembling свойство. Добавлять ли индекс разделённой части к пути к файлу всегда. Значение по умолчанию — false, то есть когда существует только одна разделённая часть, индекс разделённой части и соответствующий префикс не будут добавлены к пути к файлу"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways property

Добавлять ли всегда индекс части разделения в путь файла. Значение по умолчанию — false, то есть когда часть разделения одна, её индекс и соответствующий префикс не будут добавлены в путь файла.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### Примеры

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

### См. также

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


