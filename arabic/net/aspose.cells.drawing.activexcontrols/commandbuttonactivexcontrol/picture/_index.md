---
title: "CommandButtonActiveXControl.Picture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "CommandButtonActiveXControl خاصية. يحصل ويضبط بيانات الصورة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/
---
## CommandButtonActiveXControl.Picture property

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
    public class CommandButtonActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل لاستضافة عنصر تحكم ActiveX مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CommandButton, 
                1,  // top row
                1,  // left column
                0,  // top position
                0,  // left position
                100, // width
                30); // height
                
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            // تعيين الخصائص
            button.Caption = "Click Me";
            button.PicturePosition = ControlPicturePositionType.AboveCenter;

            // اضبط الصورة (مصفوفة البايت الفارغة تمثل عدم وجود صورة)
            button.Picture = new byte[0];

            // احفظ المصنف
            workbook.Save("CommandButtonWithPicture.xlsx");

            // تحقق من خاصية picture
            Console.WriteLine("Picture is null: " + (button.Picture == null));
        }
    }
}
```

### انظر أيضًا

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


