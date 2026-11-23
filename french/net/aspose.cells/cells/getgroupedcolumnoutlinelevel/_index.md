---
title: "Cells.GetGroupedColumnOutlineLevel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient le niveau de contour (index zéro) de la colonne"
type: docs
url: /fr/net/aspose.cells/cells/getgroupedcolumnoutlinelevel/
---
## Cells.GetGroupedColumnOutlineLevel method

Obtient le niveau de contour (à base zéro) de la colonne.

```csharp
public int GetGroupedColumnOutlineLevel(int columnIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | L'index de colonne |

### Valeur de retour

Le niveau de contour de la colonne

### Remarques

Si la colonne n'est pas groupée, renvoie zéro.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedColumnOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Regrouper les colonnes (les 3 premières colonnes) sans les masquer
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Obtenir le niveau de contour de la première colonne
            int outlineLevel = worksheet.Cells.GetGroupedColumnOutlineLevel(0);
            
            Console.WriteLine("Outline level of column 0: " + outlineLevel);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


