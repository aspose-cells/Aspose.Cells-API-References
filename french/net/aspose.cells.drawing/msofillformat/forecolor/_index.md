---
title: "MsoFillFormat.ForeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFillFormat. Obtient et définit la couleur de premier plan du remplissage"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformat/forecolor/
---
## MsoFillFormat.ForeColor property

Obtient et définit la couleur de premier plan du remplissage.

```csharp
public Color ForeColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyForeColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire avec tous les paramètres requis
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Obtenir le format de remplissage
            MsoFillFormat fillFormat = rectangle.FillFormat;

            // Définissez et démontrez la propriété ForeColor
            fillFormat.ForeColor = System.Drawing.Color.Red;
            Console.WriteLine("ForeColor set to: " + fillFormat.ForeColor);

            // Modifiez la couleur ForeColor
            fillFormat.ForeColor = System.Drawing.Color.FromArgb(0, 128, 255);
            Console.WriteLine("ForeColor changed to: " + fillFormat.ForeColor);

            // Enregistrez le classeur
            workbook.Save("MsoFillFormatForeColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


