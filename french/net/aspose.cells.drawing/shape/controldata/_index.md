---
title: "Shape.ControlData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient les données du contrôle"
type: docs
url: /fr/net/aspose.cells.drawing/shape/controldata/
---
## Shape.ControlData property

Obtient les données du contrôle.

```csharp
public byte[] ControlData { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyControlDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Accéder à ControlData (propriété en lecture seule)
            byte[] controlData = shape.ControlData;

            // Vérifier ControlData
            if (controlData != null)
            {
                Console.WriteLine("ControlData exists with length: " + controlData.Length);
            }
            else
            {
                Console.WriteLine("No data.");
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


