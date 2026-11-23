---
title: "FillFormat.Transparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Retourne ou définit le degré de transparence de la zone sous forme d'une valeur de 0.0 opaque à 1.0 clair"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/transparency/
---
## FillFormat.Transparency property

Renvoie ou définit le degré de transparence de la zone comme une valeur de 0,0 (opaque) à 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer la transparence
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 200, 100, 50, 50);

            // Définir les propriétés de remplissage avec transparence
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            shape.Fill.Transparency = 0.3; // 30% transparent

            // Enregistrez le classeur
            workbook.Save("FillFormatTransparencyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


