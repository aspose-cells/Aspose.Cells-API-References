---
title: "Row.HasCustomStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Row 属性。指示此行是否具有不同于工作簿继承的默认样式的自定义样式设置"
type: docs
url: /zh/net/aspose.cells/row/hascustomstyle/
---
## Row.HasCustomStyle property

指示此行是否具有自定义样式设置（不同于工作簿继承的默认样式）。

```csharp
public bool HasCustomStyle { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 创建并自定义样式
            Style customStyle = workbook.CreateStyle();
            customStyle.BackgroundColor = Color.LightBlue;
            customStyle.Pattern = BackgroundType.Solid;
            
            // 访问第一行
            Row row = worksheet.Cells.Rows[0];
            
            // 对该行应用自定义样式
            row.ApplyStyle(customStyle, new StyleFlag { All = true });
            
            // 检查行是否具有自定义样式（应为 true）
            bool hasCustomStyle = row.HasCustomStyle;
            Console.WriteLine("Row has custom style: " + hasCustomStyle);
            
            // 保存工作簿
            workbook.Save("RowHasCustomStyleDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


