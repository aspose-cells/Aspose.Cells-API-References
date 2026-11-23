---
title: "DigitalSignature.Certificate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DigitalSignature. Objet certificat qui a été utilisé pour signer le document"
type: docs
url: /fr/net/aspose.cells.digitalsignatures/digitalsignature/certificate/
---
## DigitalSignature.Certificate property

Objet certificat qui a été utilisé pour signer le document.

```csharp
public X509Certificate2 Certificate { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer un certificat (dans un scénario réel, vous chargeriez un certificat réel)
            // Ceci est uniquement à titre de démonstration - ne sera pas valide pour une signature réelle
            X509Certificate2 certificate = new X509Certificate2();
            
            // Créer une signature numérique avec le certificat
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Test signature", 
                DateTime.Now);
            
            // Afficher les informations actuelles du certificat
            Console.WriteLine("Current Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("Current Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Créer une collection et y ajouter la signature
            DigitalSignatureCollection signatureCollection = new DigitalSignatureCollection();
            signatureCollection.Add(signature);
            
            // Ajouter les signatures au classeur
            workbook.AddDigitalSignature(signatureCollection);
            
            // Créer un nouveau certificat (simulé)
            X509Certificate2 newCertificate = new X509Certificate2();
            
            // Modifier la propriété du certificat
            signature.Certificate = newCertificate;
            
            // Afficher les informations du nouveau certificat
            Console.WriteLine("New Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("New Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Enregistrer le classeur avec la signature numérique
            workbook.Save("DigitalSignatureWithCertificate.xlsx");
        }
    }
}
```

### Voir aussi

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


