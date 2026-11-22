---
title: "فئة PicFormatOption"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.PicFormatOption. يمثل خيار تنسيق الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picformatoption/
---
## PicFormatOption class

يمثل خيار تنسيق الصورة

```csharp
public class PicFormatOption
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PicFormatOption](picformatoption/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Bottom](../../aspose.cells.drawing/picformatoption/bottom/) { get; set; } | يحصل أو يضبط الإزاحة السفلية لتمديد الصورة. |
| [Left](../../aspose.cells.drawing/picformatoption/left/) { get; set; } | يحصل أو يضبط الإزاحة اليسرى لتمديد الصورة. |
| [Right](../../aspose.cells.drawing/picformatoption/right/) { get; set; } | يحصل أو يضبط الإزاحة اليمنى لتمديد الصورة. |
| [Scale](../../aspose.cells.drawing/picformatoption/scale/) { get; set; } | يحصل أو يضبط عدد مكدس الصورة ومعامل مقياسه. |
| [Top](../../aspose.cells.drawing/picformatoption/top/) { get; set; } | يحصل أو يضبط الإزاحة العلوية لتمديد الصورة. |
| [Type](../../aspose.cells.drawing/picformatoption/type/) { get; set; } | يحصل أو يضبط نوع تعبئة الصورة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.IO;

    public class DrawingClassPicFormatOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل وتعيين تعبئة الصورة
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);
            // تمت إزالة خاصية FillType من الوصول إلى MsoFillFormat
            shape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");

            // تكوين خيارات تنسيق الصورة
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.15,
                Right = 0.15,
                Top = 0.15,
                Bottom = 0.15,
                Scale = 0.8
            };

            // إضافة الشكل الثاني مع صورة متكررة
            Shape tiledShape = worksheet.Shapes.AddRectangle(5, 210, 0, 0, 200, 200);
            // تمت إزالة خاصية FillType من الوصول إلى MsoFillFormat
            tiledShape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");
            
            PicFormatOption tileFormat = new PicFormatOption
            {
                Type = FillPictureType.Stack,
                Scale = 1.5
            };

            workbook.Save("PicFormatOptionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


