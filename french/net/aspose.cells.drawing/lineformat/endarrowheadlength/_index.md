---
title: "LineFormat.EndArrowheadLength"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LineFormat. Obtient et définit le type de longueur de flèche de fin de la ligne"
type: docs
url: /fr/net/aspose.cells.drawing/lineformat/endarrowheadlength/
---
## LineFormat.EndArrowheadLength property

Obtient et définit le type de longueur de la flèche de fin de la ligne.

```csharp
public MsoArrowheadLength EndArrowheadLength { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne et obtenir l'objet forme directement
            LineShape line = (LineShape)worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Définir la longueur de la pointe de flèche de fin
            line.Line.EndArrowheadLength = MsoArrowheadLength.Long;

            // Enregistrez le classeur
            workbook.Save("LineFormatPropertyEndArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


