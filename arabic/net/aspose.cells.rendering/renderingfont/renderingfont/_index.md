---
title: "RenderingFont.RenderingFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ RenderingFont. يهيئ مثيلاً جديداً من RenderingFont"
type: docs
url: /ar/net/aspose.cells.rendering/renderingfont/renderingfont/
---
## RenderingFont constructor

يهيئ مثيلاً جديداً من [`RenderingFont`](../)

```csharp
public RenderingFont(string fontName, float fontSize)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fontName | String | اسم الخط |
| fontSize | Single | حجم الخط بالنقاط |

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء خط باستخدام المنشئ #ctor(string, single)
            RenderingFont font = new RenderingFont("Arial", 24f);
            font.Bold = true;
            font.Color = System.Drawing.Color.Red;
            
            // إنشاء نمط وتعيين الخط
            Style style = workbook.CreateStyle();
            style.Font.Name = font.Name;
            style.Font.Size = (int)font.Size;  // Explicit cast from float to int
            style.Font.IsBold = font.Bold;
            style.Font.Color = font.Color;
            
            // تطبيق النمط على cell
            worksheet.Cells["A1"].PutValue("Text with custom font");
            worksheet.Cells["A1"].SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("FontDemoOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


