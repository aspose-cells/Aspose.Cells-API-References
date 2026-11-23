---
title: "Shape.MacroName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit le nom de la macro"
type: docs
url: /fr/net/aspose.cells.drawing/shape/macroname/
---
## Shape.MacroName property

Obtient et définit le nom de la macro.

```csharp
public string MacroName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMacroNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Définir le nom de la macro pour la forme
            shape.MacroName = "DoWork()";

            // Afficher la confirmation
            Console.WriteLine("Shape macro name set to: " + shape.MacroName);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


