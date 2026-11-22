---
title: "ImageActiveXControl.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageActiveXControl. يحصل على نوع التحكم ActiveX"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/type/
---
## ImageActiveXControl.Type property

يحصل على نوع عنصر التحكم ActiveX.

```csharp
public override ControlType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة عنصر تحكم Image ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 1, 1, 200, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
            
            // توضيح استخدام خاصية Type
            Console.WriteLine("Control Type: " + imageControl.Type);
            
            // تعيين بعض الخصائص
            imageControl.IsAutoSize = false;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Clip;
            
            // احفظ المصنف
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlType](../../controltype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


