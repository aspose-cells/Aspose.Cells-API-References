---
title: "TextEffectFormat.FontSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextEffectFormat. La taille en points de la police utilisée dans le WordArt"
type: docs
url: /fr/net/aspose.cells.drawing/texteffectformat/fontsize/
---
## TextEffectFormat.FontSize property

La taille (en points) de la police utilisée dans le WordArt.

```csharp
public int FontSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            int textboxIndex = worksheet.TextBoxes.Add(5, 5, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[textboxIndex];
            
            // Définir le texte et le format
            textBox.Text = "Sample Text Effect";
            
            // Obtenir le format d'effet de texte
            Shape shape = textBox;
            TextEffectFormat effectFormat = shape.TextEffect;
            
            // Définir les propriétés de la police, y compris FontSize
            effectFormat.FontName = "Arial";
            effectFormat.FontBold = true;
            effectFormat.FontItalic = false;
            effectFormat.FontSize = 18; // Demonstrating FontSize property
            
            // Enregistrez le classeur
            workbook.Save("TextEffectFontSizeDemo.xlsx");
            
            Console.WriteLine("Text effect with font size 18 created successfully.");
        }
    }
}
```

### Voir aussi

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


