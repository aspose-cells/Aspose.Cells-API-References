---
title: "Shape.Spid"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Spécifie un identifiant de chaîne optionnel qu'une application peut utiliser pour identifier la forme particulière"
type: docs
url: /fr/net/aspose.cells.drawing/shape/spid/
---
## Shape.Spid property

Spécifie un identifiant de chaîne facultatif qu'une application peut utiliser pour identifier la forme particulière.

```csharp
public string Spid { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySpidDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangle à la feuille de calcul avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Obtenir et afficher la propriété Spid de la forme
            string spid = shape.Spid;
            Console.WriteLine("Shape SPID: " + spid);

            // Enregistrez le classeur
            workbook.Save("ShapePropertySpidDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


