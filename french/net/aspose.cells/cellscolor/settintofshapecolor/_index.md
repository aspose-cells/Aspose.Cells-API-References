---
title: "CellsColor.SetTintOfShapeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsColor. Définir la teinte de la couleur de forme"
type: docs
url: /fr/net/aspose.cells/cellscolor/settintofshapecolor/
---
## CellsColor.SetTintOfShapeColor method

Définir la teinte de la couleur de la forme

```csharp
public void SetTintOfShapeColor(double tint)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| teinte | Double |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CellsColorMethodSetTintOfShapeColorWithDoubleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Obtenir la couleur de remplissage de la forme
                CellsColor shapeColor = shape.Fill.SolidFill.CellsColor;
                
                // Définir la couleur à considérer comme couleur de forme
                shapeColor.IsShapeColor = true;
                
                // Définir la teinte de la couleur de forme (plage valide de -1.0 à 1.0)
                shapeColor.SetTintOfShapeColor(0.5); // Lighten the color by 50%
                
                Console.WriteLine("SetTintOfShapeColor method executed successfully with parameter 0.5");
                
                // Afficher l'effet en changeant la couleur de remplissage de la forme
                shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTintOfShapeColor method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("SetTintOfShapeColorWithDoubleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


