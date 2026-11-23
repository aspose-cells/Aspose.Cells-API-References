---
title: "StyleFlag.DiagonalUpBorder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Les paramètres de bordure diagonale ascendante seront appliqués"
type: docs
url: /fr/net/aspose.cells/styleflag/diagonalupborder/
---
## StyleFlag.DiagonalUpBorder property

Les paramètres de bordure diagonale ascendante seront appliqués.

```csharp
public bool DiagonalUpBorder { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalUpBorderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la cellule A1 et définir du texte
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Créez un objet style et définissez la bordure diagonale ascendante
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 0, 255);

            // Créez un indicateur de style et activez le drapeau de bordure diagonale ascendante
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalUpBorder = true;

            // Appliquer le style avec l'indicateur à la cellule
            cell.SetStyle(style, styleFlag);

            // Créez une autre cellule pour démontrer l'effet
            Cell cell2 = worksheet.Cells["B2"];
            cell2.PutValue("Diagonal Up Border Demo");

            // Créez un style différent pour la comparaison
            Style style2 = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 255, 0);

            // Appliquez le deuxième style avec le même indicateur
            cell2.SetStyle(style2, styleFlag);

            // Enregistrez le classeur
            workbook.Save("StyleFlagPropertyDiagonalUpBorderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


