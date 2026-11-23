---
title: "Row.GetStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Row 方法。获取此行的样式"
type: docs
url: /zh/net/aspose.cells/row/getstyle/
---
## Row.GetStyle method

获取此行的样式。

```csharp
public Style GetStyle()
```

### 备注

直接修改返回的样式对象对该行或该行中的任何单元格没有影响。必须调用 [`ApplyStyle`](../applystyle/) 或 [`SetStyle`](../setstyle/) 方法才能将更改应用于该行。行的样式是将在该行的单元格中继承的样式（那些没有自定义样式设置的单元格，例如未显式设置样式的现有单元格，或尚未实例化的单元格）。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetStyleDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // 设置演示用的样式
            Style rowStyle = workbook.CreateStyle();
            rowStyle.Pattern = BackgroundType.Solid;
            rowStyle.ForegroundColor = System.Drawing.Color.Blue;
            cells.Rows[8].ApplyStyle(rowStyle, new StyleFlag { All = true });

            Style columnStyle = workbook.CreateStyle();
            columnStyle.Pattern = BackgroundType.Solid;
            columnStyle.ForegroundColor = System.Drawing.Color.Red;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { All = true });

            // 演示 GetStyle 的用法
            Style retrievedRowStyle = cells.Rows[8].GetStyle();
            Console.WriteLine("Row 8 Style - ForegroundColor: " + retrievedRowStyle.ForegroundColor);
            Console.WriteLine("Row 8 Style - Pattern: " + retrievedRowStyle.Pattern);

            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style - ForegroundColor: " + retrievedColumnStyle.ForegroundColor);
            Console.WriteLine("Column 5 Style - Pattern: " + retrievedColumnStyle.Pattern);
        }
    }
}
```

### 另请参见

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


