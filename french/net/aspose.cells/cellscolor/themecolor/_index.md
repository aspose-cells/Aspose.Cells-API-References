---
title: "CellsColor.ThemeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsColor. Obtient la couleur du thème. S'applique uniquement au type de couleur du thème"
type: docs
url: /fr/net/aspose.cells/cellscolor/themecolor/
---
## CellsColor.ThemeColor property

Obtient la couleur du thème. S'applique uniquement au type de couleur de thème.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créer une instance de CellsColor
                CellsColor cellsColor = workbook.CreateCellsColor();

                // Définir une couleur de thème
                cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Afficher les propriétés ThemeColor
                Console.WriteLine("ThemeColor Type: " + cellsColor.ThemeColor.ColorType);
                Console.WriteLine("ThemeColor Tint: " + cellsColor.ThemeColor.Tint);

                // Appliquer la couleur à une cellule
                Style style = workbook.CreateStyle();
                style.ForegroundColor = cellsColor.Color;
                style.Pattern = BackgroundType.Solid;

                worksheet.Cells["A1"].PutValue("Theme Color Example");
                worksheet.Cells["A1"].SetStyle(style);

                // Enregistrez le classeur
                workbook.Save("ThemeColorDemo.xlsx");
                Console.WriteLine("ThemeColor has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ThemeColor](../../themecolor/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


