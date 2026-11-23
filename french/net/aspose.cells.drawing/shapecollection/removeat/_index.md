---
title: "ShapeCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Supprime la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/removeat/
---
## ShapeCollection.RemoveAt method

Supprime la forme.

```csharp
public void RemoveAt(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'indice de la forme. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter la première forme de rectangle
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Ajouter la deuxième forme de rectangle
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Supprime la première forme à l'index 0
            shapes.RemoveAt(0);

            // Enregistrez le classeur
            workbook.Save("ShapeCollectionRemoveAtDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


