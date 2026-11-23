---
title: "Cells.HideColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Masque une colonne"
type: docs
url: /fr/net/aspose.cells/cells/hidecolumn/
---
## Cells.HideColumn method

Masque une colonne.

```csharp
public void HideColumn(int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Index de colonne. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définissez des données dans la colonne que nous allons masquer
            cells["B1"].PutValue("This column will be hidden");
            cells["B2"].PutValue(123.45);

            // Masquez la colonne B (index 1)
            cells.HideColumn(1);

            // Affichez la colonne avec la largeur standard
            cells.UnhideColumn(1, cells.StandardWidth);

            // Enregistrez le classeur
            workbook.Save("HideColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


