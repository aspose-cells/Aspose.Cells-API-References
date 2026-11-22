---
title: "Picture.IsAutoSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. True تشير إلى أن حجم كائن ole سيتغير تلقائيًا كما حجم لقطة المحتوى المضمن عندما يتم تنشيط كائن ole"
type: docs
url: /ar/net/aspose.cells.drawing/picture/isautosize/
---
## Picture.IsAutoSize property

صحيح يعني أن حجم كائن OLE سيتغير تلقائيًا ليتطابق مع حجم لقطة المحتوى المضمن عند تفعيل كائن OLE.

```csharp
public bool IsAutoSize { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // عرض خاصية IsAutoSize
            Console.WriteLine("Original IsAutoSize value: " + picture.IsAutoSize);
            
            // عيّن IsAutoSize إلى true - الصورة ستُعيد حجمها تلقائيًا لتتناسب مع محتواها
            picture.IsAutoSize = true;
            Console.WriteLine("After setting IsAutoSize to true: " + picture.IsAutoSize);
            
            // عيّن IsAutoSize إلى false - الصورة ستحافظ على أبعادها الأصلية
            picture.IsAutoSize = false;
            Console.WriteLine("After setting IsAutoSize to false: " + picture.IsAutoSize);

            // احفظ المصنف
            workbook.Save("PicturePropertyIsAutoSizeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


