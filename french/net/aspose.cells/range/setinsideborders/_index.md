---
title: "Range.SetInsideBorders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Définit les bordures internes de la plage"
type: docs
url: /fr/net/aspose.cells/range/setinsideborders/
---
## Range.SetInsideBorders method

Définit les bordures internes de la plage.

```csharp
public void SetInsideBorders(BorderType borderEdge, CellBorderType lineStyle, 
    CellsColor borderColor)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| borderEdge | BorderType | Type de bordure interne, ne peut être que Verticale et Horizontale. |
| lineStyle | CellBorderType | Le style de bordure. |
| borderColor | CellsColor | La couleur de la bordure. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetInsideBordersWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une plage et définissez les bordures internes
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Vertical, CellBorderType.Thin, color);

            // Vérifiez les bordures dans une cellule de la plage
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            workbook.Save("SetInsideBordersExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


