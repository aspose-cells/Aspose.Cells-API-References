---
title: "MsoFillFormat.IsVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFillFormat. Indique s'il y a un remplissage"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformat/isvisible/
---
## MsoFillFormat.IsVisible property

Indique s'il y a un remplissage.

```csharp
public bool IsVisible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme d'exemple
            Shape shape1 = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 100, 150);

            // Définir la visibilité du remplissage pour shape1 (visible)
            shape1.FillFormat.IsVisible = true;
            shape1.FillFormat.ForeColor = System.Drawing.Color.Red;
            
            // Définir la visibilité du remplissage pour shape2 (invisible)
            shape2.FillFormat.IsVisible = false;

            // Démontrer l'utilisation de la propriété IsVisible
            Console.WriteLine("Shape1 Fill Visible: " + shape1.FillFormat.IsVisible);
            Console.WriteLine("Shape2 Fill Visible: " + shape2.FillFormat.IsVisible);

            // Comparer la visibilité du remplissage entre les formes
            if (shape1.FillFormat.IsVisible && shape2.FillFormat.IsVisible)
            {
                Console.WriteLine("Both shapes have visible fills");
            }
            else
            {
                Console.WriteLine("At least one shape has invisible fill");
            }

            // Enregistrez le classeur
            workbook.Save("MsoFillFormatIsVisibleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


