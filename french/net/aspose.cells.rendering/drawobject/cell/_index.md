---
title: "DrawObject.Cell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DrawObject. Indique l'objet Cell lors du rendu. Toutes les propriétés de Cell peuvent être accessibles"
type: docs
url: /fr/net/aspose.cells.rendering/drawobject/cell/
---
## DrawObject.Cell property

Indique l’objet Cell lors du rendu. Toutes les propriétés de la cellule sont accessibles.

```csharp
public Cell Cell { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    // Gestionnaire personnalisé pour capturer les événements DrawObject et lire la propriété Cell
    public class CellInfoDrawHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Affichez les informations de base de l'objet de dessin
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");

            // Démontrez la lecture de la propriété Cell en lecture seule
            if (drawObject.Cell != null)
            {
                var cell = drawObject.Cell;
                Console.WriteLine($"Cell Name: {cell.Name}");
                Console.WriteLine($"Cell Value: {cell.Value}");
                Console.WriteLine($"Cell Row: {cell.Row}, Column: {cell.Column}");
            }
        }
    }

    public class DrawObjectPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // Créez un nouveau classeur et obtenez la première feuille de calcul
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Ajouter des données d'exemple aux cellules
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Ajoutez une forme pour garantir que les shape draw events soient également déclenchés
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Configurez les options de rendu avec notre gestionnaire de dessin personnalisé
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CellInfoDrawHandler()
                };

                // Rendez la feuille de calcul – cela déclenchera les événements DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectCellDemo.png");

                // Enregistrer le classeur (facultatif)
                workbook.Save("DrawObjectCellDemo.xlsx");
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

* class [Cell](../../../aspose.cells/cell/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


