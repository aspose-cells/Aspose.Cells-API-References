---
title: "LineFormat.EndArrowheadWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LineFormat. Obtient et définit le type de largeur de flèche de fin de la ligne"
type: docs
url: /fr/net/aspose.cells.drawing/lineformat/endarrowheadwidth/
---
## LineFormat.EndArrowheadWidth property

Obtient et définit le type de largeur de la flèche de fin de la ligne.

```csharp
public MsoArrowheadWidth EndArrowheadWidth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne
            Shape line = worksheet.Shapes.AddLine(10, 10, 100, 10, 5, 5);

            // Obtenir le format de ligne
            LineFormat lineFmt = line.Line;

            // Définir la largeur de la flèche de fin
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Enregistrez le classeur
            workbook.Save("LineFormatPropertyEndArrowheadWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


