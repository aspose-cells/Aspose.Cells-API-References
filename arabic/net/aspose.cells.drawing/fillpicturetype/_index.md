---
title: "Enum FillPictureType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.FillPictureType enum. يمثل نوع تعبئة الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/fillpicturetype/
---
## FillPictureType enumeration

يمثل نوع تعبئة الصورة.

```csharp
public enum FillPictureType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Stretch | `0` | تمدد |
| Stack | `1` | تكديس |
| StackAndScale | `2` | StackAndScale |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFillPictureTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل لتوضيح تعبئة الصورة
            Shape shape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 200, 200);

            // تعيين خصائص تعبئة الصورة
            shape.Fill.Type = FillType.Texture;
            shape.Fill.PictureFormatType = FillPictureType.StackAndScale;

            // استخدام صورة بكسل واحد 1x1 (أبيض) للتوضيح
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            shape.Fill.ImageData = Convert.FromBase64String(base64Image);

            // إضافة شكل آخر بنوع تعبئة مختلف
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 5, 2, 0, 200, 200);
            shape2.Fill.Type = FillType.Texture;
            shape2.Fill.PictureFormatType = FillPictureType.Stretch;
            shape2.Fill.ImageData = Convert.FromBase64String(base64Image);

            // حفظ المصنف بتكوينات تعبئة مختلفة
            workbook.Save("FillPictureTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


