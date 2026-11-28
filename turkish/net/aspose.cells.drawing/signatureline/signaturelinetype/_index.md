---
title: "SignatureLine.SignatureLineType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SignatureLine özelliği. İmza tipini alır veya ayarlar. Default  Varsayılan değer ayarlandığında ilgili ProviderId değeri 00000000000000000000000000000000 olarak sabitlenir. Stamp  Değer Stamp olduğunda ilgili ProviderId değeri genellikle 000CD6A400000000C000000000000046 olur. Custom  Değer Custom olduğunda ilgili ProviderId değeri genellikle kullanıcı tarafından ayarlanmalıdır. Bu değer sağlayıcı ile birlikte gelen belgelerden elde edilmelidir."
type: docs
url: /tr/net/aspose.cells.drawing/signatureline/signaturelinetype/
---
## SignatureLine.SignatureLineType property

İmza tipini alır veya ayarlar. Default - Varsayılan değer ayarlandığında, ilgili ProviderId değeri {0000000000-0000-0000-0000-0000000000} olarak sabitlenir. Stamp - Değer Stamp olduğunda, ilgili ProviderId değeri genellikle {000CD6A4-0000-0000-C000-000000000046} olur. Custom - Değer Custom olduğunda, ilgili ProviderId değeri genellikle kullanıcı tarafından ayarlanmalıdır. Sağlayıcıyla birlikte gönderilen belgelerden elde edilmelidir.

```csharp
public SignatureType SignatureLineType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLinePropertySignatureLineTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir imza satırı oluştur
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Developer";
            signatureLine.Email = "john@example.com";
            signatureLine.IsLine = true;
            signatureLine.AllowComments = true;
            signatureLine.ShowSignedDate = true;
            signatureLine.Instructions = "Please sign here";

            // Mevcut SignatureLineType değerini göster
            Console.WriteLine("Current SignatureLineType: " + signatureLine.SignatureLineType);

            // SignatureLineType değerini Stamp olarak ayarla
            signatureLine.SignatureLineType = SignatureType.Stamp;
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("ProviderId after Stamp type: " + signatureLine.ProviderId);

            // İmza satırını şekillere ekleyerek çalışma sayfasına ekle
            Picture signaturePicture = worksheet.Shapes.AddSignatureLine(0, 0, signatureLine); // Changed to Picture type
            Console.WriteLine("Added signature line with index: " + signaturePicture.OriginalHeight);

            // SignatureLineType değerini özel ProviderId ile Custom olarak değiştir
            signatureLine.SignatureLineType = SignatureType.Custom;
            signatureLine.ProviderId = Guid.NewGuid();
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("Custom ProviderId: " + signatureLine.ProviderId);

            // Çalışma kitabını kaydedin
            workbook.Save("SignatureLineTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SignatureType](../../signaturetype/)
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


