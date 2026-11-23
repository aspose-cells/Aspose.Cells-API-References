---
title: "TextBoxOptions.AllowTextToOverflow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxOptions. Indique si le texte peut dépasser la forme"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/
---
## TextBoxOptions.AllowTextToOverflow property

Autoriser le texte à dépasser la forme.

```csharp
public bool AllowTextToOverflow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyAllowTextToOverflowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Définir le texte qui pourrait dépasser
            textBox.Text = "This is a long text that might overflow the text box boundaries if AllowTextToOverflow is false";

            // Activer le dépassement du texte
            textBox.TextBoxOptions.AllowTextToOverflow = true;

            // Enregistrez le classeur
            workbook.Save("TextBoxAllowTextToOverflowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


