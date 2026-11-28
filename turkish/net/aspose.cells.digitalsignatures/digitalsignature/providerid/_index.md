---
title: "DigitalSignature.ProviderId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DigitalSignature özelliği. İmza sağlayıcısının sınıf kimliğini belirtir. Varsayılan değer, tüm sıfırlardan oluşan boş GUID'dir."
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignature/providerid/
---
## DigitalSignature.ProviderId property

İmza sağlayıcısının sınıf kimliğini (class ID) belirtir. Varsayılan değer Boş (tüm sıfırlar) GUID'dir.

```csharp
public Guid ProviderId { get; set; }
```

### Açıklamalar

Kriptografik hizmet sağlayıcı (CSP), kimlik doğrulama, kodlama ve şifreleme için kriptografi algoritmalarını gerçekte yürüten bağımsız bir yazılım modülüdür. Microsoft Office, varsayılan imza sağlayıcısı için {00000000-0000-0000-0000-000000000000} değerini, Doğu Asya imza sağlayıcısı için ise {000CD6A4-0000-0000-C000-000000000046} değerini ayırır. Ek olarak kurulan sağlayıcının GUID'i, sağlayıcıyla birlikte gelen belgelerden elde edilmelidir.

### Örnekler

```csharp
using System;
using System.IO;
using System.Security.Cryptography;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyProviderIdDemo
    {
        public static void Run()
        {
            // Kendinden imzalı sertifika oluşturun
            X509Certificate2 certificate;
            using (var rsa = RSA.Create())
            {
                var request = new CertificateRequest(
                    new X500DistinguishedName("cn=AsposeTest"),
                    rsa,
                    HashAlgorithmName.SHA256,
                    RSASignaturePadding.Pkcs1);
                
                certificate = request.CreateSelfSigned(DateTimeOffset.Now, DateTimeOffset.Now.AddHours(1));
            }

            // Çalışma kitabı oluşturun ve imza satırı ekleyin
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // İmza satırıyla sahte bir resim ekleyin
            using (var ms = new MemoryStream())
            {
                ms.Write(new byte[] { 0x42, 0x4D, 0x1E, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x1A, 0x00, 0x00, 0x00 }, 0, 14);
                ms.Position = 0;
                
                int idx = ws.Pictures.Add(0, 0, ms);
                Picture pic = ws.Pictures[idx];
                pic.SignatureLine = new SignatureLine();
                pic.SignatureLine.ProviderId = Guid.NewGuid();
            }

            // Dijital imza oluşturun
            var signature = new DigitalSignature(certificate, "Aspose ProviderId Demo", DateTime.Now);
            signature.ProviderId = ws.Pictures[0].SignatureLine.ProviderId;

            // Dijital imzayı ayarlayın ve kaydedin
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);
            wb.SetDigitalSignature(dsCollection);

            using (MemoryStream output = new MemoryStream())
            {
                wb.Save(output, SaveFormat.Xlsx);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


