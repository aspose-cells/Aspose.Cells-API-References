---
title: "Column.ApplyStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Column. Applique des formats à une colonne entière"
type: docs
url: /fr/net/aspose.cells/column/applystyle/
---
## Column.ApplyStyle method

Applique des formats à une colonne entière.

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
    public class ColumnMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Définir du texte multi-lignes dans la colonne 2
            sheet.Cells[0, 1].Value = "Line1\nLine2";
            sheet.Cells[1, 1].Value = "Text with\nmultiple lines";
            sheet.Cells[2, 1].Value = "Another\nmulti-line\ntext";

            // Créer un style avec le texte à la ligne activé
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Appliquer le style uniquement à la propriété de texte à la ligne de la colonne 2
            sheet.Cells.Columns[1].ApplyStyle(style, new StyleFlag() { WrapText = true });

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


