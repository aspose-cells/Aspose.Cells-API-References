---
title: "LineFormat.CapType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LineFormat. Spécifie les terminaisons"
type: docs
url: /fr/net/aspose.cells.drawing/lineformat/captype/
---
## LineFormat.CapType property

Spécifie les embouts de fin.

```csharp
public LineCapType CapType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Définir les propriétés du format de ligne
            LineFormat lineFmt = line.Line;
            lineFmt.CapType = LineCapType.Flat;

            // Enregistrez le classeur
            workbook.Save("LineFormatCapTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [LineCapType](../../linecaptype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


