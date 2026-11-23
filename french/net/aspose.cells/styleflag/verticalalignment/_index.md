---
title: "StyleFlag.VerticalAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre d'alignement vertical sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/verticalalignment/
---
## StyleFlag.VerticalAlignment property

Le paramètre d’alignement vertical sera appliqué.

```csharp
public bool VerticalAlignment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créez un style avec alignement vertical
            Style style = workbook.CreateStyle();
            style.VerticalAlignment = TextAlignmentType.Center;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.Font.Color = Color.Blue;

            // Créez un indicateur de style pour n'appliquer que l'alignement vertical et la couleur de police
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.VerticalAlignment = true;
            styleFlag.FontColor = true;

            // Appliquez le style à la première ligne avec l'indicateur de style
            Row row = sheet.Cells.Rows[0];
            row.ApplyStyle(style, styleFlag);

            // Définissez du texte dans les cellules pour voir l'effet
            sheet.Cells["A1"].PutValue("Vertically Centered");
            sheet.Cells["B1"].PutValue("Blue Text");

            // Enregistrez le classeur
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


