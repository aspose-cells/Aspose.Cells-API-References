---
title: "Style.IsBorderApplied"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Style 属性。指示是否应应用边框格式"
type: docs
url: /zh/net/aspose.cells/style/isborderapplied/
---
## Style.IsBorderApplied property

指示是否应应用边框格式。

```csharp
public bool IsBorderApplied { get; set; }
```

### 备注

仅适用于已命名的样式。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsBorderAppliedDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 创建自定义样式
            Style style = workbook.CreateStyle();
            
            // 将边框设置应用于样式
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Black;
            
            // 检查是否已应用边框
            Console.WriteLine("IsBorderApplied before setting: " + style.IsBorderApplied);
            
            // 显式将 IsBorderApplied 设置为 true
            style.IsBorderApplied = true;
            
            // 将样式应用于单元格
            worksheet.Cells["A1"].SetStyle(style);
            
            // 验证边框应用
            Console.WriteLine("IsBorderApplied after setting: " + style.IsBorderApplied);
            
            // 保存工作簿
            workbook.Save("IsBorderAppliedDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


