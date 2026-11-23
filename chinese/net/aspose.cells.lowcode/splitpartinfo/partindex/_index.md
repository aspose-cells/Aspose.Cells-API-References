---
title: "SplitPartInfo.PartIndex"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SplitPartInfo 属性。基于从 0 开始的序列中当前部分的索引。1 表示没有多个部分，因此结果为单一。"
type: docs
url: /zh/net/aspose.cells.lowcode/splitpartinfo/partindex/
---
## SplitPartInfo.PartIndex property

当前部分在序列中的索引（从 0 开始）。-1 表示没有多个部分，因此结果为单一。

```csharp
public int PartIndex { get; }
```

### 备注

如果需要处理多个工作表，并且每个工作表单独进行处理（拆分），则每个工作表的部分索引始终从 0 开始。例如，在将工作簿转换为图像时，它表示当前处理的工作表的输出页索引。-1 表示当前工作表只有一页。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertyPartIndexDemo
    {
        public static void Run()
        {
            try
            {
                // 创建包含多个工作表的工作簿
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // 保存工作簿以用于拆分操作
                workbook.Save("sample.xlsx");

                // 创建加载选项
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                // 使用自定义提供程序创建拆分选项
                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;
                splitOptions.SaveOptionsProvider = new CustomPartIndexProvider();

                // 处理拆分操作
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomPartIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // 演示读取 PartIndex 属性
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### 另请参见

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


