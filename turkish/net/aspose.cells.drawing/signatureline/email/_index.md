---
title: "SignatureLine.Email"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SignatureLine özelliği. Şarkıcının e-posta adresini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/signatureline/email/
---
## SignatureLine.Email property

Şarkıcının e-posta adresini alır veya ayarlar.

```csharp
public string Email { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyEmailDemo
    {
        public static void Run()
        {
            // Yeni bir imza satırı oluştur
            SignatureLine signatureLine = new SignatureLine();
            
            // İmza satırı özelliklerini e-posta dahil ayarla
            signatureLine.Signer = "Simon Zhao";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "Simon.Zhao@aspose.com";
            signatureLine.IsLine = true;
            signatureLine.ShowSignedDate = true;
            
            // E-posta özelliğini göster
            Console.WriteLine("Signer Email: " + signatureLine.Email);
        }
    }
}
```

### Ayrıca Bakınız

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


