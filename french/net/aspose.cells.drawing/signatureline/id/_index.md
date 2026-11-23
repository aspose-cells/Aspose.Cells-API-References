---
title: "SignatureLine.Id"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SignatureLine. Obtient ou définit l'identifiant de cette ligne de signature"
type: docs
url: /fr/net/aspose.cells.drawing/signatureline/id/
---
## SignatureLine.Id property

Obtient ou définit l'identifiant de cette ligne de signature.

```csharp
public Guid Id { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un objet de ligne de signature
            SignatureLine signatureLine = new SignatureLine();
            Guid signatureId = Guid.NewGuid();
            signatureLine.Id = signatureId;
            
            // Ajouter la ligne de signature à la feuille de calcul à la position (1,1)
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Afficher l'ID de la ligne de signature
            Console.WriteLine("Signature Line ID: " + signatureLine.Id);
        }
    }
}
```

### Voir aussi

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


