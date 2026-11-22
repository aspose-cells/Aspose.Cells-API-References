---
title: "Shape.Characters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تُرجع كائن Characters يمثل نطاقًا من الأحرف داخل النص"
type: docs
url: /ar/net/aspose.cells.drawing/shape/characters/
---
## Shape.Characters method

يرجع كائن Characters الذي يمثل نطاقًا من الأحرف داخل النص.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | Int32 | فهرس بداية الحرف. |
| الطول | Int32 | عدد الأحرف. |

### قيمة الإرجاع

كائن الأحرف.

### ملاحظات

هذه الطريقة تعمل فقط على الشكل الذي لديه عنوان.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً بنص
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "Sample Text";

            // احصل على الأحرف من الفهرس 0 بطول 4
            FontSetting fontSetting = shape.Characters(0, 4);
            
            // عدّل إعدادات الخط
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.Size = 14;
            fontSetting.Font.IsBold = true;

            // احفظ المصنف
            workbook.Save("ShapeCharactersDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


