---
title: "类 SplitPartInfo"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.SplitPartInfo 类。表示多输入/输出中单个输入/输出的信息，例如在将电子表格转换为图像时要渲染的当前页面"
type: docs
url: /zh/net/aspose.cells.lowcode/splitpartinfo/
---
## SplitPartInfo class

表示多个输入/输出中的单个输入/输出信息，例如在将电子表格转换为图像时要渲染的当前页。

```csharp
public class SplitPartInfo
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [PartIndex](../../aspose.cells.lowcode/splitpartinfo/partindex/) { get; } | 当前部分在序列中的索引（从 0 开始）。-1 表示没有多个部分，因此结果为单一。 |
| [SheetIndex](../../aspose.cells.lowcode/splitpartinfo/sheetindex/) { get; } | 当前部分所在工作表的索引。-1 表示只有一个工作表。 |
| [SheetName](../../aspose.cells.lowcode/splitpartinfo/sheetname/) { get; } | 当前部分所在工作表的名称。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassSplitPartInfoDemo
    {
        public static void Run()
        {
            try
            {
                // 创建一个包含多个工作表的工作簿以进行演示
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // 创建 LowCodeLoadOptions 和 LowCodeSplitOptions
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;

                // 创建自定义提供程序以演示 SplitPartInfo 的使用
                splitOptions.SaveOptionsProvider = new CustomSplitOptionsProvider();

                // 处理拆分操作
                SpreadsheetSplitter.Process(splitOptions);

                Console.WriteLine("Split operation completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSplitOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // 演示访问 SplitPartInfo 属性
            Console.WriteLine($"Processing part: Index={partInfo.PartIndex}, SheetIndex={partInfo.SheetIndex}, SheetName={partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


