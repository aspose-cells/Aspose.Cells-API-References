---
title: "SignatureLine sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.SignatureLine sınıfı. İmza satırını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

İmza satırını temsil eder.

```csharp
public class SignatureLine
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SignatureLine](signatureline/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments/) { get; set; } | Yorumların eklenip eklenemeyeceğini gösterir. |
| [Email](../../aspose.cells.drawing/signatureline/email/) { get; set; } | Şarkıcının e-posta adresini alır veya ayarlar. |
| [Id](../../aspose.cells.drawing/signatureline/id/) { get; set; } | Bu imza satırı için tanımlayıcıyı alır veya ayarlar. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions/) { get; set; } | İmzalama sırasında kullanıcıya gösterilen metni alır veya ayarlar. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline/) { get; set; } | Bir imza satırı olup olmadığını gösterir. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid/) { get; set; } | İmza sağlayıcısının kimliğini alır veya ayarlar. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate/) { get; set; } | İmzalanma tarihinin gösterilip gösterilmeyeceğini belirtir. |
| [SignatureLineType](../../aspose.cells.drawing/signatureline/signaturelinetype/) { get; set; } | İmza tipini alır veya ayarlar. Default - Varsayılan değer ayarlandığında, ilgili ProviderId değeri {0000000000-0000-0000-0000-0000000000} olarak sabitlenir. Stamp - Değer Stamp olduğunda, ilgili ProviderId değeri genellikle {000CD6A4-0000-0000-C000-000000000046} olur. Custom - Değer Custom olduğunda, ilgili ProviderId değeri genellikle kullanıcı tarafından ayarlanmalıdır. Sağlayıcıyla birlikte gönderilen belgelerden elde edilmelidir. |
| [Signer](../../aspose.cells.drawing/signatureline/signer/) { get; set; } | İmzayı yapanı alır veya ayarlar. |
| [Title](../../aspose.cells.drawing/signatureline/title/) { get; set; } | Şarkıcının unvanını alır veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLineDemo
    {
        public static void SignatureLineExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir resim ekleme
            int imgIndex = worksheet.Pictures.Add(1, 1, "SignatureLineExample_original.png");
            Picture pic = worksheet.Pictures[imgIndex];

            // İmza satırı nesnesi oluştur.
            SignatureLine s = new SignatureLine();
            s.Signer = "Simon Zhao";
            s.Title = "Development Lead";
            s.Email = "Simon.Zhao@aspose.com";
            s.Id = Guid.NewGuid();
            s.ProviderId = Guid.NewGuid();
            s.IsLine = true;
            s.AllowComments = true;
            s.ShowSignedDate = true;
            s.Instructions = "Just do it.";

            // Signature line nesnesini Picture.SignatureLine özelliğine atayın
            pic.SignatureLine = s;

            // Excel dosyasını kaydet.
            workbook.Save("SignatureLineExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


