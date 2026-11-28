---
title: "FillFormat.PictureFormatType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FillFormat özelliği. Resim formatı türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/pictureformattype/
---
## FillFormat.PictureFormatType property

Resim formatı tipini alır ve ayarlar.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Resim doldurmayı göstermek için bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Resim dolgu özelliklerini ayarla
            shape.Fill.Type = FillType.Texture;
            shape.Fill.Texture = TextureType.BlueTissuePaper;
            shape.Fill.PictureFormatType = FillPictureType.Stretch;

            // Çalışma kitabını kaydedin
            workbook.Save("FillFormatPictureTypeDemo.xlsx");

            // Kaydedilmiş çalışma kitabını yükleyerek özellikleri doğrulayın
            Workbook verifyWorkbook = new Workbook("FillFormatPictureTypeDemo.xlsx");
            Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];

            // PictureFormatType değerini çıktılayarak kullanımını gösterin
            Console.WriteLine("PictureFormatType: " + verifyShape.Fill.PictureFormatType);
        }
    }
}
```

### Ayrıca Bakınız

* enum [FillPictureType](../../fillpicturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


