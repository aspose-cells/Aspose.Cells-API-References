---
title: "LineFormat.BeginArrowheadLength"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LineFormat. Obtient et définit le type de longueur de flèche de départ de la ligne"
type: docs
url: /fr/net/aspose.cells.drawing/lineformat/beginarrowheadlength/
---
## LineFormat.BeginArrowheadLength property

Obtient et définit le type de longueur de la flèche de départ de la ligne.

```csharp
public MsoArrowheadLength BeginArrowheadLength { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne
            Shape lineShape = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);
            LineShape line = (LineShape)lineShape;

            // Définir la longueur de la pointe de flèche de départ
            line.Line.BeginArrowheadLength = MsoArrowheadLength.Long;

            // Enregistrez le classeur
            workbook.Save("LineFormatPropertyBeginArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


