---
title: "Range.SetOutlineBorders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Définit les bordures extérieures autour d’une plage de cellules avec le même style et la même couleur de bordure"
type: docs
url: /fr/net/aspose.cells/range/setoutlineborders/
---
## SetOutlineBorders(CellBorderType, CellsColor) {#setoutlineborders}

Définit les bordures extérieures autour d'une plage de cellules avec le même style et la même couleur de bordure.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, CellsColor borderColor)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| borderStyle | CellBorderType | Style de bordure. |
| borderColor | CellsColor | Couleur de bordure. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBordersWithCellBorderTypeCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer un objet CellsColor avec une couleur de thème
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Créer une plage et définir les bordures extérieures
            Aspose.Cells.Range range = cells.CreateRange("B2:D5");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Enregistrez le classeur
            workbook.Save("OutlineBordersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders_1}

Définit les bordures extérieures autour d'une plage de cellules avec le même style et la même couleur de bordure.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| borderStyle | CellBorderType | Style de bordure. |
| borderColor | Color | Couleur de bordure. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage de cellules (A1:D4)
            Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Remplir la plage avec des données pour rendre les bordures visibles
            for (int row = 0; row < 4; row++)
            {
                for (int col = 0; col < 4; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            try
            {
                // Appeler SetOutlineBorders avec un style de bordure moyen et une couleur rouge
                range.SetOutlineBorders(CellBorderType.Medium, Color.Red);

                // Enregistrer le classeur pour voir l'effet
                workbook.Save("RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_2}

Définit les bordures extérieures autour d'une plage de cellules.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Styles de bordure. |
| borderColors | Color[] | Couleurs de bordure. |

### Remarques

La longueur de borderStyles et de borderStyles doit être de 4. L'ordre de borderStyles et de borderStyles doit être haut,bas,gauche,droite.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage de cellules (B2:D4)
            Range range = worksheet.Cells.CreateRange("B2", "D4");

            // Préparer les styles de bordure et les couleurs
            CellBorderType[] borderStyles = new CellBorderType[]
            {
                CellBorderType.Thick,
                CellBorderType.Dashed,
                CellBorderType.Double,
                CellBorderType.MediumDashDot
            };

            Color[] borderColors = new Color[]
            {
                Color.Red,
                Color.Blue,
                Color.Green,
                Color.Purple
            };

            try
            {
                // Définir les bordures extérieures avec différents styles et couleurs
                range.SetOutlineBorders(borderStyles, borderColors);

                // Remplir les cellules avec des données pour rendre les bordures visibles
                for (int row = 1; row <= 3; row++)
                {
                    for (int col = 1; col <= 3; col++)
                    {
                        worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                    }
                }

                // Enregistrez le classeur
                workbook.Save("RangeSetOutlineBordersDemo.xlsx");
            }
            catch (System.Exception ex)
            {
                System.Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


