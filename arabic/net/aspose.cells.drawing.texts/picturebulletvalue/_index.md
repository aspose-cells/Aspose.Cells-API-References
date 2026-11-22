---
title: "الفئة PictureBulletValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.Texts.PictureBulletValue class. تمثل قيمة رصاصة الصورة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/picturebulletvalue/
---
## PictureBulletValue class

يمثل قيمة رصاصة الصورة.

```csharp
public class PictureBulletValue : BulletValue
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PictureBulletValue](picturebulletvalue/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ImageData](../../aspose.cells.drawing.texts/picturebulletvalue/imagedata/) { get; set; } | الحصول وتعيين بيانات الصورة للرصاصة. |
| override [Type](../../aspose.cells.drawing.texts/picturebulletvalue/type/) { get; } | يحصل على نوع قيمة النقطة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class TextsClassPictureBulletValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // إنشاء نسخة من الفئة PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // تحميل بيانات صورة تجريبية (استبدل بمسار الصورة الفعلي)
                string imagePath = "sample.png";
                if (File.Exists(imagePath))
                {
                    bulletValue.ImageData = File.ReadAllBytes(imagePath);
                    
                    // عرض المعلومات الأساسية
                    Console.WriteLine($"PictureBulletValue created with Type: {bulletValue.Type}");
                    Console.WriteLine($"Image data length: {bulletValue.ImageData?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Sample image not found, using empty bullet value");
                }
                
                // احفظ المصنف
                workbook.Save("PictureBulletValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PictureBulletValue: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


