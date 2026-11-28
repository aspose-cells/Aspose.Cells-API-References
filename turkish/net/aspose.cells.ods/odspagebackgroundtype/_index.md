---
title: "Enum OdsPageBackgroundType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Ods.OdsPageBackgroundType enum. ods sayfasının arka plan türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.ods/odspagebackgroundtype/
---
## OdsPageBackgroundType enumeration

ods sayfa arka planı türünü temsil eder.

```csharp
public enum OdsPageBackgroundType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Arka plan yok. |
| Color | `1` | Arka planı renk ile biçimlendir. |
| Graphic | `2` | Arka planı görüntü ile biçimlendir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundTypeDemo
    {
        public static void OdsPageBackgroundTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasının PageSetup'ına eriş
            PageSetup pageSetup = worksheet.PageSetup;

            // ODSPageBackground özelliğine eriş
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Arka plan türünü Renk olarak ayarla
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Arka plan rengini ayarlayın
            odsPageBackground.Color = Color.LightBlue;

            // Çalışma kitabını kaydedin
            workbook.Save("OdsPageBackgroundTypeExample.ods");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


