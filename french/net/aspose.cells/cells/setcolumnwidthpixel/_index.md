---
title: "Cells.SetColumnWidthPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Définit la largeur de colonne en unités de pixels en vue normale"
type: docs
url: /fr/net/aspose.cells/cells/setcolumnwidthpixel/
---
## Cells.SetColumnWidthPixel method

Définit la largeur de la colonne en pixels en mode normal.

```csharp
public void SetColumnWidthPixel(int column, int pixels)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Index de colonne. |
| pixels | Int32 | Nombre de pixels. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définissez les largeurs de colonnes en pixels pour les colonnes 1 à 5
            for (int i = 0; i < 5; i++)
            {
                cells.SetColumnWidthPixel(i, 120); // 120 pixels width
            }

            // Enregistrez le classeur
            workbook.Save("SetColumnWidthPixelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


