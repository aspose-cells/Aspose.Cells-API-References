---
title: "SignatureLine.ProviderId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SignatureLine özelliği. İmza sağlayıcısının kimliğini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/signatureline/providerid/
---
## SignatureLine.ProviderId property

İmza sağlayıcısının kimliğini alır veya ayarlar.

```csharp
public Guid ProviderId { get; set; }
```

### Açıklamalar

Genellikle sağlayıcı COM eklentisinin CLSID'sidir.

### Örnekler

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyProviderIdDemo
    {
        public static void Run()
        {
            // Yeni bir imza satırı oluştur
            SignatureLine signatureLine = new SignatureLine();
            
            // İmza satırı özelliklerini ayarla
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";
            signatureLine.IsLine = true;
            
            // Sağlayıcı kimliğini ayarla (örnek GUID - gerçek sağlayıcı GUID'i ile değiştirilmelidir)
            signatureLine.ProviderId = new Guid("000CD6A4-0000-0000-C000-000000000046");
            
            // İmza tipini ayarla (bu, sağlayıcı kimliğiyle eşleşmelidir)
            signatureLine.SignatureLineType = SignatureType.Stamp;
            
            // Kullanımı göstermek için sağlayıcı kimliğini çıktı al
            Console.WriteLine("Signature Line Provider ID: " + signatureLine.ProviderId);
        }
    }
}
```

### Ayrıca Bakınız

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


