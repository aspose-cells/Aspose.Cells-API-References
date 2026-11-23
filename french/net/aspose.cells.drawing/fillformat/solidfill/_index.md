---
title: "FillFormat.SolidFill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Obtient l'objet SolidFill"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/solidfill/
---
## FillFormat.SolidFill property

Obtient l'objet `SolidFill`.

```csharp
public SolidFill SolidFill { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertySolidFillDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Définir la couleur de remplissage solide pour la forme
            shape.Fill.SolidFill.Color = System.Drawing.Color.FromArgb(135, 222, 255);
            
            // Obtenir et afficher la couleur de remplissage solide
            System.Drawing.Color fillColor = shape.Fill.SolidFill.Color;
            Console.WriteLine("Solid Fill Color - R:{0}, G:{1}, B:{2}", 
                fillColor.R, fillColor.G, fillColor.B);
            
            // Enregistrez le classeur
            workbook.Save("SolidFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SolidFill](../../solidfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


