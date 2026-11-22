---
title: "ShapeTextAlignment.NumberOfColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تحصل وتضبط عدد أعمدة النص في المستطيل المحيط"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/
---
## ShapeTextAlignment.NumberOfColumns property

يحصل على ويضبط عدد أعمدة النص في المستطيل المحيط.

```csharp
public int NumberOfColumns { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
            
            // تعيين النص للشكل
            shape.Text = "This is sample text\nin multiple columns";
            
            // الوصول إلى محاذاة النص وتعيين عدد الأعمدة
            shape.TextBody.TextAlignment.NumberOfColumns = 2;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحقق من الخاصية
            Console.WriteLine("Number of columns: " + 
                worksheet.Shapes[0].TextBody.TextAlignment.NumberOfColumns);
        }
    }
}
```

### انظر أيضًا

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


