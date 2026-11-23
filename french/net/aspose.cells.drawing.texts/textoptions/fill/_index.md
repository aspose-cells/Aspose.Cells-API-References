---
title: "TextOptions.Fill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextOptions. Représente le format de remplissage du texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textoptions/fill/
---
## TextOptions.Fill property

Représente le format de remplissage du texte.

```csharp
public FillFormat Fill { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            shape.Text = "Sample Text";
            
            FontSetting fontSetting = shape.Characters(0, shape.Text.Length);
            TextOptions textOptions = fontSetting.TextOptions;
            
            // Définir les propriétés de la police
            textOptions.Name = "Arial";
            textOptions.Size = 14;
            textOptions.IsBold = true;
            
            // Démontrer la propriété Fill
            textOptions.Fill.FillType = FillType.Solid;
            SolidFill solidFill = textOptions.Fill.SolidFill;
            solidFill.Color = System.Drawing.Color.Blue;
            
            // Enregistrez le classeur
            workbook.Save("TextOptionsFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FillFormat](../../../aspose.cells.drawing/fillformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


