---
title: "StyleFlag.WrapText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "StyleFlag propriété. Le paramètre d'habillage du texte sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/wraptext/
---
## StyleFlag.WrapText property

Le paramètre de retour à la ligne sera appliqué.

```csharp
public bool WrapText { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyWrapTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style avec l'habillage du texte activé
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Créer un indicateur de style et activer l'indicateur WrapText
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;

            // Appliquer le style à la cellule A1 avec les indicateurs spécifiés
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap in the cell");
            worksheet.Cells.ApplyStyle(style, flag);

            // Ajuster automatiquement la hauteur de la ligne pour voir le texte enveloppé
            worksheet.AutoFitRow(0);

            // Enregistrez le classeur
            workbook.Save("WrapTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


