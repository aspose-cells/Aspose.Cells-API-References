---
title: "Range.SetOutlineBorder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Définit une bordure de contour autour d’une plage de cellules"
type: docs
url: /fr/net/aspose.cells/range/setoutlineborder/
---
## SetOutlineBorder(BorderType, CellBorderType, CellsColor) {#setoutlineborder}

Définit la bordure extérieure autour d'une plage de cellules.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, 
    CellsColor borderColor)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| borderEdge | BorderType | Bordure. |
| borderStyle | CellBorderType | Style de bordure. |
| borderColor | CellsColor | Couleur de bordure. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer un objet CellsColor
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Créer une plage et définir la bordure droite
            Aspose.Cells.Range range = cells.CreateRange("A2:B3");
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Thin, color);

            // Créer une autre plage et définir toutes les bordures
            range = cells.CreateRange("C6:F10");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Enregistrez le classeur
            workbook.Save("SetOutlineBorderExample.xlsx");
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

---

## SetOutlineBorder(BorderType, CellBorderType, Color) {#setoutlineborder_1}

Définit la bordure extérieure autour d'une plage de cellules.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, Color borderColor)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| borderEdge | BorderType | Bordure. |
| borderStyle | CellBorderType | Style de bordure. |
| borderColor | Color | Couleur de bordure. |

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage de cellules
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:D5");

            // Définir les bordures de contour avec différents types de bordure et couleurs
            range.SetOutlineBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Medium, Color.Blue);
            range.SetOutlineBorder(BorderType.TopBorder, CellBorderType.Dashed, Color.Green);
            range.SetOutlineBorder(BorderType.BottomBorder, CellBorderType.Double, Color.Black);

            // Enregistrez le classeur
            workbook.Save("RangeOutlineBorderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


