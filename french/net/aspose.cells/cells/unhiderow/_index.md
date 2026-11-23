---
title: "Cells.UnhideRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Dévoile une ligne"
type: docs
url: /fr/net/aspose.cells/cells/unhiderow/
---
## Cells.UnhideRow method

Dévoile une ligne.

```csharp
public void UnhideRow(int row, double height)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Index de ligne. |
| hauteur | Double | Hauteur de la ligne. La hauteur de la ligne ne sera modifiée que lorsque la ligne est masquée et que la valeur de hauteur fournie est positive. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Masquer la ligne 5
            worksheet.Cells.HideRow(5);
            
            // Dévoiler la ligne 5 avec une hauteur de 12.75
            worksheet.Cells.UnhideRow(5, 12.75);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


