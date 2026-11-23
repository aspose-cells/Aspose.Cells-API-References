---
title: "StyleFlag.LeftBorder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Les paramètres de bordure gauche seront appliqués"
type: docs
url: /fr/net/aspose.cells/styleflag/leftborder/
---
## StyleFlag.LeftBorder property

Les paramètres de bordure gauche seront appliqués.

```csharp
public bool LeftBorder { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLeftBorderDemo
    {
        public static void Run()
        {
            // Créer un classeur
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];

            // Créer une plage et appliquer le style de bordure gauche
            var range = worksheet.Cells.CreateRange(1, 1, 1, 1);
            range.PutValue("Left Border Demo", false, false);

            // Créer le style et l'indicateur
            var style = workbook.CreateStyle();
            var flag = new StyleFlag();

            // Définir les propriétés de la bordure gauche
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thick;
            flag.LeftBorder = true;

            // Appliquer le style avec l'indicateur de bordure gauche
            range.ApplyStyle(style, flag);

            // Vérifier que la bordure gauche a été appliquée
            var appliedStyle = worksheet.Cells[1, 1].GetStyle();
            Console.WriteLine($"Left border color: {appliedStyle.Borders[BorderType.LeftBorder].Color}");
            Console.WriteLine($"Left border style: {appliedStyle.Borders[BorderType.LeftBorder].LineStyle}");

            // Enregistrez le classeur
            workbook.Save("LeftBorderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


