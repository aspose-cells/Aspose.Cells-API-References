---
title: "DigitalSignature.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DigitalSignature. Spécifie le texte de la signature réelle dans la signature numérique. La valeur par défaut est Vide"
type: docs
url: /fr/net/aspose.cells.digitalsignatures/digitalsignature/text/
---
## DigitalSignature.Text property

Spécifie le texte de la signature réelle dans la signature numérique. La valeur par défaut est Empty.

```csharp
public string Text { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturePropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un certificat de test (dans un scénario réel, utilisez un certificat valide)
            X509Certificate2 certificate = null;
            try
            {
                certificate = new X509Certificate2();
            }
            catch
            {
                Console.WriteLine("Could not create certificate. Using null for demonstration.");
            }

            // Créer une instance de signature numérique
            DigitalSignature signature = new DigitalSignature(
                certificate,
                "Sample signature comments",
                DateTime.Now);

            // Afficher la valeur actuelle de Text (la valeur par défaut est vide)
            Console.WriteLine("Current Text value: " + signature.Text);

            // Définir une nouvelle valeur pour la propriété Text
            signature.Text = "Approved by John Doe";

            // Créer une collection de signatures numériques et y ajouter la signature
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            signatures.Add(signature);

            // Ajouter les signatures numériques au classeur
            workbook.AddDigitalSignature(signatures);

            // Enregistrer le classeur avec la signature numérique
            try
            {
                workbook.Save("DigitalSignatureWithText.xlsx");
                Console.WriteLine("Workbook saved with digital signature text: " + signature.Text);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error saving workbook: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


