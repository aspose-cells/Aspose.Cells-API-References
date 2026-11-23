---
title: "Shape.Worksheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient l'objet Worksheet qui contient cette forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/worksheet/
---
## Shape.Worksheet property

Obtient l'objet [`Worksheet`](../../../aspose.cells/worksheet/) qui contient cette forme.

```csharp
public Worksheet Worksheet { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Démontrer l'utilisation de la propriété Worksheet
            Worksheet shapeWorksheet = shape.Worksheet;
            
            // Affichez le nom de la feuille de calcul pour montrer que la propriété fonctionne
            Console.WriteLine("Shape belongs to worksheet: " + shapeWorksheet.Name);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


