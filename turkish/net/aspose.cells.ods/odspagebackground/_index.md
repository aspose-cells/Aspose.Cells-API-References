---
title: "Sınıf OdsPageBackground"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Ods.OdsPageBackground sınıfı. ODS sayfa arka planını temsil eder"
type: docs
url: /tr/net/aspose.cells.ods/odspagebackground/
---
## OdsPageBackground class

ods'nin sayfa arka planını temsil eder.

```csharp
public class OdsPageBackground
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [OdsPageBackground](odspagebackground/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Color](../../aspose.cells.ods/odspagebackground/color/) { get; set; } | Arka plan rengini alır ve ayarlar. |
| [GraphicData](../../aspose.cells.ods/odspagebackground/graphicdata/) { get; set; } | Grafik verisini alır ve ayarlar. |
| [GraphicPositionType](../../aspose.cells.ods/odspagebackground/graphicpositiontype/) { get; set; } | Arka plan grafik konumunu alır ve ayarlar. |
| [GraphicType](../../aspose.cells.ods/odspagebackground/graphictype/) { get; set; } | Sayfa arka planı grafik tipini alır ve ayarlar. |
| [IsLink](../../aspose.cells.ods/odspagebackground/islink/) { get; } | Bağlantılı bir grafik olup olmadığını gösterir. |
| [LinkedGraphic](../../aspose.cells.ods/odspagebackground/linkedgraphic/) { get; set; } | Bağlantılı grafik yolunu alır ve ayarlar. |
| [Type](../../aspose.cells.ods/odspagebackground/type/) { get; set; } | Sayfa arka plan tipini alır ve ayarlar. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundDemo
    {
        public static void OdsPageBackgroundExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // PageSetup nesnesine erişin
            PageSetup pageSetup = sheet.PageSetup;

            // ODSPageBackground nesnesine eriş
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Arka plan türünü Renk olarak ayarla
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Arka plan rengini ayarlayın
            odsPageBackground.Color = Color.LightBlue;

            // Arka plan grafik tipini ayarla
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Arka plan grafik konumunu ayarla
            odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;

            // Bağlantılı grafik yolunu ayarla (varsa)
            odsPageBackground.LinkedGraphic = "path/to/graphic.png";

            // Çalışma kitabını kaydedin
            workbook.Save("OdsPageBackgroundExample.ods");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


