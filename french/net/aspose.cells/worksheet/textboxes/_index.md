---
title: "Worksheet.TextBoxes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient une collection de TextBox"
type: docs
url: /fr/net/aspose.cells/worksheet/textboxes/
---
## Worksheet.TextBoxes property

Obtient une collection de [`TextBox`](../../../aspose.cells.drawing/textbox/).

```csharp
public TextBoxCollection TextBoxes { get; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTextBoxesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            int tID = ws.TextBoxes.Add(1, 1, 500, 1000);
            Aspose.Cells.Drawing.TextBox textBox = ws.TextBoxes[tID];

            // Définissez le texte et formatez des parties de celui-ci
            textBox.Text = "Red text 1. Plain text 1. Red text 2. Plain text 2.";
            textBox.Characters(0, 10).Font.Color = Color.Red;
            textBox.Characters(26, 10).Font.Color = Color.DarkRed;

            // Enregistrez le classeur
            wb.Save("TextBoxExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextBoxCollection](../../../aspose.cells.drawing/textboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


