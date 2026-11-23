---
title: "CellsColor.Argb"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsColor. Obtient et définit la couleur à partir d'une valeur ARGB 32 bits"
type: docs
url: /fr/net/aspose.cells/cellscolor/argb/
---
## CellsColor.Argb property

Obtient et définit la couleur à partir d'une valeur ARGB de 32 bits.

```csharp
public int Argb { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyArgbDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage et un style
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A5");
            Style style = workbook.CreateStyle();

            // Créer et configurer CellsColor en utilisant la propriété Argb
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Argb = Color.FromArgb(128, 0, 0, 255).ToArgb(); // Semi-transparent blue

            // Appliquer la couleur au style
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            
            // Appliquer le style à la plage
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Enregistrez le classeur
            workbook.Save("CellsColorArgbDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


