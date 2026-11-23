---
title: "Enum BackgroundType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.BackgroundType. Énumère les types de motifs d'arrière-plan de cellule"
type: docs
url: /fr/net/aspose.cells/backgroundtype/
---
## BackgroundType enumeration

Énumère les types de motifs d'arrière-plan de cellule.

```csharp
public enum BackgroundType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DiagonalCrosshatch | `9` | Représente le motif de hachures diagonales. |
| DiagonalStripe | `8` | Représente le motif de bandes diagonales. |
| Gray6 | `18` | Représente le motif gris à 6,25 % |
| Gray12 | `17` | Représente le motif gris à 12,5 % |
| Gray25 | `4` | Représente le motif gris à 25 %. |
| Gray50 | `2` | Représente le motif gris à 50 %. |
| Gray75 | `3` | Représente le motif gris à 75 %. |
| HorizontalStripe | `5` | Représente le motif de bandes horizontales. |
| None | `0` | Représente aucun arrière-plan. |
| ReverseDiagonalStripe | `7` | Représente le motif de bandes diagonales inversées. |
| Solid | `1` | Représente le motif plein. |
| ThickDiagonalCrosshatch | `10` | Représente le motif de hachures diagonales épaisses. |
| ThinDiagonalCrosshatch | `16` | Représente le motif de hachures diagonales fines. |
| ThinDiagonalStripe | `14` | Représente le motif de bandes diagonales fines. |
| ThinHorizontalCrosshatch | `15` | Représente le motif de hachures horizontales fines. |
| ThinHorizontalStripe | `11` | Représente le motif de bandes horizontales fines. |
| ThinReverseDiagonalStripe | `13` | Représente le motif de bandes diagonales inversées fines. |
| ThinVerticalStripe | `12` | Représente un motif de bande verticale fine. |
| VerticalStripe | `6` | Représente un motif de bande verticale. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BackgroundTypeDemo
    {
        public static void BackgroundTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul du classeur
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à une cellule de la feuille de calcul
            Cell cell = worksheet.Cells["A1"];
            
            // Définissez la valeur de la cellule
            cell.PutValue("Hello, Aspose!");

            // Créez un objet de style
            Style style = cell.GetStyle();
            
            // Définissez le type de motif d'arrière-plan
            style.Pattern = BackgroundType.DiagonalStripe;
            
            // Définissez la couleur de premier plan
            style.ForegroundColor = Color.Red;
            
            // Définissez la couleur d'arrière-plan
            style.BackgroundColor = Color.Green;
            
            // Appliquez le style à la cellule
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("BackgroundTypeExample.xlsx");
            workbook.Save("BackgroundTypeExample.pdf");



        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


