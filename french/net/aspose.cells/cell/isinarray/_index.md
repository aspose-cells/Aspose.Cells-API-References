---
title: "Cell.IsInArray"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si la formule de la cellule est une formule de tableau"
type: docs
url: /fr/net/aspose.cells/cell/isinarray/
---
## Cell.IsInArray property

Indique si la formule de la cellule est une formule matricielle.

```csharp
[Obsolete("Use IsArrayFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInArray { get; }
```

### Remarques

NOTE: Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.IsArrayFormula pour vérifier si la formule de la cellule est une formule de tableau. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2018. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsInArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple avec des formules de tableau
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Définir une formule de tableau en utilisant l'API correcte
            worksheet.Cells["C2"].SetArrayFormula("A2:A3*B2:B3", 2, 1);

            // Vérifier la propriété IsInArray
            Cell cellInArray = worksheet.Cells["C2"];
            Cell cellNotInArray = worksheet.Cells["A2"];

            Console.WriteLine("Cell C2 is in array: " + cellInArray.IsInArray);
            Console.WriteLine("Cell A2 is in array: " + cellNotInArray.IsInArray);

            // Démontrer le nettoyage des cellules non tableau
            for (int row = 1; row <= 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = worksheet.Cells[row, col];
                    if (!cell.IsInArray && !cell.IsFormula)
                    {
                        cell.PutValue("");
                    }
                }
            }

            // Enregistrez le classeur
            workbook.Save("IsInArrayDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


