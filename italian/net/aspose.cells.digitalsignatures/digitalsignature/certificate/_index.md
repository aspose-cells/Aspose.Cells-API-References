---
title: "DigitalSignature.Certificate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DigitalSignature. Oggetto certificato utilizzato per firmare il documento"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignature/certificate/
---
## DigitalSignature.Certificate property

Oggetto certificato utilizzato per firmare il documento.

```csharp
public X509Certificate2 Certificate { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea un certificato (in uno scenario reale, dovresti caricare un certificato reale)
            // Questo è solo a scopo dimostrativo - non sarà valido per una firma reale
            X509Certificate2 certificate = new X509Certificate2();
            
            // Crea una firma digitale con il certificato
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Test signature", 
                DateTime.Now);
            
            // Visualizza le informazioni attuali del certificato
            Console.WriteLine("Current Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("Current Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Crea una raccolta e aggiungi la firma ad essa
            DigitalSignatureCollection signatureCollection = new DigitalSignatureCollection();
            signatureCollection.Add(signature);
            
            // Aggiungi le firme alla cartella di lavoro
            workbook.AddDigitalSignature(signatureCollection);
            
            // Crea un nuovo certificato (simulato)
            X509Certificate2 newCertificate = new X509Certificate2();
            
            // Modifica la proprietà del certificato
            signature.Certificate = newCertificate;
            
            // Visualizza le informazioni del nuovo certificato
            Console.WriteLine("New Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("New Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Salva la cartella di lavoro con firma digitale
            workbook.Save("DigitalSignatureWithCertificate.xlsx");
        }
    }
}
```

### Vedi anche

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


