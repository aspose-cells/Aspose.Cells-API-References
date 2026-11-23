---
title: "DigitalSignature.DigitalSignature"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur DigitalSignature. Constructeur de digitalSignature. Utilise l'implémentation .Net"
type: docs
url: /fr/net/aspose.cells.digitalsignatures/digitalsignature/digitalsignature/
---
## DigitalSignature(X509Certificate2, string, DateTime) {#constructor_1}

Constructeur de digitalSignature. Utilise l'implémentation .Net.

```csharp
public DigitalSignature(X509Certificate2 certificate, string comments, DateTime signTime)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| certificat | X509Certificate2 | Objet certificat qui a été utilisé pour signer le document. |
| commentaires | String | Le but de la signature. |
| signTime | DateTime | L'heure UTC lorsque le document a été signé. |

### Exemples

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignatureMethodCtorWithX509Certificate2StringDateTimeDemo
    {
        public static void Run()
        {
            // Créez une collection de signatures numériques
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Charger le certificat avec la clé privée
            X509Certificate2 certificate = new X509Certificate2("mykey2.pfx", "123456");
            
            // Créer une signature numérique avec le certificat, le but et l'horodatage
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Document approval", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Créer un nouveau classeur et le signer
            Workbook workbook = new Workbook();
            workbook.SetDigitalSignature(signatures);
            workbook.Save("signed_document.xlsx");
        }
    }
}
```

### Voir aussi

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)

---

## DigitalSignature(byte[], string, string, DateTime) {#constructor}

Constructeur de digitalSignature. Utilise l'implémentation Bouncy Castle.

```csharp
public DigitalSignature(byte[] rawData, string password, string comments, DateTime signTime)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rawData | Byte[] | Un tableau d'octets contenant les données d'un certificat X.509. |
| mot de passe | String | Le mot de passe requis pour accéder aux données du certificat X.509. |
| commentaires | String | Le but de la signature. |
| signTime | DateTime | L'heure UTC lorsque le document a été signé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.IO;

    public class DigitalSignatureConstructorWithByteArrayStringStringDateTimeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter du contenu d'exemple
            worksheet.Cells["A1"].PutValue("Digitally Signed Document");
            
            try
            {
                // Charger le fichier de certificat en tant que tableau d'octets (remplacer par le chemin réel du certificat)
                string certPath = "certificate.pfx";
                byte[] certData = File.ReadAllBytes(certPath);
                
                // Créer les paramètres de signature numérique
                string password = "certificate_password";
                string comments = "Approved by John Doe";
                DateTime signTime = DateTime.Now;
                
                // Appeler le constructeur avec (Byte[], String, String, DateTime)
                DigitalSignature signature = new DigitalSignature(certData, password, comments, signTime);
                
                // Créer une DigitalSignatureCollection et ajouter la signature à celle-ci
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                
                // Ajouter des signatures au classeur
                workbook.AddDigitalSignature(signatures);
                
                Console.WriteLine("Digital signature added successfully with parameters (Byte[], String, String, DateTime)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("DigitalSignatureDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


