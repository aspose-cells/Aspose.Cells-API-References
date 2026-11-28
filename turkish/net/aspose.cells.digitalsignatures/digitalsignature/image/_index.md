---
title: "DigitalSignature.Image"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DigitalSignature özelliği. Dijital imza için bir görüntü belirtir. Varsayılan değer null'dır"
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignature/image/
---
## DigitalSignature.Image property

Dijital imza için bir görüntü belirtir. Varsayılan değer null'dur.

```csharp
public byte[] Image { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.DigitalSignatures;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyImageDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Çalışma sayfasına bir imza satırı ekleyin
            Picture picture = ws.Pictures[0];
            SignatureLine signatureLine = picture.SignatureLine;
            signatureLine.Signer = "Test Signer";
            signatureLine.Title = "Test Title";

            // Bir test sertifikası oluşturun (gerçek kullanımda, dosyadan yükleyin)
            byte[] certData = new byte[0]; // Replace with actual certificate bytes
            X509Certificate2 certificate = new X509Certificate2(certData);

            // Görüntülü bir dijital imza oluşturun
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            signature.Image = File.ReadAllBytes("signature.png"); // Replace with actual image path

            // İmzayı ekleyin ve kaydedin
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);
            wb.SetDigitalSignature(dsCollection);

            // Bellek akışına kaydet
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


