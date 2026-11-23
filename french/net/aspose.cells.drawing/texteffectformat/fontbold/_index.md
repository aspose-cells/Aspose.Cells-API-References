---
title: "TextEffectFormat.FontBold"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextEffectFormat. Indique si la police est en gras"
type: docs
url: /fr/net/aspose.cells.drawing/texteffectformat/fontbold/
---
## TextEffectFormat.FontBold property

Indique si la police est en gras.

```csharp
public bool FontBold { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de texte (renvoie directement l'objet TextBox)
            TextBox textbox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
            textbox.Text = "Sample Text";

            // Obtenir le format d'effet de texte
            TextEffectFormat effFormat = textbox.TextEffect;

            // Définir les propriétés de la police, y compris le gras
            effFormat.FontName = "Arial";
            effFormat.FontBold = true;
            effFormat.FontItalic = false;
            effFormat.FontSize = 14;

            // Enregistrez le classeur
            workbook.Save("TextEffectFormatFontBoldDemo.xlsx");

            Console.WriteLine("Text effect format with bold font applied successfully.");
        }
    }
}
```

### Voir aussi

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


