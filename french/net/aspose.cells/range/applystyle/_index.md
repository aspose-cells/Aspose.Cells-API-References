---
title: "Range.ApplyStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Applique des formats à toute la plage"
type: docs
url: /fr/net/aspose.cells/range/applystyle/
---
## Range.ApplyStyle method

Applique des formats à une plage entière.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | Style | L'objet style qui sera appliqué. |
| flag | StyleFlag | Indicateurs qui spécifient les propriétés de formatage appliquées. |

### Remarques

Chaque cellule de cette plage contiendra un objet [`Style`](../../style/). Ainsi, il s'agit d'une méthode gourmande en mémoire. Veuillez l'utiliser avec précaution.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;

            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue("Sample text for style demonstration");

            Aspose.Cells.Range range = cells.CreateRange(0, 0, 1, 3);

            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HorizontalAlignment = true;
            styleFlag.VerticalAlignment = true;
            styleFlag.WrapText = true;

            range.ApplyStyle(style, styleFlag);

            workbook.Save("ApplyStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


