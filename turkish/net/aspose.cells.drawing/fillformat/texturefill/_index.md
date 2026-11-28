---
title: "FillFormat.TextureFill"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FillFormat özelliği. TextureFill nesnesini alır"
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/texturefill/
---
## FillFormat.TextureFill property

`TextureFill` nesnesini alır.

```csharp
public TextureFill TextureFill { get; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTextureFillDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir resim şekli ekleyin
            string imagePath = Path.Combine("your_image_directory", "texture.png");
            int pictureIndex = worksheet.Pictures.Add(0, 0, imagePath);
            Shape picture = worksheet.Shapes[pictureIndex];

            // Texture doldurma özelliklerini ayarla
            picture.Fill.TextureFill.ImageData = File.ReadAllBytes(imagePath);
            picture.Fill.TextureFill.IsTiling = true;
            picture.Fill.TextureFill.Scale = 0.5;

            // Çalışma kitabını kaydedin
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextureFill](../../texturefill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


