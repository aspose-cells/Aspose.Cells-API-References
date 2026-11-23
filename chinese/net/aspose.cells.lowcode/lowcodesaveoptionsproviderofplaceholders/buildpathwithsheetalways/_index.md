---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSaveOptionsProviderOfPlaceHolders 属性。是否始终将工作表索引或名称添加到文件路径。默认值为 false，即当只有一个工作表时，工作表索引、名称以及相应的前缀SheetNamePrefix 将不会添加到文件路径中。"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways property

是否始终将工作表索引或名称添加到文件路径。默认值为 false，即当只有一个工作表时，工作表索引、名称以及相应的前缀（[`SheetNamePrefix`](../sheetnameprefix/)）将不会添加到文件路径中。

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // 创建包含两个工作表的工作簿以演示路径差异
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // 使用工作表索引占位符配置提供程序
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_{sheet_index}.xlsx")
            {
                // 演示工作表索引偏移（可选）
                SheetIndexOffset = 1
            };

            Console.WriteLine($"Initial BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");

            // 仅在存在多个工作表时使用工作表索引进行保存（默认行为）
            provider.BuildPathWithSheetAlways = false;
            SaveWithProvider(workbook, provider, "DefaultBehavior");

            // 即使只有单个工作表也在文件名中强制包含工作表索引
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine($"Modified BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");
            SaveWithProvider(workbook, provider, "ForcedSheetIndex");
        }

        private static void SaveWithProvider(Workbook workbook, LowCodeSaveOptionsProviderOfPlaceHolders provider, string saveDescription)
        {
            // 使用 JSON 格式配置保存选项以启用拆分
            var saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Json
            };

            // 使用保存选项配置提供程序
            provider.SaveOptionsTemplate = saveOptions;

            // 使用由提供程序决定的路径进行保存
            Console.WriteLine($"Saving with {saveDescription} - check output files");
            workbook.Save($"dummy_{saveDescription}.json", saveOptions.SaveFormat);
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


