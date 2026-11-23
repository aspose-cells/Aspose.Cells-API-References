---
title: "Cells.UnhideColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Démasque une colonne"
type: docs
url: /fr/net/aspose.cells/cells/unhidecolumn/
---
## Cells.UnhideColumn method

Dévoile une colonne

```csharp
public void UnhideColumn(int column, double width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Index de colonne. |
| largeur | Double | Largeur de colonne. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideColumnWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Masquer la colonne 2
            cells.HideColumn(2);
            
            // Afficher la colonne 2 avec ajustement de largeur (-1 signifie utiliser la largeur standard)
            cells.UnhideColumn(2, -1);
            
            Console.WriteLine("Column 2 width after unhiding: " + cells.Columns[2].Width);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


