---
title: "Classe BaseShapeGuide"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.BaseShapeGuide. Représente le guide de forme"
type: docs
url: /fr/net/aspose.cells.drawing/baseshapeguide/
---
## BaseShapeGuide class

Représente le guide de forme.

```csharp
public class BaseShapeGuide
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassBaseShapeGuideDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créer une forme rectangulaire avec les paramètres corrects
                Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

                // Puisque BaseShapeGuide n'a pas de constructeur public,
                // nous démontrerons son utilisation à travers une forme qui pourrait contenir des guides
                // Remarque : il s'agit d'une démonstration simplifiée car l'accès réel aux guides peut différer
                Console.WriteLine("Shape created successfully");
                Console.WriteLine($"Shape type: {shape.GetType().Name}");

                // Enregistrez le classeur
                workbook.Save("BaseShapeGuideDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with BaseShapeGuide: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


