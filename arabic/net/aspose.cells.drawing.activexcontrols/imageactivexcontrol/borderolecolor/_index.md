---
title: "ImageActiveXControl.BorderOleColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageActiveXControl. تحصل وتضبط لون ole للخلفية"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderolecolor/
---
## ImageActiveXControl.BorderOleColor property

يحصل ويضبط لون الـole للخلفية.

```csharp
public int BorderOleColor { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 5, 0, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            imageControl.BorderOleColor = 0x0000FF; // Blue border
            imageControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;

            // إنشاء صورة بسيطة في الذاكرة إذا لم يكن ملف العرض موجودًا
            byte[] imageData;
            if (!File.Exists("demo.jpg"))
            {
                // إنشاء صورة بديلة دون System.Drawing
                imageData = CreateSampleImage(100, 100);
            }
            else
            {
                imageData = File.ReadAllBytes("demo.jpg");
            }

            imageControl.Picture = imageData;
            workbook.Save("ImageActiveXControlBorderColorDemo.xlsx");

            Console.WriteLine($"Border color set to: {imageControl.BorderOleColor:X6}");
        }

        private static byte[] CreateSampleImage(int width, int height)
        {
            // إنشاء صورة رمادية بسيطة دون System.Drawing
            byte[] pixels = new byte[width * height * 3]; // RGB
            for (int i = 0; i < pixels.Length; i++)
            {
                pixels[i] = 200; // Light gray color
            }
            return pixels;
        }
    }
}
```

### انظر أيضًا

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


