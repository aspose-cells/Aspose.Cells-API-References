---
title: "DeleteBlankOptions.EndIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DeleteBlankOptions. Spécifie l'index de ligne/colonne de fin, inclusif, de la plage à vérifier et à supprimer les lignes/colonnes vides. La valeur par défaut est 1 et 1 signifie la plage maximale de tous les objectscells drawings ... qui doivent être vérifiés"
type: docs
url: /fr/net/aspose.cells/deleteblankoptions/endindex/
---
## DeleteBlankOptions.EndIndex property

Spécifie l'index de fin de ligne/colonne (inclusif) de la plage à vérifier et à supprimer les lignes/colonnes vides. La valeur par défaut est -1 et -1 signifie la plage maximale de tous les objets (cellules, dessins, ...) qui doivent être vérifiés.

```csharp
public int EndIndex { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEndIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Remplissez certaines cellules avec des valeurs
            cells[0, 2].PutValue(2);
            cells[0, 5].PutValue(5);
            cells[0, 9].PutValue(9);

            // Créez des options de suppression avec une plage spécifique
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            dbo.StartIndex = 4;
            dbo.EndIndex = 7;

            // Supprimez les colonnes vides dans la plage spécifiée
            cells.DeleteBlankColumns(dbo);

            // Affichez les résultats pour démontrer l'effet de EndIndex
            Console.WriteLine("Value at C1: " + cells[0, 2].IntValue);
            Console.WriteLine("Value at F1 (originally G1): " + cells[0, 4].IntValue);
            Console.WriteLine("Value at G1 (originally K1): " + cells[0, 6].IntValue);
        }
    }
}
```

### Voir aussi

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


