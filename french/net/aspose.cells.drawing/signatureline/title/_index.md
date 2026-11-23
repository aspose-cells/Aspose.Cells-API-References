---
title: "SignatureLine.Title"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SignatureLine. Obtient ou définit le titre du signataire"
type: docs
url: /fr/net/aspose.cells.drawing/signatureline/title/
---
## SignatureLine.Title property

Obtient ou définit le titre du chanteur.

```csharp
public string Title { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyTitleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une ligne de signature et définir son titre
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Title = "Development Lead";

            // Ajouter la ligne de signature aux formes de la feuille de calcul avec les paramètres de position
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Afficher le titre pour démontrer que la propriété a été définie
            Console.WriteLine("Signature Line Title: " + signatureLine.Title);
        }
    }
}
```

### Voir aussi

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


