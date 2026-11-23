---
title: "MsoLineFormat.ForeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "MsoLineFormat propriété. Obtient et définit la couleur de premier plan de la ligne de bordure"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformat/forecolor/
---
## MsoLineFormat.ForeColor property

Obtient et définit la couleur de premier plan de la ligne de bordure.

```csharp
public Color ForeColor { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyForeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
            
            // Définir les propriétés du format de ligne incluant ForeColor
            textBox.LineFormat.ForeColor = Color.Red;
            textBox.LineFormat.Style = MsoLineStyle.Single;
            textBox.LineFormat.IsVisible = true;
            textBox.LineFormat.Weight = 2;

            workbook.Save("MsoLineFormatForeColorDemo.xlsx", SaveFormat.Xlsx);
            
            // Vérifier la couleur enregistrée
            Workbook loadedWorkbook = new Workbook("MsoLineFormatForeColorDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Line ForeColor: " + loadedShape.LineFormat.ForeColor.ToString());
        }
    }
}
```

### Voir aussi

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


