---
title: "Cells.ApplyColumnStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Applique des formats à une colonne entière"
type: docs
url: /fr/net/aspose.cells/cells/applycolumnstyle/
---
## Cells.ApplyColumnStyle method

Applique des formats à une colonne entière.

```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | L'index de colonne. |
| style | Style | L'objet style qui sera appliqué. |
| flag | StyleFlag | Indicateurs qui spécifient les propriétés de formatage appliquées. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyColumnStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Créer un style avec des bordures
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Créer un indicateur de style pour appliquer uniquement les bordures
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;

            // Appliquer le style à la colonne 1 (indice 0)
            cells.ApplyColumnStyle(0, style, sflag);

            // Enregistrez le classeur
            workbook.Save("ApplyColumnStyleOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


