---
title: "Shape.CreateId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit l'identifiant de création pour cette forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/createid/
---
## Shape.CreateId property

Obtient et définit l'ID de création pour cette forme.

```csharp
public Guid CreateId { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyCreateIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 200, 150);
            
            // Créer et assigner un nouveau GUID comme CreateId
            Guid createId = Guid.NewGuid();
            shape.CreateId = createId;
            
            // Enregistrez le classeur
            workbook.Save("ShapeCreateIdDemo.xlsx");
            
            // Recharger le classeur pour vérifier que le CreateId persiste
            Workbook loadedWorkbook = new Workbook("ShapeCreateIdDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Afficher le CreateId pour vérification
            Console.WriteLine("Original CreateId: " + createId);
            Console.WriteLine("Loaded CreateId: " + loadedShape.CreateId);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


