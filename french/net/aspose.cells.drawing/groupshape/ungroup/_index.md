---
title: "GroupShape.Ungroup"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GroupShape. Dégroupe les éléments de forme"
type: docs
url: /fr/net/aspose.cells.drawing/groupshape/ungroup/
---
## GroupShape.Ungroup method

Dégroupe les éléments de forme.

```csharp
public void Ungroup()
```

### Remarques

Si la forme de groupe est groupée par une autre forme de groupe, rien ne sera fait.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapeMethodUngroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter deux formes rectangulaires
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 50);
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 3, 0, 100, 50);

            // Regrouper les formes dans un GroupShape
            GroupShape groupShape = worksheet.Shapes.Group(new Shape[] { shape1, shape2 });

            try
            {
                // Exécuter la méthode Ungroup
                groupShape.Ungroup();
                Console.WriteLine("Shapes ungrouped successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ungrouping: {ex.Message}");
            }

            workbook.Save("GroupShapeUngroupDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


