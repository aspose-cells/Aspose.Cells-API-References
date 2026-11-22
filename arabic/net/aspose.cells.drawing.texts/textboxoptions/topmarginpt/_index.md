---
title: "TextBoxOptions.TopMarginPt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxOptions. تحصل وتعيّن الهامش العلوي بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textboxoptions/topmarginpt/
---
## TextBoxOptions.TopMarginPt property

يحصل ويضبط الهامش العلوي بوحدة نقاط.

```csharp
public double TopMarginPt { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة مربع نص إلى ورقة العمل
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // حدد الهامش العلوي بالنقاط
            textBox.TextBoxOptions.TopMarginPt = 0.2d;
            
            // احفظ المصنف
            workbook.Save("TextBoxTopMarginDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


