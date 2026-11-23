---
title: "Workbook.SetDigitalSignature"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Définit la signature numérique d'un fichier feuille de calcul Excel2007 et versions ultérieures"
type: docs
url: /fr/net/aspose.cells/workbook/setdigitalsignature/
---
## Workbook.SetDigitalSignature method

Applique une signature numérique à un fichier de feuille de calcul (Excel2007 et versions ultérieures).

```csharp
public void SetDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Remarques

Prise en charge uniquement de l'ajout de la signature numérique Xmldsig

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Chemin du répertoire source
            string sourceDir = "SourceDirectory/";
            
            // Chemin du répertoire de sortie
            string outputDir = "OutputDirectory/";

            // Chargez le classeur
            Workbook workbook = new Workbook(sourceDir + "TestCert.xlsx");

            // Créer une collection de signatures numériques
            DigitalSignatureCollection digitalSignatures = new DigitalSignatureCollection();

            // Charger le fichier de certificat
            string certPath = sourceDir + "certs\\sample.pfx";
            byte[] certData = File.ReadAllBytes(certPath);

            // Créer une signature numérique
            DigitalSignature signature = new DigitalSignature(certData, "1234567890", "Sample Signer", DateTime.Now);

            // Ajouter la signature à la collection
            digitalSignatures.Add(signature);

            // Définir la signature numérique du classeur
            workbook.SetDigitalSignature(digitalSignatures);

            // Enregistrez le classeur
            workbook.Save(outputDir + "DigitallySignedWorkbook.xlsx");

            Console.WriteLine("Digital signature set successfully.");
        }
    }
}
```

### Voir aussi

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


