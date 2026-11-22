---
title: "Shape.FormatPicture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتعيّن خيارات تنسيق الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/formatpicture/
---
## Shape.FormatPicture property

يحصل ويضبط خيارات تنسيق الصورة.

```csharp
public MsoFormatPicture FormatPicture { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFormatPictureDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // الوصول إلى خاصية FormatPicture الخاصة بالشكل
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;
            
            // عدّل خصائص تنسيق الصورة
            msoFormatPicture.Brightness = 0.5f;
            msoFormatPicture.Contrast = 0.7f;
            msoFormatPicture.Transparency = 0.3f;
            
            // احفظ المصنف
            workbook.Save("ShapePropertyFormatPictureDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../../msoformatpicture/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


