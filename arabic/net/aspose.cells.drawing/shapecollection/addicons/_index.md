---
title: "ShapeCollection.AddIcons"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. يضيف صورة svg"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addicons/
---
## ShapeCollection.AddIcons method

يضيف صورة svg.

```csharp
public Picture AddIcons(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageByteData, byte[] compatibleImageData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية للشكل من صفه الأيسر، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | ارتفاع الشكل، بوحدة البكسل. |
| العرض | Int32 | عرض الشكل، بوحدة البكسل. |
| imageByteData | Byte[] | بيانات البايت للصورة. |
| compatibleImageData | Byte[] | بيانات صورة محولة من svg لتكون متوافقة مع Excel 2016 أو الإصدارات الأقدم. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddIconsWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // إنشاء ملف أيقونة تجريبي (في الاستخدام الفعلي، ستستخدم ملفًا موجودًا)
            string iconPath = "icon.svg";
            File.WriteAllText(iconPath, "<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100'><circle cx='50' cy='50' r='40' fill='red'/></svg>");

            // إضافة أيقونة إلى ورقة العمل
            using (FileStream fs = new FileStream(iconPath, FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                Picture picture = shapes.AddIcons(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // احفظ المصنف
            workbook.Save("output.xlsx");

            // تنظيف (اختياري)
            File.Delete(iconPath);
        }
    }
}
```

### انظر أيضًا

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


