---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSaveOptionsProviderOfAssembling 属性。文件路径中使用的拆分部分索引与其实际值 PartIndex 之间的偏移量"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset property

文件路径中使用的拆分部分索引与其实际值（[`PartIndex`](../../splitpartinfo/partindex/)）之间的偏移量。

```csharp
public int SplitPartIndexOffset { get; set; }
```

### 示例

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
            // 创建包含测试数据的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 填充工作表以创建多个拆分部分
            for(int i = 0; i < 150; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Item {i+1}";
            }

            // 配置分页符以拆分为 3 部分
            worksheet.HorizontalPageBreaks.Add(0, 50);
            worksheet.HorizontalPageBreaks.Add(0, 100);

            // 创建提供程序并配置保存选项
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Part_",
                SplitPartPrefix = "-",
                PathTail = ".xlsx",
                SplitPartIndexOffset = 10
            };

            // 显示初始配置
            Console.WriteLine($"Initial SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
            Console.WriteLine("First save operation (offset 10):");
            Console.WriteLine($"Expected filenames: output/Part_-10.xlsx, output/Part_-11.xlsx, output/Part_-12.xlsx");

            // 更改偏移量并显示新配置
            provider.SplitPartIndexOffset = 0;
            Console.WriteLine($"\nModified SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
            Console.WriteLine("Second save operation (offset 0):");
            Console.WriteLine($"Expected filenames: output/Part_-0.xlsx, output/Part_-1.xlsx, output/Part_-2.xlsx");

            // 实际的保存操作通常是：
            // workbook.Save("output/main.xlsx", new OoxmlSaveOptions { SaveProvider = provider });
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


