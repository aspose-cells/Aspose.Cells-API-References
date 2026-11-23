---
title: "Shape.TextOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente les options de texte de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/textoptions/
---
## Shape.TextOptions property

Représente les options de texte de la forme.

```csharp
public TextOptions TextOptions { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Définir le texte pour la forme
            shape.Text = "Sample Text";

            // Accédez et modifiez TextOptions
            TextOptions opt = shape.TextOptions;
            opt.Color = Color.Blue;
            opt.Size = 8;

            // Enregistrez le classeur
            workbook.Save("ShapeTextOptionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


