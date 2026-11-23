---
title: "SolidFill.Color"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SolidFill. Obtient ou définit la Couleur"
type: docs
url: /fr/net/aspose.cells.drawing/solidfill/color/
---
## SolidFill.Color property

Obtient ou définit la couleur.

```csharp
public Color Color { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez une forme à la feuille de calcul avec les paramètres corrects
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Définissez les propriétés de la forme avec couleur
            Color fillColor = Color.LightBlue;
            Color textColor = Color.DarkBlue;
            string text = "Solid Fill Demo";

            // Démontrez l'utilisation de la propriété Color
            shape.Fill.SolidFill.Color = fillColor;
            shape.LineFormat.ForeColor = fillColor;
            shape.Text = text;
            shape.Font.Color = textColor;

            // Enregistrez le classeur
            workbook.Save("SolidFillPropertyColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


