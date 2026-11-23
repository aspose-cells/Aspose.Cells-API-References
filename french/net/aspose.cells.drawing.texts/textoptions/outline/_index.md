---
title: "TextOptions.Outline"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextOptions. Représente le format de contour du texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textoptions/outline/
---
## TextOptions.Outline property

Représente le format de contour du texte.

```csharp
public LineFormat Outline { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyOutlineDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme avec du texte
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            shape.Text = "Sample Text";

            // Accédez aux options de texte
            TextOptions textOptions = shape.TextOptions;

            // Configurez les propriétés de contour
            LineFormat outline = textOptions.Outline;
            outline.Weight = 2.48; // Set outline weight
            outline.DashStyle = MsoLineDashStyle.Solid; // Set line style
            outline.CompoundType = MsoLineStyle.Single; // Set compound type

            // Enregistrez le classeur
            workbook.Save("TextOutlineDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [LineFormat](../../../aspose.cells.drawing/lineformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


