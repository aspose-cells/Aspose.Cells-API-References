---
title: "Classe DrawObject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.DrawObject. DrawObject sera initialisé et renvoyé lors du rendu"
type: docs
url: /fr/net/aspose.cells.rendering/drawobject/
---
## DrawObject class

DrawObject sera initialisé et renvoyé lors du rendu.

```csharp
public class DrawObject
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Cell](../../aspose.cells.rendering/drawobject/cell/) { get; } | Indique l’objet Cell lors du rendu. Toutes les propriétés de la cellule sont accessibles. |
| [CurrentPage](../../aspose.cells.rendering/drawobject/currentpage/) { get; } | Indique l’indice de page de DrawObject. L’indice de page commence à zéro. Une feuille contient plusieurs pages lors du rendu. |
| [ImageBytes](../../aspose.cells.rendering/drawobject/imagebytes/) { get; } | Indique les octets d’image du graphique ou de la forme rendus lors du rendu. |
| [Shape](../../aspose.cells.rendering/drawobject/shape/) { get; } | Indique l’objet Shape lors du rendu. Toutes les propriétés de la forme sont accessibles. |
| [SheetIndex](../../aspose.cells.rendering/drawobject/sheetindex/) { get; } | Indique l’indice de la feuille actuelle de DrawObject. |
| [TotalPages](../../aspose.cells.rendering/drawobject/totalpages/) { get; } | Indique le nombre total de pages dans le rendu actuel. |
| [Type](../../aspose.cells.rendering/drawobject/type/) { get; } | Indique le type de DrawObject. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;

namespace AsposeCellsExamples
{
    // Implémentation personnalisée de DrawObjectEventHandler
    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"Drawing object at X: {x}, Y: {y}, Width: {width}, Height: {height}");
            Console.WriteLine($"Object Type: {drawObject.Type}");
            Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}");

            if (drawObject.Cell != null)
            {
                Console.WriteLine($"Rendering Cell: {drawObject.Cell.Name}, Value: {drawObject.Cell.Value}");
            }

            if (drawObject.Shape != null)
            {
                Console.WriteLine($"Rendering Shape: {drawObject.Shape.Name}");
            }
        }
    }

    public class DrawObjectDemo
    {
        public static void RunDemo()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

            // Ajouter une forme
            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddShape(Aspose.Cells.Drawing.MsoDrawingType.Rectangle, 5, 0, 5, 0, 100, 100);
            shape.Text = "Sample Shape";

            // Créer une instance de CustomDrawObjectEventHandler
            CustomDrawObjectEventHandler drawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Définir les options d’image ou d’impression
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                DrawObjectEventHandler = drawObjectEventHandler,
                OnePagePerSheet = true,
                ImageType = Aspose.Cells.Drawing.ImageType.Png
            };

            // Rendre la feuille en image
            SheetRender sr = new SheetRender(sheet, options);
            sr.ToImage(0, "DrawObjectDemo.png");

            // Enregistrez le classeur
            workbook.Save("DrawObjectDemo.xlsx");
            workbook.Save("DrawObjectDemo.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


