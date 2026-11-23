---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSaveOptionsProviderOfAssembling 属性。拆分部分索引的前缀"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix property

拆分部件索引的前缀。

```csharp
public string SplitPartPrefix { get; set; }
```

### 备注

如果只有一个拆分部分且 [`BuildPathWithSplitPartAlways`](../buildpathwithsplitpartalways/) 为 false，则此前缀和拆分部分索引（0）将不会添加到生成的文件路径中。

### 示例

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
            // 创建包含跨多页数据的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
                worksheet.Cells[$"A{i + 1}"].Value = $"Data Row {i + 1}";

            // 配置页面设置以创建多页
            worksheet.PageSetup.PrintArea = "A1:A30";
            worksheet.PageSetup.FitToPagesTall = 1;

            // 使用拆分配置初始化保存选项提供程序
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitResults/",
                SplitPartPrefix = "OriginalPart_",
                PathTail = ".pdf",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Pdf }
            };

            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");

            // 使用初始前缀保存（将生成 SplitResults/OriginalPart_0.pdf 等）
            workbook.Save("InitialSplit.pdf", new PdfSaveOptions());

            // 修改拆分前缀
            provider.SplitPartPrefix = "ModifiedPart_";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // 使用修改后的前缀保存（将生成 SplitResults/ModifiedPart_0.pdf 等）
            workbook.Save("ModifiedSplit.pdf", new PdfSaveOptions());
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


