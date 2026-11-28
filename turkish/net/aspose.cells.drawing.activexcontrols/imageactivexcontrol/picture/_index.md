---
title: "ImageActiveXControl.Picture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageActiveXControl özelliği. Resmin verisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/
---
## ImageActiveXControl.Picture property

Resmin verilerini alır ve ayarlar.

```csharp
public byte[] Picture { get; set; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir Image ActiveX kontrolü ekleyin
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 100, 100, 100, 100);
            ImageActiveXControl imgControl = (ImageActiveXControl)shape.ActiveXControl;

            // Özellikleri ayarla
            imgControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imgControl.PictureAlignment = ControlPictureAlignmentType.TopLeft;
            imgControl.IsTiled = false;

            // Picture özelliğini ayarlayın (örnek bir resim bayt dizisi kullanarak)
            byte[] imageData = new byte[] { 0x00, 0x01, 0x02 }; // Sample image data
            imgControl.Picture = imageData;

            // Picture özelliğinin ayarlandığını doğrulayın
            Console.WriteLine("Picture data length: " + imgControl.Picture.Length);

            // Çalışma kitabını kaydedin
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


