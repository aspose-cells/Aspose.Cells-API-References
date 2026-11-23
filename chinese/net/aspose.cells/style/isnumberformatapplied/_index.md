---
title: "Style.IsNumberFormatApplied"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Style 属性。指示是否应应用数字格式"
type: docs
url: /zh/net/aspose.cells/style/isnumberformatapplied/
---
## Style.IsNumberFormatApplied property

指示是否应应用数字格式。

```csharp
public bool IsNumberFormatApplied { get; set; }
```

### 备注

仅适用于已命名的样式。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsNumberFormatAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 创建带数字格式的样式
            Style style = workbook.CreateStyle();
            style.Number = 14; // Format as "m/d/yyyy"
            style.IsNumberFormatApplied = true;
            
            // 将样式应用于单元格
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // 验证已应用数字格式
            Console.WriteLine("IsNumberFormatApplied: " + style.IsNumberFormatApplied);
            Console.WriteLine("Cell value format: " + cell.GetDisplayStyle().Number);
        }
    }
}
```

### 另请参见

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


