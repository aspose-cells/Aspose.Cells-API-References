---
title: "ThreeDFormat.Material"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Représente le matériau prédéfini qui est combiné aux propriétés d'éclairage pour donner l'apparence finale d'une forme"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/material/
---
## ThreeDFormat.Material property

Représente le matériau prédéfini qui est combiné aux propriétés d'éclairage pour donner l'apparence finale d'une forme.

```csharp
public PresetMaterialType Material { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyMaterialDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer le formatage 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);
            shape.Text = "3D Material Demo";
            
            // Accéder au ThreeDFormat de la forme
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Afficher la valeur actuelle du matériau
            Console.WriteLine("Current Material value: " + threeDFormat.Material);

            // Définissez différents types de matériaux et observez les effets
            threeDFormat.Material = PresetMaterialType.Metal;
            Console.WriteLine("Material changed to Metal");

            threeDFormat.Material = PresetMaterialType.Plastic;
            Console.WriteLine("Material changed to Plastic");

            threeDFormat.Material = PresetMaterialType.Matte;
            Console.WriteLine("Material changed to Matte");

            // Configurez d'autres propriétés 3D pour mieux voir l'effet du matériau
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Enregistrer le classeur avec les effets 3D
            workbook.Save("ThreeDFormatMaterialDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


