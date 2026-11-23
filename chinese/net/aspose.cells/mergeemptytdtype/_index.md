---
title: "枚举 MergeEmptyTdType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.MergeEmptyTdType 枚举。表示在导出文件为 HTML 时空 TD 元素的合并类型"
type: docs
url: /zh/net/aspose.cells/mergeemptytdtype/
---
## MergeEmptyTdType enumeration

表示在导出文件为 HTML 时空 TD 元素的合并类型。

```csharp
public enum MergeEmptyTdType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Default | `0` | 显示效果类似于 MS Excel。 |
| None | `1` | 导出文件为 HTML 时，空的 TD 元素将不会被合并。这会生成显著更大的 HTML 文件。 |
| MergeForcely | `2` | 在导出文件为 HTML 时强制合并空的 TD 元素。将该值设为 true 后，HTML 文件的大小将显著减小。如果希望将 HTML 文件导入 Excel，或在保存为 HTML 时导出完美的网格线，请保持默认值。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MergeEmptyTdTypeDemo
    {
        public static void MergeEmptyTdTypeExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加一些数据
            worksheet.Cells["A1"].PutValue("Data1");
            worksheet.Cells["B1"].PutValue("Data2");
            worksheet.Cells["C1"].PutValue("Data3");

            // 创建 HtmlSaveOptions 并设置 MergeEmptyTdType 属性
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.MergeForcely;

            // 将工作簿保存为 HTML 格式
            workbook.Save("MergeEmptyTdTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with MergeEmptyTdType.MergeForcely option.");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


