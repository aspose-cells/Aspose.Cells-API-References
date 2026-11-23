---
title: "Row.FirstDataCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Row. Obtient la première cellule non vide de la ligne"
type: docs
url: /fr/net/aspose.cells/row/firstdatacell/
---
## Row.FirstDataCell property

Obtient la première cellule non vide de la ligne.

```csharp
public Cell FirstDataCell { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Placer des valeurs dans différentes cellules
            cells["A1"].PutValue("Header");
            cells["B2"].PutValue("FirstData");
            cells["C2"].PutValue("SecondData");
            
            // Obtenir la première cellule de données dans la ligne 1 (index 0)
            Cell firstDataCellRow1 = cells.Rows[0].FirstDataCell;
            Console.WriteLine("First data cell in row 1: " + (firstDataCellRow1 != null ? firstDataCellRow1.Name : "null"));
            
            // Obtenir la première cellule de données dans la ligne 2 (index 1)
            Cell firstDataCellRow2 = cells.Rows[1].FirstDataCell;
            Console.WriteLine("First data cell in row 2: " + firstDataCellRow2.Name);
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


