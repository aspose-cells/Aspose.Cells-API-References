---
title: "CellsColor.ColorIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsColor. Obtient et définit l'index de couleur dans la palette de couleurs. S'applique uniquement aux couleurs indexées"
type: docs
url: /fr/net/aspose.cells/cellscolor/colorindex/
---
## CellsColor.ColorIndex property

Obtient et définit l'index de couleur dans la palette. S'applique uniquement aux couleurs indexées.

```csharp
public int ColorIndex { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class CellsColorPropertyColorIndexDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir une plage à laquelle nous appliquerons une bordure colorée
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Créer une instance de CellsColor
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Définir le ColorIndex (index de palette) – par exemple, 5
            cellsColor.ColorIndex = 5;

            // Appliquer le CellsColor comme couleur de bordure intérieure de la plage
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical,
                                   CellBorderType.Thin,
                                   cellsColor);

            // Lire et afficher la valeur actuelle de ColorIndex
            Console.WriteLine("Current ColorIndex value: " + cellsColor.ColorIndex);

            // Enregistrer le classeur pour visualiser le résultat
            try
            {
                workbook.Save("ColorIndexDemo.xlsx");
                Console.WriteLine("Workbook saved as ColorIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


