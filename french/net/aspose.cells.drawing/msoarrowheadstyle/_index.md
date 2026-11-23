---
title: "Enum MsoArrowheadStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.MsoArrowheadStyle. Énumère le type d'extrémité de ligne du bord de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/msoarrowheadstyle/
---
## MsoArrowheadStyle enumeration

Énumère le type d’extrémité de ligne de la bordure de forme.

```csharp
public enum MsoArrowheadStyle
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Pas de type d'extrémité de ligne. |
| Arrow | `1` | Type d'extrémité de ligne flèche. |
| ArrowStealth | `2` | Type d'extrémité de ligne flèche furtive. |
| ArrowDiamond | `3` | Type d'extrémité de ligne flèche diamant. |
| ArrowOval | `4` | Type d'extrémité de ligne flèche ovale. |
| ArrowOpen | `5` | Type d'extrémité de ligne flèche ouverte. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassMsoArrowheadStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne
            LineShape lineShape = worksheet.Shapes.AddLine(5, 5, 10, 10, 100, 100);

            // Définir les propriétés de la ligne
            MsoLineFormat lineFormat = lineShape.LineFormat;
            lineFormat.ForeColor = System.Drawing.Color.Black;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 0.75;

            // Définir les styles de pointe de flèche
            lineShape.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
            lineShape.Line.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineShape.Line.BeginArrowheadLength = MsoArrowheadLength.Medium;
            lineShape.Line.EndArrowheadLength = MsoArrowheadLength.Medium;

            // Enregistrez le classeur
            workbook.Save("MsoArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


