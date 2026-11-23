---
title: "Cells.SetRowHeight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Définit la hauteur de la ligne spécifiée"
type: docs
url: /fr/net/aspose.cells/cells/setrowheight/
---
## Cells.SetRowHeight method

Définit la hauteur de la ligne spécifiée.

```csharp
public void SetRowHeight(int row, double height)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Index de ligne. |
| hauteur | Double | Hauteur de la ligne. En unité de point, elle doit être comprise entre 0 et 409,5. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définissez la hauteur de la première ligne (indice 0) à 25,5 points
            cells.SetRowHeight(0, 25.5);

            // Vérifiez la hauteur de la ligne
            Console.WriteLine("Row height of row 0: " + cells.GetRowHeight(0));
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


