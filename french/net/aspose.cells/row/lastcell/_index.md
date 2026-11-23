---
title: "Row.LastCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Row. Obtient le dernier objet cellule de la ligne"
type: docs
url: /fr/net/aspose.cells/row/lastcell/
---
## Row.LastCell property

Obtient le dernier objet cellule de la ligne.

```csharp
public Cell LastCell { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("First");
            worksheet.Cells["B1"].PutValue("Second");
            worksheet.Cells["C1"].PutValue("Last");

            // Obtenir la première ligne
            Row row = worksheet.Cells.Rows[0];

            // Accéder à la dernière cellule de la ligne
            Cell lastCell = row.LastCell;
            
            // Afficher la valeur de la dernière cellule
            Console.WriteLine("Last cell value: " + lastCell.Value);
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


