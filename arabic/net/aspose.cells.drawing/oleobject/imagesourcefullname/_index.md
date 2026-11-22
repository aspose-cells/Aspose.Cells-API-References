---
title: "OleObject.ImageSourceFullName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تحصل أو تضبط مسار واسم ملف المصدر للصورة المرتبطة"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/imagesourcefullname/
---
## OleObject.ImageSourceFullName property

يحصل على أو يضبط المسار واسم ملف المصدر للصورة المرتبطة.

```csharp
public string ImageSourceFullName { get; set; }
```

### ملاحظات

القيمة الافتراضية هي سلسلة فارغة. إذا لم يكن SourceFullName سلسلة فارغة، فإن الصورة مرتبطة. إذا لم يكن SourceFullName سلسلة فارغة، ولكن Data يساوي null، فإن الصورة تكون مرتبطة ولا تُخزن في الملف.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageSourceFullNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملف PDF تجريبي للتضمين
            byte[] pdfBytes = File.ReadAllBytes("example.pdf");

            // إضافة OleObject إلى ورقة العمل
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfBytes);
            OleObject oleObj = worksheet.OleObjects[oleIndex];

            // قم بتعيين خصائص OleObject بما في ذلك ImageSourceFullName
            oleObj.DisplayAsIcon = false;
            oleObj.FileFormatType = FileFormatType.Pdf;
            oleObj.ImageSourceFullName = "sample_image.png"; // Demonstrating ImageSourceFullName usage
            oleObj.IsAutoSize = false;
            oleObj.IsLink = false;
            oleObj.ProgID = "Acrobat.Document.DC";

            // احفظ المصنف
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


