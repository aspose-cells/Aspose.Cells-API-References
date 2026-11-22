---
title: "ShapeCollection.AddSvg"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. يضيف صورة svg"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addsvg/
---
## ShapeCollection.AddSvg method

يضيف صورة svg.

```csharp
public Picture AddSvg(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] svgData, byte[] compatibleImageData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية للشكل من صفه الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | ارتفاع الشكل، بوحدة البكسل. |
| العرض | Int32 | عرض الشكل، بوحدة البكسل. |
| svgData | Byte[] | بيانات صورة svg. |
| compatibleImageData | Byte[] | بيانات صورة محولة من svg لتكون متوافقة مع Excel 2016 أو الإصدارات الأقدم. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSvgWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.ShapeCollection shapes = worksheet.Shapes;

            // تحميل ملف SVG
            using (FileStream fs = new FileStream("image.svg", FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                
                // إضافة SVG إلى ورقة العمل
                Aspose.Cells.Drawing.Picture picture = shapes.AddSvg(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


