---
title: "TextBoxOptions.TopMarginPt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextBoxOptions. Obtient et définit la marge supérieure en unité de points"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textboxoptions/topmarginpt/
---
## TextBoxOptions.TopMarginPt property

Obtient et définit la marge supérieure en unité de Points.

```csharp
public double TopMarginPt { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une zone de texte à la feuille de calcul
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Définir la marge supérieure en points
            textBox.TextBoxOptions.TopMarginPt = 0.2d;
            
            // Enregistrez le classeur
            workbook.Save("TextBoxTopMarginDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


