---
title: "VbaProject.Sign"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode VbaProject. Signer ce projet VBA avec une DigitalSignature"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/sign/
---
## VbaProject.Sign method

Signe ce projet VBA avec une DigitalSignature

```csharp
public void Sign(DigitalSignature digitalSignature)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |

### Exemples

```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.Vba;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodSignWithDigitalSignatureDemo
    {
        public static void Run()
        {
            // Chargez le classeur avec le projet VBA
            Workbook workbook = new Workbook("SignXlsm.xlsm");
            
            // Obtenir le projet VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            if (vbaProject != null)
            {
                // Charger le certificat depuis le fichier
                X509Certificate2 certificate = new X509Certificate2("YourCertificate.pfx", "password");
                
                // Créez une signature numérique
                DigitalSignature certSign = new DigitalSignature(certificate, "Test Signing", DateTime.Now);
                
                // Signer le projet VBA
                vbaProject.Sign(certSign);
                
                // Enregistrer le classeur signé
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsm);
                    
                    // Vérifier la signature
                    Workbook verifyWorkbook = new Workbook(stream);
                    Console.WriteLine("Is Signed: " + verifyWorkbook.VbaProject.IsSigned);
                    Console.WriteLine("Is Valid Signed: " + verifyWorkbook.VbaProject.IsValidSigned);
                }
            }
        }
    }
}
```

### Voir aussi

* class [DigitalSignature](../../../aspose.cells.digitalsignatures/digitalsignature/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


