---
title: "Cells.GetCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient l’élément Cell ou null à l’indice de ligne et de colonne de cellule spécifiés"
type: docs
url: /fr/net/aspose.cells/cells/getcell/
---
## Cells.GetCell method

Obtient l’élément [`Cell`](../../cell/) ou null à l’indice de ligne et de colonne de cellule spécifiés.

```csharp
[Obsolete("Use Cells.CheckCell(int row, int column) instead.")]
public Cell GetCell(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne |
| column | Int32 | Indice de colonne |

### Valeur de retour

Renvoie l’objet Cell si un objet Cell existe. Renvoie null si la cellule n’existe pas.

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode CheckCell(int row, int column). Cette méthode sera supprimée 12 mois plus tard, depuis février 2024. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la cellule à la ligne 1, colonne 2 (indice basé sur 0)
            Cell cell = worksheet.Cells.GetCell(1, 2);
            
            // Définir la valeur et le style à des fins de démonstration
            cell.PutValue("Test Value");
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("GetCellDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


