---
title: "LineFormat.CompoundType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LineFormat. Spécifie le type de composé de ligne"
type: docs
url: /fr/net/aspose.cells.drawing/lineformat/compoundtype/
---
## LineFormat.CompoundType property

Spécifie le type de composition de la ligne.

```csharp
public MsoLineStyle CompoundType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCompoundTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Obtenir le format de ligne
            LineFormat lineFmt = line.Line;

            // Définir le type composé
            lineFmt.CompoundType = MsoLineStyle.Single;

            // Enregistrez le classeur
            workbook.Save("LineFormatCompoundTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoLineStyle](../../msolinestyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


