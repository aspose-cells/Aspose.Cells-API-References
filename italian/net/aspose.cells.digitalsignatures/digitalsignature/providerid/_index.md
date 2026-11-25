---
title: "DigitalSignature.ProviderId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DigitalSignature. Specifica l'ID classe del provider di firma. Il valore predefinito è Guid vuoto, tutti zero"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignature/providerid/
---
## DigitalSignature.ProviderId property

Specifica l'ID classe del provider di firma. Il valore predefinito è Empty (tutti zero) Guid.

```csharp
public Guid ProviderId { get; set; }
```

### Osservazioni

Il provider di servizi crittografici (CSP) è un modulo software indipendente che esegue effettivamente gli algoritmi crittografici per l'autenticazione, la codifica e la cifratura. Microsoft Office riserva il valore {00000000-0000-0000-0000-000000000000} per il suo provider di firma predefinito e {000CD6A4-0000-0000-C000-000000000046} per il suo provider di firma per le lingue dell'Est asiatico. Il GUID del provider aggiuntivamente installato deve essere ottenuto dalla documentazione fornita con il provider.

### Esempi

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
            // Crea un certificato autofirmato
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

            // Crea una cartella di lavoro e aggiungi una riga di firma
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Aggiungi un'immagine fittizia con la riga di firma
            using (var ms = new MemoryStream())
            {
                ms.Write(new byte[] { 0x42, 0x4D, 0x1E, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x1A, 0x00, 0x00, 0x00 }, 0, 14);
                ms.Position = 0;
                
                int idx = ws.Pictures.Add(0, 0, ms);
                Picture pic = ws.Pictures[idx];
                pic.SignatureLine = new SignatureLine();
                pic.SignatureLine.ProviderId = Guid.NewGuid();
            }

            // Crea firma digitale
            var signature = new DigitalSignature(certificate, "Aspose ProviderId Demo", DateTime.Now);
            signature.ProviderId = ws.Pictures[0].SignatureLine.ProviderId;

            // Imposta la firma digitale e salva
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

### Vedi anche

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


