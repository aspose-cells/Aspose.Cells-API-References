---
title: "ShapeTextAlignment.IsLockedText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeTextAlignment. Indique si la forme est verrouillée lorsque la feuille de calcul est protégée"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/islockedtext/
---
## ShapeTextAlignment.IsLockedText property

Indique si la forme est verrouillée lorsque la feuille de calcul est protégée.

```csharp
public bool IsLockedText { get; set; }
```

### Remarques

Fonctionne uniquement lorsque la feuille de calcul est protégée.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsLockedTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text";

            // Accédez aux propriétés d'alignement du texte
            Aspose.Cells.Drawing.Texts.ShapeTextAlignment textAlignment = textBox.TextBody.TextAlignment;

            // Définissez et démontrez la propriété IsLockedText
            textAlignment.IsLockedText = true;
            Console.WriteLine("Text locked status: " + textAlignment.IsLockedText);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


