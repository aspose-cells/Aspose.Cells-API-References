---
title: "类 DeleteBlankOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.DeleteBlankOptions 类。表示删除空白单元格/行/列的设置"
type: docs
url: /zh/net/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class

表示删除空白单元格/行/列的设置。

```csharp
public class DeleteBlankOptions : DeleteOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [DeleteBlankOptions](deleteblankoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DrawingsAsBlank](../../aspose.cells/deleteblankoptions/drawingsasblank/) { get; set; } | 指示是否将图片、形状、图表等绘图相关对象视为空白。默认值为 true。 |
| [EmptyFormulaValueAsBlank](../../aspose.cells/deleteblankoptions/emptyformulavalueasblank/) { get; set; } | 当单元格为公式且计算结果为 null 或空字符串时，是否将其视为空白。默认值为 false。 |
| [EmptyStringAsBlank](../../aspose.cells/deleteblankoptions/emptystringasblank/) { get; set; } | 指示当单元格的值为空字符串时是否将其视为空白。默认值为 true。 |
| [EndIndex](../../aspose.cells/deleteblankoptions/endindex/) { get; set; } | 指定要检查并删除空白行/列的范围的结束行/列索引（含）。默认值为 -1，-1 表示需要检查的所有对象（单元格、绘图等）的最大范围。 |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | 获取/设置用于跟踪删除导致的更改的监视器。（继承自 [`DeleteOptions`](../deleteoptions/)。） |
| [MergedCellsShrinkType](../../aspose.cells/deleteblankoptions/mergedcellsshrinktype/) { get; set; } | 指示在删除空白行/列时如何处理合并单元格。 |
| [StartIndex](../../aspose.cells/deleteblankoptions/startindex/) { get; set; } | 指定要检查并删除空行/列的范围的起始行/列索引。 |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | 指示是否在其他工作表中更新引用。（继承自[`DeleteOptions`](../deleteoptions/)。） |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteBlankOptionsDemo
    {
        public static void DeleteBlankOptionsExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 用一些数据填充工作表
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // 创建 DeleteBlankOptions 的实例
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true,
                EmptyFormulaValueAsBlank = false,
                UpdateReference = true
            };

            // 根据选项删除空行
            worksheet.Cells.DeleteBlankRows(options);

            // 保存工作簿
            workbook.Save("DeleteBlankOptionsExample.xlsx");
            workbook.Save("DeleteBlankOptionsExample.pdf");
            return;
        }
    }
}
```

### 另请参见

* class [DeleteOptions](../deleteoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


