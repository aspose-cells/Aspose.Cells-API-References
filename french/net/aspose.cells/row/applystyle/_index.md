---
title: "Row.ApplyStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Row. Applique des formats pour une ligne entière"
type: docs
url: /fr/net/aspose.cells/row/applystyle/
---
## Row.ApplyStyle method

Applique les formats à toute la ligne.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | Style | L'objet style qui sera appliqué. |
| flag | StyleFlag | Indicateurs qui spécifient les propriétés de formatage appliquées. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Définir le contenu HTML dans la première cellule
            sheet.Cells[0, 0].HtmlString = @"<font style=""color: #49c131; font-weight: bold;"">Styled </font><font>text</font>";

            // Obtenir la première ligne et son style
            Row row = sheet.Cells.Rows[0];
            Style style = row.GetStyle();
            
            // Modifier les propriétés du style
            style.IsTextWrapped = true;
            style.HorizontalAlignment = TextAlignmentType.Center;

            // Appliquer le style avec des indicateurs spécifiques (seul le retour à la ligne sera appliqué)
            row.ApplyStyle(style, new StyleFlag { WrapText = true });

            // Ajustement automatique à des fins de démonstration
            sheet.AutoFitRows();
            sheet.AutoFitColumns();

            // Enregistrez le classeur
            workbook.Save("RowApplyStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


