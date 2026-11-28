---
title: "Enum OdsPageBackgroundGraphicType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicType enum. Görüntülü sayfa arka planı biçimlendirme türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.ods/odspagebackgroundgraphictype/
---
## OdsPageBackgroundGraphicType enumeration

Resim içeren sayfa arka planı biçimlendirme türünü temsil eder.

```csharp
public enum OdsPageBackgroundGraphicType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Position | `0` | Görüntüyü belirli konuma ayarlayın. |
| Area | `1` | Görüntüyü uzatın. |
| Tile | `2` | Görüntüyü tekrarlayın ve yineleyin. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundGraphicTypeDemo
    {
        public static void OdsPageBackgroundGraphicTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasının PageSetup'ına eriş
            PageSetup pageSetup = worksheet.PageSetup;

            // PageSetup'ın ODSPageBackground'ına erişin
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Arka plan rengini ayarlayın
            odsPageBackground.Color = Color.LightBlue;

            // Arka plan grafik türünü Döşeme olarak ayarlayın
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Bağlantılı grafik yolunu ayarlayın (görüntünün çalıştırılabilir dosyayla aynı dizinde olduğunu varsayarak)
            odsPageBackground.LinkedGraphic = "background_image.png";

            // Çalışma kitabını kaydedin
            workbook.Save("OdsPageBackgroundGraphicTypeExample.ods");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


