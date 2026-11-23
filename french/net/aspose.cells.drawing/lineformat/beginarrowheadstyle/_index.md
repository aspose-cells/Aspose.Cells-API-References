---
title: "LineFormat.BeginArrowheadStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LineFormat. Obtient et définit le type de flèche de départ de la ligne"
type: docs
url: /fr/net/aspose.cells.drawing/lineformat/beginarrowheadstyle/
---
## LineFormat.BeginArrowheadStyle property

Obtient et définit le type de flèche de départ de la ligne.

```csharp
public MsoArrowheadStyle BeginArrowheadStyle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Définir le style de la pointe de flèche de départ
            line.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Enregistrez le classeur
            workbook.Save("LineFormatPropertyBeginArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


