---
title: "FillFormat.FillType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Obtient et définit le type de remplissage"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/filltype/
---
## FillFormat.FillType property

Obtient et définit le type de remplissage

```csharp
public FillType FillType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Définissez un remplissage uni avec couleur
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Red;

            // Affichez le type de remplissage
            Console.WriteLine("Shape fill type: " + shape.Fill.FillType);

            // Passez à un remplissage en dégradé
            shape.Fill.FillType = FillType.Gradient;
            Console.WriteLine("Shape fill type changed to: " + shape.Fill.FillType);

            // Enregistrez le classeur
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


