---
title: "DigitalSignature.Certificate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DigitalSignature-Eigenschaft. Zertifikatsobjekt, das zum Signieren des Dokuments verwendet wurde"
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignature/certificate/
---
## DigitalSignature.Certificate property

Zertifikatsobjekt, das zum Signieren des Dokuments verwendet wurde.

```csharp
public X509Certificate2 Certificate { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturePropertyCertificateDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle ein Zertifikat (im realen Szenario würdest du ein tatsächliches Zertifikat laden)
            // Dies ist nur zur Demonstration – wird für das tatsächliche Signieren nicht gültig sein
            X509Certificate2 certificate = new X509Certificate2();
            
            // Erstelle eine digitale Signatur mit dem Zertifikat
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Test signature", 
                DateTime.Now);
            
            // Zeige aktuelle Zertifikatsinformationen an
            Console.WriteLine("Current Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("Current Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Erstelle eine Sammlung und füge die Signatur hinzu
            DigitalSignatureCollection signatureCollection = new DigitalSignatureCollection();
            signatureCollection.Add(signature);
            
            // Füge die Signaturen zum Arbeitsbuch hinzu
            workbook.AddDigitalSignature(signatureCollection);
            
            // Erstelle ein neues Zertifikat (simuliert)
            X509Certificate2 newCertificate = new X509Certificate2();
            
            // Ändere die Zertifikatseigenschaft
            signature.Certificate = newCertificate;
            
            // Zeige neue Zertifikatsinformationen an
            Console.WriteLine("New Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("New Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Die Arbeitsmappe mit digitaler Signatur speichern
            workbook.Save("DigitalSignatureWithCertificate.xlsx");
        }
    }
}
```

### Siehe auch

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


