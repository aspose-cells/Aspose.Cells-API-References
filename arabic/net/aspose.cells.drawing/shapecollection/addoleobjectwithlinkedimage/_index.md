---
title: "ShapeCollection.AddOleObjectWithLinkedImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. إضافة صورة مرتبطة"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addoleobjectwithlinkedimage/
---
## ShapeCollection.AddOleObjectWithLinkedImage method

أضف صورة مرتبطة.

```csharp
public OleObject AddOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, 
    string sourceFullName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| الارتفاع | Int32 | ارتفاع الشكل. بوحدة البكسل |
| العرض | Int32 | عرض الشكل. بوحدة البكسل |
| sourceFullName | String | المسار واسم ملف المصدر للصورة المرتبطة |

### قيمة الإرجاع

[`Picture`](../../picture/) Picture object.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddOleObjectWithLinkedImageWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // المسار إلى ملف الصورة المراد ربطه
            string imagePath = "example.jpg";

            try
            {
                // استدعِ طريقة AddOleObjectWithLinkedImage مع معلمات محددة
                OleObject oleObject = worksheet.Shapes.AddOleObjectWithLinkedImage(
                    1,  // upperLeftRow
                    1,  // upperLeftColumn
                    200, // height
                    300, // width
                    imagePath); // sourceFullName

                // عيّن خصائص إضافية لـ OleObject
                oleObject.DisplayAsIcon = false;
                oleObject.IsAutoSize = true;

                Console.WriteLine("OLE object with linked image added successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddOleObjectWithLinkedImage method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("AddOleObjectWithLinkedImageDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


