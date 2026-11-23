---
title: "SignatureLine.Instructions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SignatureLine. Obtient ou définit le texte affiché à l'utilisateur lors de la signature."
type: docs
url: /fr/net/aspose.cells.drawing/signatureline/instructions/
---
## SignatureLine.Instructions property

Obtient ou définit le texte affiché à l'utilisateur lors de la signature.

```csharp
public string Instructions { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyInstructionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un objet de ligne de signature
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Instructions = "Please sign here after reviewing the document.";

            // Ajouter la ligne de signature à la feuille de calcul à la position (1,1)
            worksheet.Shapes.AddSignatureLine(1, 1, signatureLine);

            // Enregistrez le classeur
            workbook.Save("SignatureLineDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


