---
title: "Column.SetStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Column 方法。设置此列的样式"
type: docs
url: /zh/net/aspose.cells/column/setstyle/
---
## Column.SetStyle method

设置此列的样式。

```csharp
public void SetStyle(Style style)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 样式 | 样式 | 用于此列中单元格的默认样式。 |

### 备注

此方法仅将给定的样式设置为此列的默认样式，而不更改此列中已有单元格的样式设置。若要同时将已有单元格的样式更新为指定样式，请使用[`ApplyStyle`](../applystyle/)

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnMethodSetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 访问第一列
            Column column = worksheet.Cells.Columns[0];

            // 从工作簿创建新样式
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            try
            {
                // 将自定义样式应用于整列
                column.SetStyle(style);
                
                Console.WriteLine($"Style applied successfully to column {column.Index}");
                Console.WriteLine($"Font: {style.Font.Name}, Size: {style.Font.Size}, Bold: {style.Font.IsBold}");
                Console.WriteLine($"Background: {style.ForegroundColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStyle method: {ex.Message}");
            }

            // 保存已修改的工作簿
            workbook.Save("ColumnMethodSetStyleDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


