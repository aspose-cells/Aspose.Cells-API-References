---
title: "Cells.CheckCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient l’élément Cell ou null à l’indice de ligne et de colonne de cellule spécifiés"
type: docs
url: /fr/net/aspose.cells/cells/checkcell/
---
## Cells.CheckCell method

Obtient l’élément [`Cell`](../../cell/) ou null à l’indice de ligne et de colonne de cellule spécifiés.

```csharp
public Cell CheckCell(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne |
| column | Int32 | Indice de colonne |

### Valeur de retour

Renvoie l’objet Cell si un objet Cell existe. Renvoie null si la cellule n’existe pas.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir les valeurs dans les cellules
            cells[0, 0].PutValue("Hello");
            cells[1, 1].PutValue(123);
            cells[2, 2].PutValue(DateTime.Now);

            // Vérifier les cellules en utilisant la méthode CheckCell avec des paramètres Int32
            Cell cell1 = cells.CheckCell(0, 0);
            Console.WriteLine("Cell A1 value: " + cell1.StringValue);

            Cell cell2 = cells.CheckCell(1, 1);
            Console.WriteLine("Cell B2 value: " + cell2.StringValue);

            Cell cell3 = cells.CheckCell(2, 2);
            Console.WriteLine("Cell C3 value: " + cell3.StringValue);

            // Vérifier une cellule inexistante (renverra null)
            Cell cell4 = cells.CheckCell(10, 10);
            if (cell4 == null)
            {
                Console.WriteLine("Cell K11 doesn't exist (as expected)");
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


