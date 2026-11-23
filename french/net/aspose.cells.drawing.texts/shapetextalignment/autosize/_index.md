---
title: "ShapeTextAlignment.AutoSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeTextAlignment. Indique si la taille de la forme est ajustée automatiquement en fonction de son contenu"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/autosize/
---
## ShapeTextAlignment.AutoSize property

Indique si la taille de la forme est ajustée automatiquement en fonction de son contenu.

```csharp
public bool AutoSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de texte
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            textBox.Text = "This is a sample text that will demonstrate AutoSize property functionality";

            // Obtenez l'alignement du texte
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // Démontrez AutoSize = false (par défaut)
            shapeTextAlignment.AutoSize = false;
            Console.WriteLine("AutoSize false - Fixed size: " + textBox.Width + "x" + textBox.Height);

            // Démontrez AutoSize = true
            shapeTextAlignment.AutoSize = true;
            Console.WriteLine("AutoSize true - Auto sized: " + textBox.Width + "x" + textBox.Height);

            // Enregistrez le classeur
            workbook.Save("ShapeTextAlignmentAutoSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


