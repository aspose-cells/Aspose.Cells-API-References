---
title: "ImageActiveXControl.BorderOleColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageActiveXControl özelliği. Arka planın ole rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderolecolor/
---
## ImageActiveXControl.BorderOleColor property

Arka planın ole rengini alır ve ayarlar.

```csharp
public int BorderOleColor { get; set; }
```

### Örnekler

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

            // Demo dosyası mevcut değilse bellekte basit bir görüntü oluştur
            byte[] imageData;
            if (!File.Exists("demo.jpg"))
            {
                // System.Drawing olmadan alternatif görüntü oluşturma
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
            // System.Drawing olmadan basit bir gri tonlamalı görüntü oluştur
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

### Ayrıca Bakınız

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


