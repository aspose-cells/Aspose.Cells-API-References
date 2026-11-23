---
title: "CellsColor.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsColor. Le type de couleur"
type: docs
url: /fr/net/aspose.cells/cellscolor/type/
---
## CellsColor.Type property

Le type de couleur.

```csharp
public ColorType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CellsColorPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour démontrer CellsColor
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            CellsColor cellsColor = shape.Fill.SolidFill.CellsColor;

            // Afficher le type de couleur initial
            Console.WriteLine("Initial Color Type: " + cellsColor.Type);

            // Définir la couleur RVB et afficher le changement de type
            cellsColor.Color = System.Drawing.Color.Red;
            Console.WriteLine("After setting RGB Color - Type: " + cellsColor.Type);

            // Définir la couleur indexée et afficher le changement de type
            cellsColor.ColorIndex = 5; // Standard Excel color index
            Console.WriteLine("After setting ColorIndex - Type: " + cellsColor.Type);

            // Définir la couleur du thème et afficher le changement de type
            cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.0); // Added tint parameter
            Console.WriteLine("After setting ThemeColor - Type: " + cellsColor.Type);

            // Démontrer différents types de couleur dans les cellules
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("RGB Color");
            Style style1 = cell1.GetStyle(); // Use GetStyle() instead of Style property
            style1.ForegroundColor = System.Drawing.Color.Blue;
            style1.Pattern = BackgroundType.Solid;
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Indexed Color");
            Style style2 = cell2.GetStyle(); // Use GetStyle() instead of Style property
            style2.ForegroundColor = System.Drawing.Color.FromArgb(5); // Using color index
            style2.Pattern = BackgroundType.Solid;
            cell2.SetStyle(style2);

            // Enregistrer le résultat
            workbook.Save("CellsColorTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ColorType](../../colortype/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


