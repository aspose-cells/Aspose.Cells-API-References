---
title: "Row.GetCellByIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Row. Obtient la cellule à un indice spécifique dans la collection de cellules de cette ligne"
type: docs
url: /fr/net/aspose.cells/row/getcellbyindex/
---
## Row.GetCellByIndex method

Obtenez la cellule par un index spécifique dans la collection de cellules de cette ligne.

```csharp
public Cell GetCellByIndex(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'index (position) de la cellule dans la collection de cellules de cette ligne. |

### Valeur de retour

L'objet Cell à la position donnée.

### Remarques

Pour parcourir toutes les cellules séquentiellement sans modification, utiliser [`GetEnumerator`](../getenumerator/) offrira de meilleures performances que d'utiliser cette méthode pour obtenir les cellules une par une.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données aux cellules de la première ligne
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            // Obtenir la première ligne
            Row row = worksheet.Cells.Rows[0];

            // Démontrer GetCellByIndex avec le paramètre Int32
            Cell cellAtIndex0 = row.GetCellByIndex(0);
            Cell cellAtIndex1 = row.GetCellByIndex(1);
            Cell cellAtIndex2 = row.GetCellByIndex(2);

            Console.WriteLine("Cell at index 0: " + cellAtIndex0.StringValue);
            Console.WriteLine("Cell at index 1: " + cellAtIndex1.StringValue);
            Console.WriteLine("Cell at index 2: " + cellAtIndex2.StringValue);

            workbook.Save("RowGetCellByIndexDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


