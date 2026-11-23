---
title: "Style.IsAlignmentApplied"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Style 属性。指示是否应应用对齐格式"
type: docs
url: /zh/net/aspose.cells/style/isalignmentapplied/
---
## Style.IsAlignmentApplied property

指示是否应应用对齐格式。

```csharp
public bool IsAlignmentApplied { get; set; }
```

### 备注

仅适用于已命名的样式。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsAlignmentAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            
            // 设置对齐属性
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            
            // 启用对齐应用
            style.IsAlignmentApplied = true;
            
            cell.SetStyle(style);
            
            // 验证已应用对齐
            Console.WriteLine("Alignment applied: " + style.IsAlignmentApplied);
            Console.WriteLine("Horizontal Alignment: " + style.HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + style.VerticalAlignment);
            
            workbook.Save("AlignmentExample.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


