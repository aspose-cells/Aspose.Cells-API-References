---
title: "التعداد ControlPictureAlignmentType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType. يمثل محاذاة الصورة داخل النموذج أو الصورة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/controlpicturealignmenttype/
---
## ControlPictureAlignmentType enumeration

يمثل محاذاة الصورة داخل الـ Form أو Image.

```csharp
public enum ControlPictureAlignmentType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| TopLeft | `0` | الزاوية العلوية اليسرى. |
| TopRight | `1` | الزاوية العلوية اليمنى. |
| Center | `2` | الوسط. |
| BottomLeft | `3` | الزاوية السفلية اليسرى. |
| BottomRight | `4` | الزاوية السفلية اليمنى. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPictureAlignmentTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر ImageActiveXControl مع جميع المعلمات المطلوبة
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                10,  // left
                10,  // top
                200, // width
                200, // height
                0,   // imageWidth
                0    // imageHeight
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // تعيين خصائص الصورة
            imageControl.Picture = File.ReadAllBytes("sample.png");
            imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Stretch;

            // احفظ المصنف
            workbook.Save("ImageControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


