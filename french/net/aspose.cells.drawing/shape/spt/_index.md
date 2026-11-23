---
title: "Shape.Spt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Spécifie un nombre optionnel qu'une application peut utiliser pour associer la forme particulière à un type de forme défini"
type: docs
url: /fr/net/aspose.cells.drawing/shape/spt/
---
## Shape.Spt property

Spécifie un nombre facultatif qu'une application peut utiliser pour associer la forme particulière à un type de forme défini.

```csharp
public int Spt { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySptDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un shape rectangle avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 100, 100, 100, 100);

            // Obtenez et affichez la propriété Spt
            int spt = shape.Spt;
            Console.WriteLine("Shape Spt value: " + spt);

            // Créez une nouvelle forme ovale pour démontrer une valeur Spt différente
            Shape ovalShape = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 1, 1, 100, 100, 100, 100);
            Console.WriteLine("Oval shape Spt value: " + ovalShape.Spt);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


