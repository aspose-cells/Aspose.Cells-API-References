---
title: "Picture.Data"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. تحصل على بيانات الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picture/data/
---
## Picture.Data property

يحصل على بيانات الصورة.

```csharp
public byte[] Data { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إدراج الصورة الأولى
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "example1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // إدراج الصورة الثانية
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "example2.jpeg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // عرض خاصية Data عن طريق نسخ بيانات الصورة
            pic2.Data = pic1.Data;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


