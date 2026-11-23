---
title: "Classe DigitalSignatureCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.DigitalSignatures.DigitalSignatureCollection. Fournit une collection de signatures numériques attachées à un document"
type: docs
url: /fr/net/aspose.cells.digitalsignatures/digitalsignaturecollection/
---
## DigitalSignatureCollection class

Fournit une collection de signatures numériques attachées à un document.

```csharp
public class DigitalSignatureCollection : IEnumerable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DigitalSignatureCollection](digitalsignaturecollection/)() | Le constructeur de DigitalSignatureCollection. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.digitalsignatures/digitalsignaturecollection/add/)(DigitalSignature) | Ajoutez une signature à DigitalSignatureCollection. |
| [GetEnumerator](../../aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/)() | Obtenez l'énumérateur pour DigitalSignatureCollection, cet énumérateur permet d'itérer sur la collection |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignatureCollectionDemo
    {
        public static void DigitalSignatureCollectionExample()
        {
            // Chargez un classeur à partir d'un fichier source signé
            Workbook signedWorkbook = new Workbook(@"DigitalSignatureCollection_original.xlsx");

            // Vérifier si le classeur est signé numériquement
            Console.WriteLine("Is the workbook digitally signed? " + signedWorkbook.IsDigitallySigned);

            // Obtenez la collection de signatures numériques du classeur
            DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();

            if (existingDsc != null)
            {
                // Itérez sur les signatures numériques de la collection
                foreach (DigitalSignature existingDs in existingDsc)
                {
                    Console.WriteLine("Comments: " + existingDs.Comments);
                    Console.WriteLine("Sign Time: " + existingDs.SignTime);
                    Console.WriteLine("Is Valid: " + existingDs.IsValid);
                }

                // Créez une nouvelle signature numérique
                X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "password");
                DigitalSignature newSignature = new DigitalSignature(certificate, "New signature comment", DateTime.Now);

                // Ajoutez la nouvelle signature numérique à la collection
                existingDsc.Add(newSignature);
            }     
            

            // Enregistrez le classeur avec la nouvelle signature numérique
            signedWorkbook.Save("DigitalSignatureCollectionExample.xlsx");
            signedWorkbook.Save("DigitalSignatureCollectionExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


