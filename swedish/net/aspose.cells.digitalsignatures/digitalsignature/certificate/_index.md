---
title: "DigitalSignature.Certificate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignature-egenskap. Certifikatobjekt som användes för att signera dokumentet"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/certificate/
---
## DigitalSignature.Certificate property

Certifikatobjekt som användes för att signera dokumentet.

```csharp
public X509Certificate2 Certificate { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa ett certifikat (i ett riktigt scenario skulle du läsa in ett faktiskt certifikat)
            // Detta är bara för demonstration - kommer inte vara giltigt för faktisk signering
            X509Certificate2 certificate = new X509Certificate2();
            
            // Skapa en digital signatur med certifikatet
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Test signature", 
                DateTime.Now);
            
            // Visa aktuell certifikatinformation
            Console.WriteLine("Current Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("Current Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Skapa en samling och lägg till signaturen i den
            DigitalSignatureCollection signatureCollection = new DigitalSignatureCollection();
            signatureCollection.Add(signature);
            
            // Lägg till signaturerna i arbetsboken
            workbook.AddDigitalSignature(signatureCollection);
            
            // Skapa ett nytt certifikat (simulerat)
            X509Certificate2 newCertificate = new X509Certificate2();
            
            // Ändra certifikategenskapen
            signature.Certificate = newCertificate;
            
            // Visa ny certifikatinformation
            Console.WriteLine("New Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("New Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Spara arbetsboken med digital signatur
            workbook.Save("DigitalSignatureWithCertificate.xlsx");
        }
    }
}
```

### Se även

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


