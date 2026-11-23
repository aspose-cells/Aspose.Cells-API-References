---
title: "LineFormat.EndArrowheadStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LineFormat. Obtient et définit le type de flèche de fin de la ligne"
type: docs
url: /fr/net/aspose.cells.drawing/lineformat/endarrowheadstyle/
---
## LineFormat.EndArrowheadStyle property

Obtient et définit le type de flèche de fin de la ligne.

```csharp
public MsoArrowheadStyle EndArrowheadStyle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Obtenir le format de ligne
            LineFormat lineFmt = line.Line;

            // Définissez le style de tête de flèche de fin
            lineFmt.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Enregistrez le classeur
            workbook.Save("LineFormatPropertyEndArrowheadStyleDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


