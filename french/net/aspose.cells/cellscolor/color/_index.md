---
title: "CellsColor.Color"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsColor. Obtient et définit la couleur RVB"
type: docs
url: /fr/net/aspose.cells/cellscolor/color/
---
## CellsColor.Color property

Obtient et définit la couleur RVB.

```csharp
public Color Color { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage et définir des bordures colorées
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical, CellBorderType.Thin, color);

            // Vérifier les paramètres de bordure dans une cellule
            Cell cell = worksheet.Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            // Enregistrez le classeur
            workbook.Save("CellsColorPropertyColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


