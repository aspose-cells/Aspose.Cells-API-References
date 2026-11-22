---
title: "Enum ImageBinarizationMethod"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Rendering.ImageBinarizationMethod enum. يحدد الطريقة المستخدمة لتصوير الصورة ثنائية"
type: docs
url: /ar/net/aspose.cells.rendering/imagebinarizationmethod/
---
## ImageBinarizationMethod enumeration

يحدد الطريقة المستخدمة لتحويل الصورة إلى ثنائية.

```csharp
public enum ImageBinarizationMethod
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Threshold | `0` | يحدد طريقة العتبة. |
| FloydSteinbergDithering | `1` | يحدد التمويه باستخدام طريقة انتشار الخطأ فلويد-ستينبرغ. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class RenderingClassImageBinarizationMethodDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد ببيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء الخلايا بقيم تدرجية للتوضيح
            for (int row = 0; row < 50; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue((double)(row * col) / 500);
                }
            }

            // تكوين خيارات عرض الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4,
                TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering
            };

            // إنشاء عرض للورقة باستخدام الخيارات المكوّنة
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // عرض الصفحة الأولى من ورقة العمل كصورة مع التحويل الثنائي
            renderer.ToImage(0, "BinarizedOutput.tiff");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


