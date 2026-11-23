---
title: "MsoFillFormat.BackColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFillFormat. Obtient et définit la couleur d'arrière-plan du fichier"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformat/backcolor/
---
## MsoFillFormat.BackColor property

Obtient et définit la couleur d'arrière-plan du fichier.

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
    public class MsoFillFormatPropertyBackColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);
            MsoFillFormat fillFormat = arcShape.FillFormat;

            fillFormat.ForeColor = Color.Blue;
            fillFormat.BackColor = Color.LightBlue;
            fillFormat.Transparency = 0.5;

            Console.WriteLine("BackColor set to: " + fillFormat.BackColor.Name);

            workbook.Save("MsoFillFormatBackColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


