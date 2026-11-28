---
title: "Enum ControlPictureSizeMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode enum. Resmin nasıl görüntüleneceğini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/controlpicturesizemode/
---
## ControlPictureSizeMode enumeration

Resmin nasıl görüntüleneceğini temsil eder.

```csharp
public enum ControlPictureSizeMode
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Clip | `0` | Resmin, kontrolün sınırlarından daha büyük olan herhangi bir bölümünü kırpar. |
| Stretch | `1` | Resmi, kontrolün alanını dolduracak şekilde uzatır. Bu ayar, resmi yatay ya da dikey yönde bozar. |
| Zoom | `3` | Resmi büyütür, ancak resmi yatay ya da dikey yönde bozmadan. |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int pictureIndex = worksheet.Pictures.Add(1, 1, "ControlPictureSizeMode.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Çalışma sayfasına bir ImageActiveXControl ekle
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 5, 5,5,100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // ImageActiveXControl için resim verisini ayarla
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // PictureSizeMode özelliğini Zoom olarak ayarlayın
            imageControl.PictureSizeMode = ControlPictureSizeMode.Zoom;

            // ImageActiveXControl'un diğer özelliklerini ayarlayın
            imageControl.IsAutoSize = true;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black color
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // Çalışma kitabını kaydedin
            workbook.Save("ControlPictureSizeModeExample.xlsx");
            workbook.Save("ControlPictureSizeModeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


