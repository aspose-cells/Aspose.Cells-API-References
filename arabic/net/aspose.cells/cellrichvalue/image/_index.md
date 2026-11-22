---
title: "CellRichValue.Image"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellRichValue. يحصل على بيانات الصورة للخلية"
type: docs
url: /ar/net/aspose.cells/cellrichvalue/image/
---
## CellRichValue.Image property

يحصل على بيانات الصورة للخلية.

```csharp
public virtual byte[] Image { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class CellRichValuePropertyImageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة صورة إلى ورقة العمل
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // الحصول على قيمة الخلية الغنية التي تحتوي على الصورة
            Cell cell = worksheet.Cells[0, 0];
            cell.PutValue("test data");
            cell.EmbeddedImage = picture.Data;

            // الوصول إلى القيمة الغنية
            CellRichValue richValue = cell.GetRichValue();

            // عرض خصائص الصورة
            Console.WriteLine("Image data length: " + (richValue.Image?.Length ?? 0));
            Console.WriteLine("Alt text: " + richValue.AltText);

            // تعيين نص بديل جديد للصورة
            richValue.AltText = "Sample product image";

            // احفظ المصنف
            workbook.Save("CellRichValueImageDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


