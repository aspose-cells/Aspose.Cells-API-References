---
title: "Cell.Row"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient le numéro de ligne zéro basé sur la cellule"
type: docs
url: /fr/net/aspose.cells/cell/row/
---
## Cell.Row property

Obtient le numéro de ligne (à partir de zéro) de la cellule.

```csharp
public int Row { get; }
```

### Property Value

Numéro de ligne Cell

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple et une formule
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Trouver la cellule contenant la formule
            Cell cell = worksheet.Cells.Find("=SUM(A1", null, new FindOptions()
            { 
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains 
            });
            
            // Démontrez la propriété Row
            Console.WriteLine("Formula found in row: " + cell.Row);
            Console.WriteLine("Formula found in column: " + cell.Column);
            
            // Vérifier que la ligne est correcte
            if (cell.Row == 2 && cell.Column == 0)
            {
                Console.WriteLine("Row property works correctly");
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


