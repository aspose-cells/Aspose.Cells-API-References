---
title: "PicFormatOption.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PicFormatOption. تحصل أو تعين نوع تعبئة الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picformatoption/type/
---
## PicFormatOption.Type property

يحصل أو يضبط نوع تعبئة الصورة.

```csharp
public FillPictureType Type { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أنشئ صورة BMP بسيطة بحجم 1×1 بكسل
            byte[] bmpBytes = new byte[]
            {
                0x42, 0x4D, 0x39, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
                0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
                0x18, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00
            };

            // إضافة صورة إلى ورقة العمل
            int pictureIndex = worksheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes));
            Picture picture = worksheet.Pictures[pictureIndex];

            // حدد موضع الصورة وحجمها
            picture.UpperLeftRow = 0;
            picture.UpperLeftColumn = 0;
            picture.LowerRightRow = 5;
            picture.LowerRightColumn = 5;

            try
            {
                // احصل على PicFormatOption من تعبئة نسيج الصورة
                PicFormatOption picFormat = picture.Fill.TextureFill.PicFormatOption;

                // عرض قيمة Type الحالية
                Console.WriteLine("Current Type: " + picFormat.Type);

                // عيّن قيم Type مختلفة وعرضها
                picFormat.Type = FillPictureType.Stretch;
                Console.WriteLine("Type set to Stretch: " + picFormat.Type);

                picFormat.Type = FillPictureType.Stack;
                Console.WriteLine("Type set to Stack: " + picFormat.Type);

                picFormat.Type = FillPictureType.StackAndScale;
                Console.WriteLine("Type set to StackAndScale: " + picFormat.Type);

                // احفظ المصنف
                workbook.Save("PicFormatOptionTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
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

* enum [FillPictureType](../../fillpicturetype/)
* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


