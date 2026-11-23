---
title: "DigitalSignature.Comments"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DigitalSignature. Le but de la signature"
type: docs
url: /fr/net/aspose.cells.digitalsignatures/digitalsignature/comments/
---
## DigitalSignature.Comments property

Le but de la signature.

```csharp
public string Comments { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyCommentsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature with Comments");

            // Créez une signature numérique avec des commentaires
            DigitalSignature signature = new DigitalSignature(
                File.ReadAllBytes("sample.pfx"), 
                "password", 
                "Sample Signature with Comments", 
                DateTime.Now)
            {
                Comments = "This is a test comment for the digital signature"
            };

            // Ajouter la signature à la collection
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Signez le classeur
            workbook.SetDigitalSignature(dsCollection);

            // Enregistrer le classeur signé
            string outputPath = "SignedWithComments.xlsx";
            workbook.Save(outputPath);

            // Vérifiez et affichez les informations de la signature
            Workbook signedWorkbook = new Workbook(outputPath);
            DigitalSignatureCollection signatures = signedWorkbook.GetDigitalSignature();

            foreach (DigitalSignature ds in signatures)
            {
                Console.WriteLine($"Comments: {ds.Comments}");
                Console.WriteLine($"Sign Time: {ds.SignTime}");
                Console.WriteLine($"Is Valid: {ds.IsValid}");
            }
        }
    }
}
```

### Voir aussi

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


