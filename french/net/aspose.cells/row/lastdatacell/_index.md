---
title: "Row.LastDataCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Row. Obtient la dernière cellule non vide de la ligne"
type: docs
url: /fr/net/aspose.cells/row/lastdatacell/
---
## Row.LastDataCell property

Obtient la dernière cellule non vide de la ligne.

```csharp
public Cell LastDataCell { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Insérer des données dans les cellules
            cells["A1"].PutValue("First cell");
            cells["B1"].PutValue("Second cell");
            cells["C2"].PutValue("Not in first row");
            
            // Obtenir la dernière cellule de données de la première ligne
            Cell lastDataCell = cells.Rows[0].LastDataCell;
            
            Console.WriteLine("Last data cell in first row: " + lastDataCell.Name);
            Console.WriteLine("Value in last data cell: " + lastDataCell.StringValue);
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


