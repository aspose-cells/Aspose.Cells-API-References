---
title: "ImageActiveXControl.IsAutoSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageActiveXControl. تشير إلى ما إذا كان التحكم سيعيد الحجم تلقائيًا لعرض كامل محتوياته"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/isautosize/
---
## ImageActiveXControl.IsAutoSize property

يشير إلى ما إذا كان العنصر سيعيد حجمه تلقائيًا لعرض محتوياته بالكامل.

```csharp
public override bool IsAutoSize { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة ImageActiveXControl إلى ورقة العمل
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                5,  // left
                5,  // top
                100, // width
                100, // height
                0,   // imageWidth (0 for default)
                0    // imageHeight (0 for default)
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // تعيين بيانات الصورة (تأكد من وجود ملف الصورة)
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // عرض خاصية IsAutoSize
            imageControl.IsAutoSize = true; // Control will automatically resize to fit the image
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Zoom;

            // احفظ المصنف
            workbook.Save("ImageActiveXControlIsAutoSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


