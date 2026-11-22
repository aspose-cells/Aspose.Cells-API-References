---
title: "PictureBulletValue.ImageData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PictureBulletValue. تحصل أو تعين بيانات الصورة للرصاصة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/picturebulletvalue/imagedata/
---
## PictureBulletValue.ImageData property

الحصول وتعيين بيانات الصورة للرصاصة.

```csharp
public byte[] ImageData { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class PictureBulletValuePropertyImageDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // أنشئ مثيلاً من PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // عرض تعيين واسترجاع ImageData
                byte[] sampleImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample data
                bulletValue.ImageData = sampleImageData;
                
                // اعرض قيمة خاصية ImageData
                Console.WriteLine("ImageData length: " + (bulletValue.ImageData?.Length ?? 0) + " bytes");
                
                // اعرض خاصية Type (للقراءة فقط)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // احفظ المصنف
                workbook.Save("PictureBulletValueImageDataDemo.xlsx");
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

* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


