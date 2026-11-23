---
title: "Cell.HasCustomStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "单元格属性。指示此单元格是否具有不同于相应行、列或工作簿继承的默认设置的自定义样式"
type: docs
url: /zh/net/aspose.cells/cell/hascustomstyle/
---
## Cell.HasCustomStyle property

指示此单元格是否具有自定义样式设置（不同于相应行、列或工作簿继承的默认设置）。

```csharp
public bool HasCustomStyle { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // 创建一个新工作簿并访问第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Check HasCustomStyle");

            // 显示初始 HasCustomState 值（继承默认样式）
            Console.WriteLine("Initial HasCustomStyle: " + cell.HasCustomStyle);

            // 创建自定义样式并将其应用于单元格
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.IsBold = true;
            cell.SetStyle(customStyle);

            // 验证在样式修改后 HasCustomStyle 为 true
            Console.WriteLine("After applying custom style - HasCustomStyle: " + cell.HasCustomStyle);

            // 保存已应用自定义样式的工作簿
            workbook.Save("CellCustomStyleDemo.xlsx");

            // 将单元格的样式重置为工作簿的默认样式
            Style defaultStyle = workbook.DefaultStyle;
            cell.SetStyle(defaultStyle);

            // 验证恢复默认后 HasCustomStyle 为 false
            Console.WriteLine("After resetting to default style - HasCustomStyle: " + cell.HasCustomStyle);
        }
    }
}
```

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


