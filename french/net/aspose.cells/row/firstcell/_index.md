---
title: "Row.FirstCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Row. Obtient le premier objet cellule de la ligne"
type: docs
url: /fr/net/aspose.cells/row/firstcell/
---
## Row.FirstCell property

Obtient le premier objet cellule de la ligne.

```csharp
public Cell FirstCell { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données aux cellules de la première ligne
            worksheet.Cells["A1"].PutValue("First Cell");
            worksheet.Cells["B1"].PutValue("Second Cell");
            worksheet.Cells["C1"].PutValue("Third Cell");
            
            // Obtenir la première ligne
            Row row = worksheet.Cells.Rows[0];
            
            // Démontrer la propriété FirstCell
            Cell firstCell = row.FirstCell;
            Console.WriteLine("First cell in row: " + firstCell.Name + " with value: " + firstCell.StringValue);
            
            // Modifier la première cellule
            firstCell.PutValue("Modified First Cell");
            Console.WriteLine("Updated first cell value: " + firstCell.StringValue);
            
            // Enregistrez le classeur
            workbook.Save("RowFirstCellDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


