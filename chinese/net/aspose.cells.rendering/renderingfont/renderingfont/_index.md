---
title: "RenderingFont.RenderingFont"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingFont 构造函数。初始化 RenderingFont 的新实例"
type: docs
url: /zh/net/aspose.cells.rendering/renderingfont/renderingfont/
---
## RenderingFont constructor

初始化一个新的 [`RenderingFont`](../) 实例

```csharp
public RenderingFont(string fontName, float fontSize)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontName | String | 字体名称 |
| fontSize | Single | 以点为单位的字体大小 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontMethodCtorWithStringSingleDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 使用 #ctor(string, single) 构造函数创建字体
            RenderingFont font = new RenderingFont("Arial", 24f);
            font.Bold = true;
            font.Color = System.Drawing.Color.Red;
            
            // 创建样式并设置字体
            Style style = workbook.CreateStyle();
            style.Font.Name = font.Name;
            style.Font.Size = (int)font.Size;  // Explicit cast from float to int
            style.Font.IsBold = font.Bold;
            style.Font.Color = font.Color;
            
            // 将样式应用于单元格
            worksheet.Cells["A1"].PutValue("Text with custom font");
            worksheet.Cells["A1"].SetStyle(style);
            
            // 保存工作簿
            workbook.Save("FontDemoOutput.xlsx");
        }
    }
}
```

### 另请参见

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


