---
title: "MsoLineFormat.BackColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoLineFormat. Obtient et définit la couleur d'arrière-plan de la bordure de ligne"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformat/backcolor/
---
## MsoLineFormat.BackColor property

Obtient et définit la couleur d'arrière-plan de la ligne de bordure.

```csharp
public Color BackColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyBackColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Définir les propriétés de la ligne
            line.LineFormat.ForeColor = Color.Red;
            line.LineFormat.BackColor = Color.Yellow; // Demonstrating BackColor usage
            line.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            line.LineFormat.Weight = 2.0;

            // Enregistrez le classeur
            workbook.Save("LineFormatBackColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


