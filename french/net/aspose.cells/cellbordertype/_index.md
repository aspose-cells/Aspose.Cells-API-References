---
title: "Enum CellBorderType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.CellBorderType enum. Énumère le type de bordure d'une cellule"
type: docs
url: /fr/net/aspose.cells/cellbordertype/
---
## CellBorderType enumeration

Énumère le type de bordure d'une cellule.

```csharp
public enum CellBorderType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DashDot | `9` | Représente une ligne fine tiret-point. |
| DashDotDot | `11` | Représente une ligne fine tiret-point-point. |
| Dashed | `3` | Représente une ligne en pointillés. |
| Dotted | `4` | Représente une ligne pointillée. |
| Double | `6` | Représente une double ligne. |
| Hair | `7` | Représente une ligne très fine. |
| MediumDashDot | `10` | Représente une ligne moyenne tiret-point. |
| MediumDashDotDot | `12` | Représente une ligne moyenne tiret-point-point. |
| MediumDashed | `8` | Représente une ligne moyenne en pointillés. |
| None | `0` | Représente aucune ligne. |
| Medium | `2` | Représente une ligne moyenne. |
| SlantedDashDot | `13` | Représente une ligne moyenne inclinée tiret-point. |
| Thick | `5` | Représente une ligne épaisse. |
| Thin | `1` | Représente une ligne fine. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellBorderTypeDemo
    {
        public static void CellBorderTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage (A1:D4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Obtenir le style de la plage
            Style style = workbook.CreateStyle();

            // Définir différents styles de bordure pour la plage
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = Color.Black;

            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;

            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.LeftBorder].Color = Color.Green;

            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            style.Borders[BorderType.RightBorder].Color = Color.Red;

            // Appliquer le style à la plage
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;
            range.ApplyStyle(style, styleFlag);

            // Enregistrez le classeur
            workbook.Save("CellBorderTypeExample.xlsx");
            workbook.Save("CellBorderTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


