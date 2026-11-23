---
title: "DigitalSignature.Id"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DigitalSignature. Spécifie un GUID qui peut être référencé avec le GUID de la ligne de signature stockée dans le contenu du document. La valeur par défaut est un GUID vide composé de zéros"
type: docs
url: /fr/net/aspose.cells.digitalsignatures/digitalsignature/id/
---
## DigitalSignature.Id property

Spécifie un GUID qui peut être référencé en croix avec le GUID de la ligne de signature stockée dans le contenu du document. La valeur par défaut est Empty (tous les zéros) Guid.

```csharp
public Guid Id { get; set; }
```

### Remarques

Lorsqu'il est défini, il associe [`SignatureLine`](../../../aspose.cells.drawing/signatureline/) à la [`DigitalSignature`](../) correspondante.

### Exemples

```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une signature numérique avec un ID spécifique
            Guid signatureId = Guid.NewGuid();
            
            // Créez une signature numérique
            X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            
            // Définir l'ID de la signature
            signature.Id = signatureId;

            // Ajouter la signature à la collection
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Appliquer la signature numérique au classeur
            workbook.SetDigitalSignature(dsCollection);

            // Enregistrez le classeur
            workbook.Save("signed_workbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


