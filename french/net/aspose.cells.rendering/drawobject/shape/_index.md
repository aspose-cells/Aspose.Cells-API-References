---
title: "DrawObject.Shape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DrawObject. Indique l'objet Shape lors du rendu. Toutes les propriétés de Shape peuvent être accessibles"
type: docs
url: /fr/net/aspose.cells.rendering/drawobject/shape/
---
## DrawObject.Shape property

Indique l’objet Shape lors du rendu. Toutes les propriétés de la forme sont accessibles.

```csharp
public Shape Shape { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyShapeDemo
    {
        public static void Run()
        {
            try
            {
                // Créez un nouveau classeur et obtenez la première feuille de calcul
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajoutez des données d'exemple pour rendre le rendu significatif
                worksheet.Cells["A1"].Value = "Sample Data";
                worksheet.Cells["A2"].Value = "More Data";

                // Ajouter une forme à la feuille de calcul
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Configurez les options de rendu avec un gestionnaire personnalisé
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new ShapePropertyHandler()
                };

                // Rendez la feuille de calcul - cela déclenchera les événements DrawObject
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "ShapeDemo.png");

                // Enregistrez le classeur
                workbook.Save("ShapeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Gestionnaire personnalisé pour capturer les événements DrawObject et lire la propriété Shape
        private class ShapePropertyHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                if (drawObject.Shape != null)
                {
                    Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                    Console.WriteLine($"Shape Name: {drawObject.Shape.Name}");
                    Console.WriteLine($"Shape Text: {drawObject.Shape.Text}");
                    Console.WriteLine($"Shape Width: {drawObject.Shape.Width} pixels");
                    Console.WriteLine($"Shape Height: {drawObject.Shape.Height} pixels");
                    Console.WriteLine($"Shape Type: {drawObject.Shape.AutoShapeType}");
                    Console.WriteLine();
                }
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../../../aspose.cells.drawing/shape/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


