---
title: "PictureBulletValue.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PictureBulletValue. تحصل على نوع قيمة الرصاصة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/picturebulletvalue/type/
---
## PictureBulletValue.Type property

يحصل على نوع قيمة النقطة.

```csharp
public override BulletType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class PictureBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // أنشئ مثيلاً من PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // اعرض قيمة خاصية Type (عملية قراءة فقط)
                Console.WriteLine("PictureBulletValue Type: " + bulletValue.Type);
                
                // عرض أن الخاصية Type تم تعيينها بشكل صحيح إلى Picture لهذه الفئة
                if (bulletValue.Type == BulletType.Picture)
                {
                    Console.WriteLine("Type is correctly set to Picture for PictureBulletValue");
                }
                
                // احفظ المصنف
                workbook.Save("PictureBulletValueTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [BulletType](../../bullettype/)
* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


