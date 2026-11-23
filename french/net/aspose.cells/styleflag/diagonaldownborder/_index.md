---
title: "StyleFlag.DiagonalDownBorder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Les paramètres de bordure diagonale descendante seront appliqués"
type: docs
url: /fr/net/aspose.cells/styleflag/diagonaldownborder/
---
## StyleFlag.DiagonalDownBorder property

Les paramètres de bordure diagonale descendante seront appliqués.

```csharp
public bool DiagonalDownBorder { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalDownBorderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la cellule A1 et définir du texte
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Down Border Demo");

            // Créer un objet style et définir la bordure diagonale descendante
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 0, 255);
            
            // Créer un indicateur de style et activer l'indicateur de bordure diagonale descendante
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalDownBorder = true;

            // Appliquer le style avec l'indicateur à la cellule
            cell.SetStyle(style, styleFlag);

            // Vérifier si l'indicateur de bordure diagonale descendante est activé
            Console.WriteLine("DiagonalDownBorder flag is enabled: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);

            // Désactiver l'indicateur de bordure diagonale descendante
            styleFlag.DiagonalDownBorder = false;
            style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 255, 0);

            // Appliquer le style avec l'indicateur à la cellule
            cell.SetStyle(style, styleFlag);
            Console.WriteLine("DiagonalDownBorder flag is now: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);

            // Enregistrez le classeur
            workbook.Save("StyleFlagPropertyDiagonalDownBorderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


