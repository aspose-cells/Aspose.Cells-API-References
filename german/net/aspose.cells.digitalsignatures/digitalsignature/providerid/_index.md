---
title: "DigitalSignature.ProviderId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DigitalSignature property. Gibt die Klassen-ID des Signaturanbieters an. Standardwert ist ein leerer GUID mit allen Nullen."
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignature/providerid/
---
## DigitalSignature.ProviderId property

Gibt die Klassen-ID des Signaturanbieters an. Standardwert ist Empty (alle Nullen) Guid.

```csharp
public Guid ProviderId { get; set; }
```

### Hinweise

Der kryptografische Dienstanbieter (CSP) ist ein unabhängiges Softwaremodul, das tatsächlich kryptografische Algorithmen für Authentifizierung, Codierung und Verschlüsselung ausführt. Microsoft Office reserviert den Wert {00000000-0000-0000-0000-000000000000} für seinen Standard‑Signaturanbieter und {000CD6A4-0000-0000-C000-000000000046} für seinen ostasiatischen Signaturanbieter. Der GUID des zusätzlich installierten Anbieters sollte aus der mit dem Anbieter gelieferten Dokumentation entnommen werden.

### Beispiele

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
            // Selbstsigniertes Zertifikat erstellen
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

            // Arbeitsmappe erstellen und Signaturzeile hinzufügen
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Platzhalterbild mit Signaturzeile hinzufügen
            using (var ms = new MemoryStream())
            {
                ms.Write(new byte[] { 0x42, 0x4D, 0x1E, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x1A, 0x00, 0x00, 0x00 }, 0, 14);
                ms.Position = 0;
                
                int idx = ws.Pictures.Add(0, 0, ms);
                Picture pic = ws.Pictures[idx];
                pic.SignatureLine = new SignatureLine();
                pic.SignatureLine.ProviderId = Guid.NewGuid();
            }

            // Digitale Signatur erstellen
            var signature = new DigitalSignature(certificate, "Aspose ProviderId Demo", DateTime.Now);
            signature.ProviderId = ws.Pictures[0].SignatureLine.ProviderId;

            // Digitale Signatur festlegen und speichern
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

### Siehe auch

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


