---
title: "DigitalSignature.Id"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DigitalSignature özelliği. Belge içeriğinde saklanan imza satırının GUID'iyle çapraz referans yapılabilen bir GUID belirtir. Varsayılan değer, tüm sıfırlardan oluşan Boş GUID'dir"
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignature/id/
---
## DigitalSignature.Id property

Belge içeriğinde depolanan imza satırının GUID'iyle çapraz referans yapılabilen bir GUID belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID'dir.

```csharp
public Guid Id { get; set; }
```

### Açıklamalar

Ayarlandığında, [`SignatureLine`](../../../aspose.cells.drawing/signatureline/) öğesini ilgili [`DigitalSignature`](../) ile ilişkilendirir.

### Örnekler

```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Belirli bir ID'ye sahip bir dijital imza oluşturun
            Guid signatureId = Guid.NewGuid();
            
            // Dijital imza oluşturun
            X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            
            // İmzanın Id'sini ayarlayın
            signature.Id = signatureId;

            // İmzayı koleksiyona ekleyin
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Dijital imzayı çalışma kitabına uygulayın
            workbook.SetDigitalSignature(dsCollection);

            // Çalışma kitabını kaydedin
            workbook.Save("signed_workbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


