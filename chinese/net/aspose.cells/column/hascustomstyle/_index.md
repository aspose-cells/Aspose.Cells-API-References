---
title: "Column.HasCustomStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Column 属性。指示此列是否具有不同于从工作簿继承的默认样式的自定义样式设置。"
type: docs
url: /zh/net/aspose.cells/column/hascustomstyle/
---
## Column.HasCustomStyle property

指示此列是否具有自定义样式设置（不同于从工作簿继承的默认样式）。

```csharp
public bool HasCustomStyle { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 访问第一列
            Column column = worksheet.Cells.Columns[0];

            // 显示初始 HasCustomState 值
            Console.WriteLine("Initial HasCustomStyle: " + column.HasCustomStyle);

            // 修改列样式以演示 HasCustomStyle 的更改
            Style columnStyle = column.GetStyle();
            columnStyle.BackgroundColor = Color.LightBlue;
            column.SetStyle(columnStyle);

            // 显示更新后的 HasCustomStyle 值
            Console.WriteLine("After style modification - HasCustomStyle: " + column.HasCustomStyle);

            // 创建另一列，使用默认样式进行比较
            Column secondColumn = worksheet.Cells.Columns[1];
            Console.WriteLine("Second column HasCustomStyle: " + secondColumn.HasCustomStyle);

            // 保存工作簿
            workbook.Save("ColumnHasCustomStyleDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


