---
title: "Cells.SetColumnWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Définit la largeur de la colonne spécifiée en vue normale"
type: docs
url: /fr/net/aspose.cells/cells/setcolumnwidth/
---
## Cells.SetColumnWidth method

Définit la largeur de la colonne spécifiée en mode normal.

```csharp
public void SetColumnWidth(int column, double width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Index de colonne. |
| largeur | Double | Largeur de la colonne en unité de caractères. La largeur de la colonne doit être comprise entre 0 et 255. |

### Remarques

Pour les feuilles de calcul, la largeur de colonne est mesurée en nombre de caractères correspondant à la largeur maximale d'un chiffre des nombres 0~9 tels qu'ils sont rendus avec la police du style normal.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetColumnWidth(0, 25.5);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


