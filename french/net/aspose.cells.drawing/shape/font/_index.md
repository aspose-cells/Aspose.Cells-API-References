---
title: "Shape.Font"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente la police de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/font/
---
## Shape.Font property

Représente la police de la forme.

```csharp
public Font Font { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFontDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Accéder et modifier les propriétés de police de la forme
            Aspose.Cells.Font font = shape.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;

            // Enregistrez le classeur
            workbook.Save("ShapeFontDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../../../aspose.cells/font/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


