---
title: "ShapeCollection.AddFreeFloatingShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. يضيف شكلاً عائمًا إلى ورقة العمل. ينطبق فقط على شكل خط/صورة"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addfreefloatingshape/
---
## ShapeCollection.AddFreeFloatingShape method

يضيف شكلاً عائمًا حرًا إلى ورقة العمل. ينطبق فقط على شكل الخط/الصورة.

```csharp
public Shape AddFreeFloatingShape(MsoDrawingType type, int top, int left, int height, int width, 
    byte[] imageData, bool isOriginalSize)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | MsoDrawingType | نوع الشكل. |
| أعلى | Int32 | يمثل الإزاحة العمودية للشكل من الصف العلوي لورقة العمل، بوحدة البكسل. |
| يسار | Int32 | يمثل الإزاحة الأفقية للشكل من العمود الأيسر لورقة العمل، بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع LineShape، بوحدة البكسل. |
| العرض | Int32 | يمثل عرض LineShape، بوحدة البكسل. |
| imageData | Byte[] | بيانات الصورة، تنطبق فقط على الصورة. |
| isOriginalSize | منطقي | ما إذا كان الشكل يستخدم الحجم الأصلي إذا كان الشكل صورة. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeFloatingShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // أضف شكل خط
            Shape floatingShape_Line = shapes.AddFreeFloatingShape(
                MsoDrawingType.Line, 
                100, 100, 100, 50, 
                null, 
                false);

            // إضافة شكل صورة (باستخدام بيانات صورة نموذجية)
            byte[] imageData = null;
            try
            {
                using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
                {
                    imageData = new byte[fs.Length];
                    fs.Read(imageData, 0, (int)fs.Length);
                }
            }
            catch
            {
                // إنشاء بيانات صورة تجريبية إذا لم يُعثر على الملف
                imageData = new byte[100];
            }

            Shape floatingShape_Picture = shapes.AddFreeFloatingShape(
                MsoDrawingType.Picture, 
                200, 100, 100, 50, 
                imageData, 
                false);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


