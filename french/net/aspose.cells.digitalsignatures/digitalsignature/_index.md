---
title: "Classe DigitalSignature"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.DigitalSignatures.DigitalSignature. Signature dans le fichier"
type: docs
url: /fr/net/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class

Signature dans le fichier.

```csharp
public class DigitalSignature
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DigitalSignature](digitalsignature/#constructor_1)(X509Certificate2, string, DateTime) | Constructeur de digitalSignature. Utilise l'implémentation .Net. |
| [DigitalSignature](digitalsignature/#constructor)(byte[], string, string, DateTime) | Constructeur de digitalSignature. Utilise l'implémentation Bouncy Castle. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate/) { get; set; } | Objet certificat qui a été utilisé pour signer le document. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments/) { get; set; } | Le but de la signature. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id/) { get; set; } | Spécifie un GUID qui peut être référencé en croix avec le GUID de la ligne de signature stockée dans le contenu du document. La valeur par défaut est Empty (tous les zéros) Guid. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image/) { get; set; } | Spécifie une image pour la signature numérique. La valeur par défaut est null. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid/) { get; } | Si cette signature numérique est valide et que le document n'a pas été altéré, cette valeur sera vraie. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid/) { get; set; } | Spécifie l'ID de classe du fournisseur de signature. La valeur par défaut est Empty (tous les zéros) Guid. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime/) { get; set; } | Le moment où le document a été signé. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text/) { get; set; } | Spécifie le texte de la signature réelle dans la signature numérique. La valeur par défaut est Empty. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype/) { get; set; } | Type XAdES. La valeur par défaut est None (XAdES est désactivé). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturesClassDigitalSignatureDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Digital Signature Demo");

            try
            {
                // Créer une signature numérique en utilisant le constructeur de certificat
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(
                    certificate,
                    "Document signed for approval",
                    DateTime.Now);

                // Définir des propriétés supplémentaires
                signature.Id = Guid.NewGuid();
                signature.Text = "Approved";
                signature.XAdESType = XAdESType.XAdES;

                // Ajouter la signature au classeur
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                workbook.SetDigitalSignature(signatures);

                // Afficher les informations de la signature
                Console.WriteLine($"Signature added: {signature.Comments}");
                Console.WriteLine($"Sign time: {signature.SignTime}");
                Console.WriteLine($"Signature ID: {signature.Id}");

                // Enregistrer le classeur signé
                workbook.Save("DigitalSignatureDemo.xlsx");
                Console.WriteLine("Workbook signed and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DigitalSignature: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


