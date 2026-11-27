---
title: "DigitalSignature.ProviderId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignature property. Anger klass-ID för signaturleverantören. Standardvärdet är Tomt, alla nollor Guid"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/providerid/
---
## DigitalSignature.ProviderId property

Anger klass-ID för signaturleverantören. Standardvärdet är Empty (alla nollor) Guid.

```csharp
public Guid ProviderId { get; set; }
```

### Anmärkningar

Den kryptografiska tjänsteleverantören (CSP) är en oberoende programmodul som faktiskt utför kryptografialgoritmer för autentisering, kodning och kryptering. Microsoft Office reserverar värdet {00000000-0000-0000-0000-000000000000} för sin standardsignaturleverantör och {000CD6A4-0000-0000-C000-000000000046} för sin östasiatiska signaturleverantör. GUID för den ytterligare installerade leverantören bör hämtas från dokumentationen som levereras med leverantören.

### Exempel

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
            // Skapa självsignerat certifikat
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

            // Skapa arbetsbok och lägg till signaturrad
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Lägg till dummy-bild med signaturrad
            using (var ms = new MemoryStream())
            {
                ms.Write(new byte[] { 0x42, 0x4D, 0x1E, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x1A, 0x00, 0x00, 0x00 }, 0, 14);
                ms.Position = 0;
                
                int idx = ws.Pictures.Add(0, 0, ms);
                Picture pic = ws.Pictures[idx];
                pic.SignatureLine = new SignatureLine();
                pic.SignatureLine.ProviderId = Guid.NewGuid();
            }

            // Skapa digital signatur
            var signature = new DigitalSignature(certificate, "Aspose ProviderId Demo", DateTime.Now);
            signature.ProviderId = ws.Pictures[0].SignatureLine.ProviderId;

            // Ställ in digital signatur och spara
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

### Se även

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


