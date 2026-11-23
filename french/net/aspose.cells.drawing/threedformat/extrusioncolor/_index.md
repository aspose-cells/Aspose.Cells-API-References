---
title: "ThreeDFormat.ExtrusionColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient la couleur d'extrusion d'une forme"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/extrusioncolor/
---
## ThreeDFormat.ExtrusionColor property

Obtient la couleur d'extrusion d'une forme.

```csharp
public CellsColor ExtrusionColor { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyExtrusionColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer le formatage 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
            shape.Text = "3D ExtrusionColor Demo";
            
            // Obtenir le ThreeDFormat de la forme
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Configurez les propriétés 3D de base pour rendre l'extrusion visible
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Material = PresetMaterialType.Plastic;

            try
            {
                // Obtenez et affichez la valeur de ExtrusionColor
                CellsColor extrusionColor = threeDFormat.ExtrusionColor;
                Console.WriteLine("ExtrusionColor properties:");
                Console.WriteLine($"Type: {extrusionColor.Type}");
                Console.WriteLine($"Color (RGB): {extrusionColor.Color}");
                Console.WriteLine($"Transparency: {extrusionColor.Transparency}");

                // Enregistrez le classeur pour voir les effets 3D
                workbook.Save("ThreeDFormatExtrusionColorDemo.xlsx");
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


