---
title: "Cells.CheckColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient l'élément Column ou null à l'index de colonne spécifié"
type: docs
url: /fr/net/aspose.cells/cells/checkcolumn/
---
## Cells.CheckColumn method

Obtient l'élément [`Column`](../../column/) ou null à l'index de colonne spécifié.

```csharp
public Column CheckColumn(int columnIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | L'index de colonne. |

### Valeur de retour

L'objet Column.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Définir une valeur dans la colonne 1 (B3)
            cells["B3"].PutValue("Sample Data");
            
            // Vérifier la colonne 4 (colonne E)
            Column column = cells.CheckColumn(4);
            
            // Afficher les propriétés de la colonne
            Console.WriteLine("Column Width: " + column.Width);
            Console.WriteLine("Column Index: " + column.Index);
        }
    }
}
```

### Voir aussi

* class [Column](../../column/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


