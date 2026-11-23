---
title: "LineFormat.BeginArrowheadWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LineFormat. Obtient et définit le type de largeur de flèche de début de la ligne"
type: docs
url: /fr/net/aspose.cells.drawing/lineformat/beginarrowheadwidth/
---
## LineFormat.BeginArrowheadWidth property

Obtient et définit le type de largeur de la flèche de départ de la ligne.

```csharp
public MsoArrowheadWidth BeginArrowheadWidth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Définir les propriétés du format de ligne
            LineFormat lineFmt = line.Line;
            lineFmt.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Enregistrez le classeur
            workbook.Save("LineFormatDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


