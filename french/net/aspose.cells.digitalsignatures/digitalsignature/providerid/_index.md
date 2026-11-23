---
title: "DigitalSignature.ProviderId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DigitalSignature. Spécifie l'ID de classe du fournisseur de signature. La valeur par défaut est un GUID vide composé uniquement de zéros"
type: docs
url: /fr/net/aspose.cells.digitalsignatures/digitalsignature/providerid/
---
## DigitalSignature.ProviderId property

Spécifie l'ID de classe du fournisseur de signature. La valeur par défaut est Empty (tous les zéros) Guid.

```csharp
public Guid ProviderId { get; set; }
```

### Remarques

Le fournisseur de services cryptographiques (CSP) est un module logiciel indépendant qui exécute réellement les algorithmes de cryptographie pour l'authentification, le codage et le chiffrement. Microsoft Office réserve la valeur {00000000-0000-0000-0000-000000000000} pour son fournisseur de signature par défaut, et {000CD6A4-0000-0000-C000-000000000046} pour son fournisseur de signature asiatique. Le GUID du fournisseur installé en supplément doit être obtenu dans la documentation fournie avec le fournisseur.

### Exemples

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
            // Créez un certificat auto-signé
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

            // Créez un classeur et ajoutez une ligne de signature
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Ajoutez une image factice avec une ligne de signature
            using (var ms = new MemoryStream())
            {
                ms.Write(new byte[] { 0x42, 0x4D, 0x1E, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x1A, 0x00, 0x00, 0x00 }, 0, 14);
                ms.Position = 0;
                
                int idx = ws.Pictures.Add(0, 0, ms);
                Picture pic = ws.Pictures[idx];
                pic.SignatureLine = new SignatureLine();
                pic.SignatureLine.ProviderId = Guid.NewGuid();
            }

            // Créer une signature numérique
            var signature = new DigitalSignature(certificate, "Aspose ProviderId Demo", DateTime.Now);
            signature.ProviderId = ws.Pictures[0].SignatureLine.ProviderId;

            // Définissez la signature numérique et enregistrez
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

### Voir aussi

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


