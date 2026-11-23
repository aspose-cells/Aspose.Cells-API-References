---
title: "Cells.SetRowHeightPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Définit la hauteur de la ligne en unités de pixels"
type: docs
url: /fr/net/aspose.cells/cells/setrowheightpixel/
---
## Cells.SetRowHeightPixel method

Définit la hauteur de la ligne en unités de pixels.

```csharp
public void SetRowHeightPixel(int row, int pixels)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Index de ligne. |
| pixels | Int32 | Nombre de pixels. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définissez la hauteur de la première ligne à 50 pixels
            worksheet.Cells.SetRowHeightPixel(0, 50);

            // Définissez la hauteur de la deuxième ligne à 100 pixels
            worksheet.Cells.SetRowHeightPixel(1, 100);

            // Enregistrez le classeur
            workbook.Save("RowHeightPixelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


