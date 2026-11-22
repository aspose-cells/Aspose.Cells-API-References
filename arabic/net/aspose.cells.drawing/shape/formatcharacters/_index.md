---
title: "Shape.FormatCharacters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. ينسق بعض الأحرف باستخدام إعداد الخط"
type: docs
url: /ar/net/aspose.cells.drawing/shape/formatcharacters/
---
## Shape.FormatCharacters method

يقوم بتنسيق بعض الأحرف باستخدام إعداد الخط.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | Int32 | فهرس البداية. |
| الطول | Int32 | الطول. |
| خط | خط | إعداد الخط. |
| علامة | StyleFlag | علامة إعداد الخط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة مربع نص إلى ورقة العمل
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text Formatting";
            
            // إنشاء خط بالخصائص المطلوبة
            Aspose.Cells.Font font = textBox.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // إنشاء علم نمط لتحديد الخصائص التي سيتم تطبيقها
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            
            // تطبيق التنسيق على أحرف محددة
            textBox.FormatCharacters(0, 6, font, flag);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


