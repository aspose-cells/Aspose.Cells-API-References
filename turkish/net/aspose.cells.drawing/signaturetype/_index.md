---
title: "Enum SignatureType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.SignatureType enum. İmza tipini belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/signaturetype/
---
## SignatureType enumeration

İmza türünü belirtir.

```csharp
public enum SignatureType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` | Varsayılan değer, ilgili ProviderId değeri {0000000000-0000-0000-0000-0000000000} olarak sabitlenir. |
| Stamp | `1` | İlgili ProviderId değeri genellikle {000CD6A4-0000-0000-C000-000000000046} olur. |
| Custom | `3` | İlgili ProviderId değeri genellikle kullanıcı tarafından ayarlanmalıdır. Sağlayıcıyla birlikte gelen belgelerden elde edilmelidir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassSignatureTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Farklı tiplerde imza satırları ekle
            Picture stampPicture = worksheet.Shapes.AddSignatureLine(3, 1, new SignatureLine());
            stampPicture.SignatureLine.SignatureLineType = SignatureType.Stamp;

            Picture customPicture = worksheet.Shapes.AddSignatureLine(8, 1, new SignatureLine());
            customPicture.SignatureLine.SignatureLineType = SignatureType.Custom;
            customPicture.SignatureLine.ProviderId = new Guid("12345678-ABCD-4321-5678-9876543210AB");

            // Çalışma kitabını imza yapılandırmalarıyla kaydet
            workbook.Save("SignatureTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


