---
title: "Sınıf PicFormatOption"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.PicFormatOption sınıfı. Resim formatı seçeneğini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/picformatoption/
---
## PicFormatOption class

Resim biçimi seçeneğini temsil eder.

```csharp
public class PicFormatOption
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PicFormatOption](picformatoption/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Bottom](../../aspose.cells.drawing/picformatoption/bottom/) { get; set; } | Resmi uzatmak için alt ofseti alır veya ayarlar. |
| [Left](../../aspose.cells.drawing/picformatoption/left/) { get; set; } | Resmi uzatmak için sol ofseti alır veya ayarlar. |
| [Right](../../aspose.cells.drawing/picformatoption/right/) { get; set; } | Resmi uzatmak için sağ ofseti alır veya ayarlar. |
| [Scale](../../aspose.cells.drawing/picformatoption/scale/) { get; set; } | Resmin kaç katmanla yığıldığını ve ölçeklendirileceğini alır veya ayarlar. |
| [Top](../../aspose.cells.drawing/picformatoption/top/) { get; set; } | Resmi uzatmak için üst ofseti alır veya ayarlar. |
| [Type](../../aspose.cells.drawing/picformatoption/type/) { get; set; } | Resim doldurma tipini alır veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.IO;

    public class DrawingClassPicFormatOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir şekil ekleyin ve resim doldurmasını ayarlayın
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);
            // MsoFillFormat erişiminden FillType özelliği kaldırıldı
            shape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");

            // Resim formatı seçeneklerini yapılandırın
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.15,
                Right = 0.15,
                Top = 0.15,
                Bottom = 0.15,
                Scale = 0.8
            };

            // Döşeli görüntülü ikinci şekli ekleyin
            Shape tiledShape = worksheet.Shapes.AddRectangle(5, 210, 0, 0, 200, 200);
            // MsoFillFormat erişiminden FillType özelliği kaldırıldı
            tiledShape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");
            
            PicFormatOption tileFormat = new PicFormatOption
            {
                Type = FillPictureType.Stack,
                Scale = 1.5
            };

            workbook.Save("PicFormatOptionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


