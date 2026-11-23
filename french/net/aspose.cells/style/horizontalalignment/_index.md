---
title: "Style.HorizontalAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient ou définit le type d'alignement horizontal du texte dans une cellule"
type: docs
url: /fr/net/aspose.cells/style/horizontalalignment/
---
## Style.HorizontalAlignment property

Obtient ou définit le type d'alignement horizontal du texte dans une cellule.

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir le texte dans les cellules
            cells["A1"].PutValue("Left Aligned");
            cells["A2"].PutValue("Center Aligned");
            cells["A3"].PutValue("Right Aligned");

            // Obtenir les objets de style
            Style styleLeft = cells["A1"].GetStyle();
            Style styleCenter = cells["A2"].GetStyle();
            Style styleRight = cells["A3"].GetStyle();

            // Définir l'alignement horizontal
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            styleRight.HorizontalAlignment = TextAlignmentType.Right;

            // Appliquer des styles aux cellules
            cells["A1"].SetStyle(styleLeft);
            cells["A2"].SetStyle(styleCenter);
            cells["A3"].SetStyle(styleRight);

            // Enregistrez le classeur
            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


