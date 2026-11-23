---
title: "CellsHelper.CellIndexToName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Obtient le nom de la cellule selon ses indices de ligne et de colonne"
type: docs
url: /fr/net/aspose.cells/cellshelper/cellindextoname/
---
## CellsHelper.CellIndexToName method

Obtient le nom de la cellule selon ses indices de ligne et de colonne.

```csharp
public static string CellIndexToName(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Index de ligne. |
| column | Int32 | Index de colonne. |

### Valeur de retour

Nom de la cellule.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCellIndexToNameWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez quelques données
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);

            // Obtenez le nom de la cellule à partir des indices de ligne et de colonne
            string cellName = CellsHelper.CellIndexToName(2, 1); // Row 2, Column 1 (B3)

            // Afficher le résultat
            Console.WriteLine("Cell name for row 2, column 1 is: " + cellName);
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


