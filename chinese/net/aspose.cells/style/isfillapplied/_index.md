---
title: "Style.IsFillApplied"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Style 属性。指示是否应应用填充格式"
type: docs
url: /zh/net/aspose.cells/style/isfillapplied/
---
## Style.IsFillApplied property

指示是否应应用填充格式。

```csharp
public bool IsFillApplied { get; set; }
```

### 备注

仅适用于已命名的样式。

### 示例

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFillAppliedDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 创建样式
            Style style = workbook.CreateStyle();
            
            // 最初，IsFillApplied 应为 false
            Console.WriteLine("IsFillApplied (initial): " + style.IsFillApplied);
            
            // 应用填充设置
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // 设置填充属性后，IsFillApplied 应为 true
            Console.WriteLine("IsFillApplied (after setting fill): " + style.IsFillApplied);
            
            // 将样式应用于单元格
            worksheet.Cells["A1"].SetStyle(style);
            
            // 保存工作簿
            workbook.Save("IsFillAppliedDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


