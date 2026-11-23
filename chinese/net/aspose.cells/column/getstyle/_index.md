---
title: "Column.GetStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Column 方法。获取此列的样式"
type: docs
url: /zh/net/aspose.cells/column/getstyle/
---
## Column.GetStyle method

获取此列的样式。

```csharp
public Style GetStyle()
```

### 备注

直接修改返回的样式对象对该列或该列中的任何单元格没有影响。必须调用[`ApplyStyle`](../applystyle/) 或 [`SetStyle`](../setstyle/) 方法才能将更改应用于此列。列的样式是将被该列单元格继承的样式（那些没有自定义样式设置的单元格，例如尚未显式设置样式的现有单元格，或尚未实例化的单元格）。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodGetStyleDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // 为第5列设置样式
            Style columnStyle = cells.Columns[5].GetStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 14;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { Font = true });

            // 为第7行设置样式
            Style rowStyle = cells.Rows[7].GetStyle();
            rowStyle.Font.Color = System.Drawing.Color.Red;
            rowStyle.Font.IsItalic = true;
            cells.Rows[7].ApplyStyle(rowStyle, new StyleFlag { Font = true });

            // 验证列样式
            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style:");
            Console.WriteLine($"Font: {retrievedColumnStyle.Font.Name}, Size: {retrievedColumnStyle.Font.Size}, Bold: {retrievedColumnStyle.Font.IsBold}");

            // 验证行样式
            Style retrievedRowStyle = cells.Rows[7].GetStyle();
            Console.WriteLine("\nRow 7 Style:");
            Console.WriteLine($"Color: {retrievedRowStyle.Font.Color}, Italic: {retrievedRowStyle.Font.IsItalic}");

            // 保存工作簿
            workbook.Save("ColumnMethodGetStyleDemo_output.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


