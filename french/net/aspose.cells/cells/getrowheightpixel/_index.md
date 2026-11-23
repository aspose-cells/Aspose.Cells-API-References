---
title: "Cells.GetRowHeightPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient la hauteur d'une ligne spécifiée en unité de pixel"
type: docs
url: /fr/net/aspose.cells/cells/getrowheightpixel/
---
## Cells.GetRowHeightPixel method

Obtient la hauteur d'une ligne spécifiée en unité de pixel.

```csharp
public int GetRowHeightPixel(int row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne |

### Valeur de retour

Hauteur de la ligne

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightPixelWithInt32Demo
    {
        public static void Run()
        {
            // Instanciez un nouveau classeur
            Workbook wb = new Workbook();

            // Obtenir la première feuille de calcul
            Worksheet worksheet = wb.Worksheets[0];

            // Définir la hauteur de la ligne 5 (en pixels)
            worksheet.Cells.SetRowHeightPixel(5, 30);

            // Obtenir la hauteur de la ligne 5 (en pixels)
            int rowHeight = worksheet.Cells.GetRowHeightPixel(5);

            Console.WriteLine("Row height of row 5 in pixels: " + rowHeight);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


