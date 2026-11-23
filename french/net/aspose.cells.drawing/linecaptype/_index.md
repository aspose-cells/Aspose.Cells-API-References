---
title: "Enum LineCapType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.LineCapType. Représente les extrémités d'une ligne"
type: docs
url: /fr/net/aspose.cells.drawing/linecaptype/
---
## LineCapType enumeration

Représente les extrémités d’une ligne

```csharp
public enum LineCapType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Square | `0` | Le carré dépasse de la moitié de la largeur de ligne. |
| Round | `1` | Extrémités arrondies. |
| Flat | `2` | La ligne se termine au point final. |
| None | `3` | Aucun cap |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
            
            LineFormat lineFmt = shape.Line;
            lineFmt.CapType = LineCapType.Flat;
            lineFmt.Weight = 2.0;
            lineFmt.DashStyle = MsoLineDashStyle.Solid;
            
            workbook.Save("LineCapTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


