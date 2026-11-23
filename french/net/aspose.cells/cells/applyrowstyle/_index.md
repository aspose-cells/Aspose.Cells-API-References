---
title: "Cells.ApplyRowStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Applique des formats à une ligne entière"
type: docs
url: /fr/net/aspose.cells/cells/applyrowstyle/
---
## Cells.ApplyRowStyle method

Applique les formats à toute la ligne.

```csharp
public void ApplyRowStyle(int row, Style style, StyleFlag flag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| style | Style | L'objet style qui sera appliqué. |
| flag | StyleFlag | Indicateurs qui spécifient les propriétés de formatage appliquées. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyRowStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer un style avec des bordures
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Créer un indicateur de style pour les bordures
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Appliquer le style à la première ligne
            cells.ApplyRowStyle(0, style, styleFlag);

            // Enregistrez le classeur
            workbook.Save("ApplyRowStyleDemo.xlsx");
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


