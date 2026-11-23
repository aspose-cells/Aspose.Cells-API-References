---
title: "SignatureLine.Signer"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SignatureLine. Obtient ou définit le signataire"
type: docs
url: /fr/net/aspose.cells.drawing/signatureline/signer/
---
## SignatureLine.Signer property

Obtient ou définit le signataire.

```csharp
public string Signer { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertySignerDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une ligne de signature et définir ses propriétés
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";

            // Ajouter la ligne de signature à la feuille de calcul à la ligne 1, colonne 1
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

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


