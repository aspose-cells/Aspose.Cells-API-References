---
title: "ShapeTextAlignment.TextShapeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeTextAlignment. Obtient et définit le type de transformation du texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/textshapetype/
---
## ShapeTextAlignment.TextShapeType property

Obtient et définit le type de transformation du texte.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de texte
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);

            // Obtenir l'alignement du texte de la forme
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // Définir la propriété TextShapeType
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;

            // Enregistrez le classeur
            workbook.Save("TextShapeTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [AutoShapeType](../../../aspose.cells.drawing/autoshapetype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


