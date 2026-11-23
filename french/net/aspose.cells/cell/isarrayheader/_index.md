---
title: "Cell.IsArrayHeader"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique que la formule de la cellule est une formule de tableau et qu'elle est la première cellule du tableau"
type: docs
url: /fr/net/aspose.cells/cell/isarrayheader/
---
## Cell.IsArrayHeader property

Indique que la formule de la cellule est une formule de tableau et qu'elle est la première cellule du tableau.

```csharp
public bool IsArrayHeader { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayHeaderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une formule de tableau dans la plage B2:D4
            worksheet.Cells["B2"].SetArrayFormula("=A1:A3*B1:B3", 3, 3);
            
            // Vérifier et afficher la propriété IsArrayHeader
            // Remarque : IsArrayHeader est en lecture seule et est automatiquement défini pour les en-têtes de formules de tableau
            Console.WriteLine("B2 IsArrayHeader: " + worksheet.Cells["B2"].IsArrayHeader);
            Console.WriteLine("B3 IsArrayHeader: " + worksheet.Cells["B3"].IsArrayHeader);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


