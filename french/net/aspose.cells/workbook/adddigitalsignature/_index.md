---
title: "Workbook.AddDigitalSignature"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Ajoute une signature numérique à un fichier de feuille de calcul OOXML Excel2007 et versions ultérieures"
type: docs
url: /fr/net/aspose.cells/workbook/adddigitalsignature/
---
## Workbook.AddDigitalSignature method

Ajoute une signature numérique à un fichier de feuille de calcul OOXML (Excel2007 et versions ultérieures).

```csharp
public void AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Remarques

Prend uniquement en charge l’ajout de la signature numérique Xmldsig à un fichier de feuille de calcul OOXML

### Exemples

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAddDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature");

            // Charger le certificat (remplacez par le chemin et le mot de passe de votre propre certificat)
            X509Certificate2 certificate = new X509Certificate2("DrWatson.pfx", "1234567890");

            // Créer une signature numérique
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);

            // Créer une collection de signatures numériques et ajouter une signature
            DigitalSignatureCollection digitalSignatureCollection = new DigitalSignatureCollection();
            digitalSignatureCollection.Add(digitalSignature);

            // Ajouter une signature numérique au classeur
            workbook.AddDigitalSignature(digitalSignatureCollection);

            // Enregistrez le classeur
            workbook.Save("DigitallySignedWorkbook.xlsx");
        }
    }
}
```

### Voir aussi

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


