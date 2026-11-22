---
title: "ImageActiveXControl.Picture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageActiveXControl. يحصل على ويضبط بيانات الصورة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/
---
## ImageActiveXControl.Picture property

يحصل على بيانات الصورة ويضبطها.

```csharp
public byte[] Picture { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر Image ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 100, 100, 100, 100);
            ImageActiveXControl imgControl = (ImageActiveXControl)shape.ActiveXControl;

            // تعيين الخصائص
            imgControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imgControl.PictureAlignment = ControlPictureAlignmentType.TopLeft;
            imgControl.IsTiled = false;

            // تعيين خاصية Picture (باستخدام مصفوفة بايت لصورة نموذجية)
            byte[] imageData = new byte[] { 0x00, 0x01, 0x02 }; // Sample image data
            imgControl.Picture = imageData;

            // تحقق من تعيين خاصية Picture
            Console.WriteLine("Picture data length: " + imgControl.Picture.Length);

            // احفظ المصنف
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


