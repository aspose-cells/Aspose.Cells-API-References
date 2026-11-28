---
title: "Enum FillPictureType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.FillPictureType enum. Resim dolgu türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/fillpicturetype/
---
## FillPictureType enumeration

Resim dolgu türünü temsil eder.

```csharp
public enum FillPictureType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Stretch | `0` | Uzat |
| Stack | `1` | Yığma |
| StackAndScale | `2` | StackAndScale |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFillPictureTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Resim dolgusunu göstermek için bir dikdörtgen şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 200, 200);

            // Resim dolgu özelliklerini ayarla
            shape.Fill.Type = FillType.Texture;
            shape.Fill.PictureFormatType = FillPictureType.StackAndScale;

            // Gösterim için minimum 1x1 piksel (beyaz) görüntü kullan
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            shape.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Farklı dolgu türüne sahip başka bir şekil ekle
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 5, 2, 0, 200, 200);
            shape2.Fill.Type = FillType.Texture;
            shape2.Fill.PictureFormatType = FillPictureType.Stretch;
            shape2.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Çalışma kitabını farklı dolgu yapılandırmalarıyla kaydet
            workbook.Save("FillPictureTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


