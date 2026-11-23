---
title: "Style.IsFontApplied"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Style 属性。指示是否应应用字体格式"
type: docs
url: /zh/net/aspose.cells/style/isfontapplied/
---
## Style.IsFontApplied property

指示是否应应用字体格式。

```csharp
public bool IsFontApplied { get; set; }
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
    public class StylePropertyIsFontAppliedDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 从工作表访问单元格
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            
            // 获取单元格的样式
            Style style = cell.GetStyle();
            
            // 应用字体设置
            style.Font.Name = "Times New Roman";
            style.Font.Size = 14;
            style.Font.Color = Color.Blue;
            
            // 启用字体应用
            style.IsFontApplied = true;
            
            // 将修改后的样式设置回单元格
            cell.SetStyle(style);
            
            // 保存工作簿
            workbook.Save("FontAppliedDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


