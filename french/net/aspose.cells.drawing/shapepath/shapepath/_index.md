---
title: "ShapePath.ShapePath"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur ShapePath. Initialise une nouvelle instance de la classe ShapePath"
type: docs
url: /fr/net/aspose.cells.drawing/shapepath/shapepath/
---
## ShapePath constructor

Initialise une nouvelle instance de la classe [`ShapePath`](../).

```csharp
public ShapePath()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créez un nouveau chemin de forme en utilisant la méthode #ctor
                ShapePath shapePath = new ShapePath();

                // Ajoutez des segments de chemin pour créer une forme simple
                shapePath.MoveTo(100, 100);
                shapePath.LineTo(200, 100);
                shapePath.LineTo(200, 200);
                shapePath.LineTo(100, 200);
                shapePath.Close();

                //ajouter une forme libre
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath });

                Console.WriteLine("ShapePath created and added to worksheet successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShapePath constructor: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("ShapePathMethodCtorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


