---
title: "Cells.SetColumnWidthInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Définit la largeur de colonne en unités de pouces en vue normale"
type: docs
url: /fr/net/aspose.cells/cells/setcolumnwidthinch/
---
## Cells.SetColumnWidthInch method

Définit la largeur de la colonne en pouces en mode normal.

```csharp
public void SetColumnWidthInch(int column, double inches)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Index de colonne. |
| pouces | Double | Nombre de pouces. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définissez les largeurs de colonne en pouces
            cells.SetColumnWidthInch(0, 2.0);
            cells.SetColumnWidthInch(1, 1.5);
            cells.SetColumnWidthInch(2, 0.8);

            // Définissez des données dans les cellules pour rendre le fichier visible
            cells["A1"].PutValue("Column A (2 inches)");
            cells["B1"].PutValue("Column B (1.5 inches)");
            cells["C1"].PutValue("Column C (0.8 inches)");

            // Enregistrez le classeur
            workbook.Save("ColumnWidthsInInches.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


