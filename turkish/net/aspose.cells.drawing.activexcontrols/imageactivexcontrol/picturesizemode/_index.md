---
title: "ImageActiveXControl.PictureSizeMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageActiveXControl özelliği. Resmin nasıl görüntüleneceğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/
---
## ImageActiveXControl.PictureSizeMode property

Resmin nasıl görüntüleneceğini alır ve ayarlar.

```csharp
public ControlPictureSizeMode PictureSizeMode { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureSizeModeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir Image ActiveX kontrolü ekleyin
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 200, 200, 0, 0);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // PictureSizeMode özelliğini ve diğer özellikleri ayarlayın
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            
            // Örnek bir resmi yükleyin (kendi resim yolunuzla değiştirin)
            string imagePath = "sample.jpg";
            if (File.Exists(imagePath))
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                imageControl.Picture = imageData;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ImageActiveXControlDemo.xlsx");

            // PictureSizeMode değerini çıktılayın
            Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlPictureSizeMode](../../controlpicturesizemode/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


