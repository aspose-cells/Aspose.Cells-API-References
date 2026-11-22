---
title: "Enum FillType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.FillType enum. نوع تنسيق التعبئة"
type: docs
url: /ar/net/aspose.cells.drawing/filltype/
---
## FillType enumeration

نوع تنسيق التعبئة.

```csharp
public enum FillType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Automatic | `0` | يمثل نوع التنسيق التلقائي. |
| None | `1` | يمثل نوع التنسيق لا شيء. |
| Solid | `2` | تنسيق تعبئة صلبة. |
| Gradient | `3` | تنسيق تعبئة متدرج. |
| Texture | `4` | تنسيق تعبئة نسيج (يتضمن تعبئة الصورة). |
| Pattern | `5` | تنسيق تعبئة نمط. |
| Group | `6` | وراثة خصائص التعبئة للمجموعة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 150);
            
            // تعيين نوع تعبئة التدرج
            rectangle.Fill.FillType = FillType.Gradient;
            rectangle.Fill.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            // إضافة مربع نص
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 10, 10, 100, 150);
            textBox.Text = "Gradient Fill Example";
            
            // تعيين نوع تعبئة التدرج لمربع النص
            textBox.Fill.FillType = FillType.Gradient;
            textBox.Fill.SetTwoColorGradient(Color.LightGreen, Color.DarkGreen, GradientStyleType.Vertical, 1);

            // احفظ المصنف
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


