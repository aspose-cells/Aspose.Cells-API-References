---
title: "التعداد ControlPictureSizeMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode. يمثل طريقة عرض الصورة."
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/controlpicturesizemode/
---
## ControlPictureSizeMode enumeration

يمثل طريقة عرض الصورة.

```csharp
public enum ControlPictureSizeMode
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Clip | `0` | يقص أي جزء من الصورة أكبر من حدود التحكم. |
| Stretch | `1` | يمدد الصورة لملء مساحة التحكم. هذا الإعداد يشوه الصورة إما في الاتجاه الأفقي أو العمودي. |
| Zoom | `3` | يكبر الصورة، لكنه لا يشوه الصورة في أي من الاتجاهين الأفقي أو العمودي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System.IO;

    public class ControlPictureSizeModeDemo
    {
        public static void ControlPictureSizeModeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة صورة إلى ورقة العمل
            int pictureIndex = worksheet.Pictures.Add(1, 1, "ControlPictureSizeMode.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // إضافة ImageActiveXControl إلى ورقة العمل
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 5, 5,5,100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // ضبط بيانات الصورة لـ ImageActiveXControl
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // اضبط PictureSizeMode إلى Zoom
            imageControl.PictureSizeMode = ControlPictureSizeMode.Zoom;

            // اضبط الخصائص الأخرى لـ ImageActiveXControl
            imageControl.IsAutoSize = true;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black color
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // احفظ المصنف
            workbook.Save("ControlPictureSizeModeExample.xlsx");
            workbook.Save("ControlPictureSizeModeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


