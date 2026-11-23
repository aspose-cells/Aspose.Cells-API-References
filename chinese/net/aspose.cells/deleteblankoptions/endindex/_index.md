---
title: "DeleteBlankOptions.EndIndex"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DeleteBlankOptions 属性。指定要检查并删除空行/列的范围的结束行/列索引（包括在内）。默认值为 1，且 1 表示需要检查的所有对象（单元格、图形等）的最大范围……"
type: docs
url: /zh/net/aspose.cells/deleteblankoptions/endindex/
---
## DeleteBlankOptions.EndIndex property

指定要检查并删除空白行/列的范围的结束行/列索引（含）。默认值为 -1，-1 表示需要检查的所有对象（单元格、绘图等）的最大范围。

```csharp
public int EndIndex { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEndIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // 为一些单元格填充值
            cells[0, 2].PutValue(2);
            cells[0, 5].PutValue(5);
            cells[0, 9].PutValue(9);

            // 创建具有特定范围的删除选项
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            dbo.StartIndex = 4;
            dbo.EndIndex = 7;

            // 删除指定范围内的空列
            cells.DeleteBlankColumns(dbo);

            // 输出结果以演示 EndIndex 的效果
            Console.WriteLine("Value at C1: " + cells[0, 2].IntValue);
            Console.WriteLine("Value at F1 (originally G1): " + cells[0, 4].IntValue);
            Console.WriteLine("Value at G1 (originally K1): " + cells[0, 6].IntValue);
        }
    }
}
```

### 另请参见

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


